git clone https://github.com/YOUR_USERNAME/ride-local-impact-global.git

# Ride Local, Impact Global

## Quick Start

### Prerequisites
- Node.js 18+
- npm

### Install dependencies
```bash
npm install
```

### Run the Vite React app
```bash
npm run my-app:dev
```

### Build for production
```bash
npm run my-app:build
```

### Preview production build
```bash
npm run my-app:preview
```

---

This repo uses a single root `package.json` and lockfile. The Vite React app source is in `my-app/`.

---

---

## 📁 Project Structure

```
/
├── components/           # React components
│   ├── About.tsx
│   ├── BetaBanner.tsx   # NEW: Beta launch banner
│   ├── CarbonCalculator.tsx
│   ├── CookieConsent.tsx # NEW: Cookie consent banner
│   ├── EducationalDisclaimer.tsx # NEW: Legal disclaimer
│   ├── ESGEducation.tsx
│   ├── Footer.tsx
│   ├── GivebackTracker.tsx
│   ├── GoogleAnalytics.tsx # NEW: GA4 integration
│   ├── Hero.tsx
│   ├── Navbar.tsx
│   ├── PrivacyPolicy.tsx # NEW: Privacy policy modal
│   ├── SEOHead.tsx      # NEW: Meta tags for SEO
│   ├── ShopPreview.tsx
│   ├── StrategicShowcase.tsx
│   ├── TermsOfService.tsx # NEW: Terms modal
│   ├── Testimonials.tsx
│   └── TutorialHub.tsx
├── data/
│   └── mockData.ts      # App data and content
├── public/
│   ├── robots.txt       # NEW: SEO crawler instructions
│   └── sitemap.xml      # NEW: SEO sitemap
├── styles/
│   └── globals.css      # Global styles and Tailwind
├── App.tsx              # Main app component
├── DEPLOYMENT_GUIDE.md  # NEW: Step-by-step deployment
├── LAUNCH_CHECKLIST.md  # NEW: 1-hour launch plan
└── POST_LAUNCH_GUIDE.md # NEW: Growth strategy
```

---

## ✅ Features

### Core Modules
- 🎯 **Hero Banner** - Rotating showcase of Salt Lake bikeways + Velotric bikes
- 🤝 **Strategic Partners** - Velotric, LINKA (investment CTA), Sweet Streets
- 📊 **Carbon Calculator** - Interactive CO2 savings estimator
- 💬 **Testimonials** - Community feedback carousel
- 🎓 **Tutorial Hub** - Embedded educational videos
- 🛒 **Shop Preview** - E-bike product showcase
- 🎓 **SLCC Tracker** - Scholarship giveback visualization
- 📚 **ESG Education** - Downloadable resources, Utah incentives

### Launch Features (NEW!)
- ✅ **Beta Banner** - Dismissible launch announcement
- ✅ **Cookie Consent** - GDPR/CCPA compliant banner
- ✅ **SEO Optimization** - Meta tags, Open Graph, Twitter cards
- ✅ **Google Analytics** - GA4 integration (ready for your ID)
- ✅ **Legal Compliance** - Privacy Policy, Terms, Educational Disclaimer
- ✅ **Email Collection** - Google Form integration
- ✅ **Mobile Responsive** - Works on all devices

---

## 🔧 Configuration

### Google Analytics Setup
1. Create Google Analytics 4 property at [analytics.google.com](https://analytics.google.com)
2. Copy your Measurement ID (format: `G-XXXXXXXXXX`)
3. Open `/components/GoogleAnalytics.tsx`
4. Replace `'G-XXXXXXXXXX'` with your actual ID
5. Deploy changes

### Email Subscription
Currently connected to Google Form:
- Form URL: `https://docs.google.com/forms/d/e/1FAIpQLSegfr_SXvyq-AqE9vHyupO2fFkXcIlTMi6NFuZfrnaxRMh8Nw/viewform`
- Update in `/components/Footer.tsx` if using different form

### Contact Information
Update these in `/components/Footer.tsx`:
- Email: `contact@ridelocalimpactglobal.org`
- Phone: `801-999-8053`
- Location: Salt Lake City, Utah

### LINKA Investment Email
Update in `/data/mockData.ts` if changing email:
- Current: `ridelocalimpactglobal@gmail.com`

---

## 🚀 Deployment

### Vercel (Recommended - Free)

**1-Click Deploy:**
```bash
# Push to GitHub
git add .
git commit -m "Initial deployment"
git push

# Go to vercel.com
# Connect GitHub repo
# Click Deploy
```

**Custom Domain:**
1. Add domain in Vercel project settings
2. Update DNS records at your registrar
3. Wait for DNS propagation (5-30 min)
4. Automatic SSL/HTTPS enabled!

**Full deployment guide:** See `/DEPLOYMENT_GUIDE.md`

### Other Platforms
- **Netlify:** Drag and drop `/dist` folder
- **Cloudflare Pages:** Connect GitHub repo
- **AWS Amplify:** Use Amplify Console
- **GitHub Pages:** Requires additional config

---

## 📊 Tech Stack

- **Framework:** React 18 + TypeScript
- **Build Tool:** Vite
- **Styling:** Tailwind CSS v4
- **Icons:** Lucide React
- **Charts:** Recharts
- **Forms:** React Hook Form
- **Carousel:** React Slick
- **Animations:** Motion (formerly Framer Motion)
- **Hosting:** Vercel (recommended)
- **Analytics:** Google Analytics 4
- **Email:** Google Forms

---

## 🎨 Design System

### Colors
- **Primary:** Green (`#10b981` / `bg-green-500`)
- **Accent:** Blue for investment CTAs
- **Neutral:** Grays for text and backgrounds
- **Success:** Green-400
- **Warning:** Amber-500

### Typography
- Configured in `/styles/globals.css`
- Default system fonts with fallbacks
- Responsive sizing via Tailwind

### Components
- Reusable UI components in `/components/ui/`
- Accessible form controls
- Responsive cards and modals

---

## 📋 Pre-Launch Checklist

Before going live, ensure:

- [ ] Update Google Analytics ID in `GoogleAnalytics.tsx`
- [ ] Verify contact email in `Footer.tsx`
- [ ] Add favicon files to `/public` folder
- [ ] Test email subscription flow
- [ ] Review all legal disclaimers
- [ ] Test on mobile devices
- [ ] Check all external links
- [ ] Verify LINKA investment email CTA
- [ ] Test cookie consent banner
- [ ] Confirm DNS settings for domain

**Full checklist:** See `/LAUNCH_CHECKLIST.md`

---

## 🎯 Post-Launch Strategy

### Week 1 Goals
- [ ] Gather 3-5 real testimonials
- [ ] Reach out to Velotric for affiliate partnership
- [ ] Contact LINKA about investment opportunity
- [ ] Start SLCC scholarship partnership discussion
- [ ] Share on social media (personal accounts)
- [ ] Join Utah cycling Facebook groups

### Month 1 Goals
- [ ] 500+ website visitors
- [ ] 100+ email subscribers
- [ ] 1 partnership formalized
- [ ] Create social media accounts
- [ ] Publish 4 blog posts (if adding blog)

### Month 3 Goals
- [ ] 3,000+ website visitors
- [ ] 500+ email subscribers
- [ ] 3+ active partnerships
- [ ] Award first SLCC scholarship ($500)

**Full strategy:** See `/POST_LAUNCH_GUIDE.md`

---

## 🤝 Partnership Opportunities

### Current Status
- **Velotric:** Partnership pending (featured in shop preview)
- **LINKA:** Investment opportunity (pitch deck CTA active)
- **Sweet Streets:** Partnership pending (strategic showcase)
- **SLCC:** Scholarship prototype (formalization needed)

### Interested in Partnering?
Contact us:
- **Email:** contact@ridelocalimpactglobal.org
- **Phone:** 801-999-8053
- **Investment Inquiries:** Use "Request Pitch Deck" button on site

---

## 📜 Legal & Compliance

### Implemented
- ✅ Privacy Policy (comprehensive)
- ✅ Terms of Service (comprehensive)
- ✅ Educational Disclaimer (detailed)
- ✅ Cookie Consent (localStorage-based)
- ✅ Beta disclaimers (transparency)
- ✅ Investment disclaimers (not financial advice)
- ✅ Partnership status transparency

### Disclaimers
- Platform is for educational purposes
- No active affiliate partnerships (pending formalization)
- Testimonials are illustrative (beta phase)
- SLCC tracker is prototype (partnership pending)
- Investment opportunities require independent verification

---

## 🐛 Troubleshooting

### Development Issues
```bash
# Clear cache and reinstall
rm -rf node_modules package-lock.json
npm install

# Clear Vite cache
rm -rf .vite
npm run dev
```

### Build Issues
```bash
# Check for TypeScript errors
npm run build

# Test production build locally
npm run preview
```

### Analytics Not Tracking
1. Verify Google Analytics ID is correct
2. Check browser console for errors
3. Ensure cookies are accepted (analytics only loads after consent)
4. Wait 24-48 hours for data to appear in GA dashboard

---

## 📈 Success Metrics

### Key Performance Indicators (KPIs)
- **Traffic:** Google Analytics pageviews
- **Engagement:** Time on site, carbon calculator usage
- **Conversions:** Email subscriptions, partnership inquiries
- **Revenue:** Affiliate commissions (when active)
- **Impact:** SLCC scholarships awarded

### Tracking
- Google Analytics dashboard for traffic
- Google Form responses for email subscribers
- Email inbox for partnership inquiries
- Spreadsheet for revenue/scholarship tracking

---

## 🌱 Future Enhancements

### Phase 2 (Month 2-3)
- Blog section for content marketing
- Downloadable e-bike buyer's guide
- Email automation (welcome sequence)
- Heatmap tracking (Hotjar/Clarity)

### Phase 3 (Month 4-6)
- User accounts/profiles
- Community forum
- Event calendar
- Scholarship application portal

### Phase 4 (Year 1+)
- E-commerce integration (merch)
- Mobile app
- Advanced personalization
- Multiple scholarship programs

---

## 🙏 Acknowledgments

**Built for:**
- Utah's e-bike community
- SLCC students pursuing education
- Local businesses supporting sustainability
- Environmental advocates

**Powered by:**
- React + Vite
- Tailwind CSS
- Vercel hosting
- Open source community

---

## 📞 Contact & Support

**Project Contact:**
- Email: contact@ridelocalimpactglobal.org
- Phone: 801-999-8053
- Location: Salt Lake City, Utah

**Technical Issues:**
- Create issue in GitHub repository
- Check `/DEPLOYMENT_GUIDE.md` for common fixes

**Partnership Inquiries:**
- Use website contact form
- Email directly with "Partnership" in subject
- Investment opportunities: Use "Request Pitch Deck" CTA

---

## 📄 License

© 2025 Ride Local, Impact Global. All rights reserved.

This is an educational platform. See Terms of Service and Privacy Policy for details.

---

## 🚴‍♂️ Let's Ride!

**Ready to launch?** Follow the guides in order:
1. `/DEPLOYMENT_GUIDE.md` - Get online in 60 minutes
2. `/LAUNCH_CHECKLIST.md` - Pre-flight verification
3. `/POST_LAUNCH_GUIDE.md` - Growth and partnerships

**Together, we're building a sustainable future for Utah, one e-bike at a time.** 🌟

---

*Last Updated: December 4, 2024*
