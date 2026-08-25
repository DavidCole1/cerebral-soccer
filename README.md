# Cerebral Soccer website

Static site for Coach Daniel. No build step or dependencies. The site uses plain HTML, CSS, and JavaScript and is ready for GitHub and Vercel.

## Pages

| File | Page |
|---|---|
| `index.html` | Home page with hero, credentials, programs, approach, and inquiry form |
| `training.html` | Private & small group training, session structure, FAQ |
| `film-room.html` | Film analysis: how it works, interactive sample analysis, submission form, FAQ |
| `about.html` | Coach Daniel bio, license ladder, timeline, philosophy |

## Deploy (GitHub + Vercel)

1. Create a new GitHub repo (e.g. `cerebral-soccer`) and push this folder's contents to the repo root.
2. In Vercel: **Add New → Project → Import** the repo.
3. Framework preset: **Other**. Leave build command and output directory empty. Deploy.
4. Add a custom domain in Vercel → Project → Settings → Domains when ready.

Any later edit: commit + push, Vercel redeploys automatically.

## Status

Live at https://cerebral-soccer.vercel.app. Forms are connected through Formspree to dansoccerlab@gmail.com. Contact details appear in the footer, SEO files are in place, Search Console is verified, and Google has indexed the homepage. The Google Business Profile has been created and is awaiting verification.

## Optional next steps

1. **Real testimonials:** Add verified family or player quotes when permission has been confirmed.
2. **Instagram:** Add Daniel's profile when the final account URL is available.
3. **Photos:** Overwrite the images in `images/` at any time. No HTML changes are needed when filenames stay the same.
4. **Custom domain:** Add it in Vercel → Settings → Domains, then update the canonical, og:url, and og:image URLs on every page and in sitemap.xml.

## Notes

- Fonts load from Google Fonts (Big Shoulders Display, Instrument Sans, Spline Sans Mono).
- The Film Room sample analysis is interactive: clicking a timestamped note switches the annotation on the tactical board (`main.js`).
- Tested at widths of 1440px, 390px, 360px, and 320px. There is no horizontal overflow, and the mobile menu, film-note sync, and form guard are verified.
- Accessibility: skip link, labeled inputs, `aria-current` nav state, visible focus styles, `prefers-reduced-motion` respected.
