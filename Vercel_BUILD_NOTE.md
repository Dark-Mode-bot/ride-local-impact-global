Vercel Build Fix — 2025-12-05
=================================

Summary
-------
On 2025-12-05 I moved `vite` from `devDependencies` into the root `dependencies` and updated root npm scripts to run Vite with `--root my-app`.

Reason
------
On Vercel the production install step can skip `devDependencies`, which caused the build to fail with:

  sh: line 1: vite: command not found

This happens because the `vite` binary wasn't installed into `node_modules/.bin` when the build ran.

What changed
------------
- Moved `vite` into the root `dependencies` so the Vite CLI is available during production installs.
- Updated root scripts to run Vite from the repository root using `--root my-app`:
  - `build`: `vite build --root my-app`
  - `preview`: `vite preview --root my-app`
  - `dev`: `vite --root my-app`

Why this is safe
-----------------
This keeps `my-app/` as a source-only folder and ensures a single root installation of Vite is used for CI/build environments (including Vercel). It prevents production installs that skip devDependencies from breaking the build.

How to revert or alternative approaches
--------------------------------------
If you prefer a different workflow, you can revert by either:

1. Restoring a `my-app/package.json` with `vite` as a `devDependency` and configure Vercel to use `my-app` as the project root (preferred if `my-app` should be standalone).
2. Keep `vite` as a `devDependency` and change Vercel's Install Command (Project Settings) to `npm install` so devDependencies are installed during build.
3. Move `vite` back to `devDependencies` in root `package.json` if you add a root build step that installs devDependencies before running the build.

Contacts / Notes
----------------
Commit: "Move vite to dependencies and run Vite from root with --root my-app for build/preview"
If you want this changed to a different approach (restore `my-app/package.json`, or change Vercel settings), tell me which option and I'll apply it.
