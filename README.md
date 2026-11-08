# Kasavu Invites – professional multi-page site
Static site (no backend). 15 pages: Home, Themes, 6 theme pages, Pricing, Order, FAQ, About & Contact, Terms, Privacy, Refunds, plus robots.txt and 404.

## Publish (simplest)
1. Netlify Drop (app.netlify.com/drop): drag this whole folder in. Or Cloudflare Pages / GitHub Pages.
2. Open the link on your phone and test: menu, themes, order flow, Call/WhatsApp bar.

## Edit prices, themes, contact details
All content lives in `source/data.js`. Edit it, then run `node build.js dist` inside `source/` (needs Node.js), or send me the changes and I will rebuild.

## Turn on the growth features (all in `source/data.js`)
- `domain`: your final site address (e.g. https://yourname.in). Enables canonical tags, absolute WhatsApp preview image and sitemap.xml. Rebuild after setting it, then submit sitemap.xml in Google Search Console.
- `formEndpoint`: a Formspree or Netlify Forms URL so every order is also saved as a lead.
- `plausible`: your domain, to track WhatsApp clicks and order steps (cookie-free).
- `instagram`, `gst`: shown in the footer when filled in.

## Connect a domain
Buy a .in or .com, then in Netlify/Cloudflare add the custom domain and follow the DNS steps. HTTPS is automatic.

## Google Business Profile checklist
Create a profile for "Kasavu Invites" (service business, Chirakkadavu, Kottayam), add phone +91 80781 02296, the site link, 5+ sample photos, services and prices; ask real customers for reviews.

## Still needed from you
Delivery time, revision count, payment method/schedule and refund policy (pages currently say they are confirmed on WhatsApp before payment); Instagram handle; PIN code; GST number if registered; sample-couple permission for Archana & Gokul's photos; public demo links (the demo links go to private preview pages); a business email on your own domain later. Malayalam toggle covers the menu and home headline only; please proofread those strings in `build.js`.
