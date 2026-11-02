# InvoicePro by RMH Creative Studio

A React + Vite starter application for a free invoice generator and small-business tools.

## Run locally

```bash
npm install
npm run dev
```

Create a production build with `npm run build`; deploy the `dist/` directory to Netlify or Vercel.

## Configure Google AdSense

AdSense is prepared but intentionally inactive until valid details are supplied.

1. Obtain a publisher account and have the website/domain reviewed by Google.
2. Set `VITE_ADSENSE_CLIENT=ca-pub-XXXXXXXXXXXXXXXX` in the deployment environment.
3. Set the relevant ad-slot environment variables:
   - `VITE_ADSENSE_HOME_SLOT`
   - `VITE_ADSENSE_HOME_MID_SLOT`
   - `VITE_ADSENSE_TEMPLATES_SLOT`
   - `VITE_ADSENSE_TOOLS_SLOT`
4. Rebuild and redeploy. The reusable `AdBanner` component only renders when a publisher ID and a real slot ID are configured.
5. For Auto Ads, configure them in AdSense after site approval and follow Google's current instructions. Do not paste fabricated IDs.

**Important:** This project does not connect to an AdSense account, guarantee approval, or implement a consent-management platform. Review Google's current publisher policies and applicable privacy/consent requirements before enabling ads. If the site owner is under 18, an adult parent or guardian must handle the AdSense account.

## Before publishing

- Replace `YOUR-DOMAIN.example` in `index.html`, `public/robots.txt`, and `public/sitemap.xml`.
- Set a real support email and update the Contact page in `src/App.jsx`.
- Review Privacy, Terms, Disclaimer, and tax-related content for your jurisdiction.
- Add a real cookie/consent solution if required for your audience and advertising setup.
- Add your own canonical domain, social preview image, and verified business details.
- Test PDF output, print output, mobile layout, backups and restore on the deployment domain.

## Current scope

Included: responsive landing page, animated/floating hero artwork, local invoice and client storage, invoice calculations, live invoice preview, PDF export, print, invoice list and status actions, client list, ten template showcase cards, six working calculator views, blog guide pages, business settings, JSON backup/restore, legal/trust page drafts, theme toggle, SEO metadata, robots and sitemap files, configurable AdSense component.

This is a deployable starter, not a legal/tax compliance certification. Some advanced items from the original brief—true multi-page invoice pagination, full template-specific PDF rendering, advanced client editing/history, a production consent platform, and a full article CMS—need further implementation and testing before calling the site production-ready.
