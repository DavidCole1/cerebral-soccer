# 360 Soccer Training website

Static site for Coach Daniel. No build step or dependencies. It uses plain HTML, CSS, and JavaScript and is ready for GitHub and Vercel.

## Pages

| File | Page |
|---|---|
| `index.html` | Home with hero, credentials, programs, testimonials, and inquiry form |
| `training.html` | Private & small group training, session structure, FAQ |
| `film-room.html` | Film analysis: how it works, interactive sample analysis, submission form, FAQ |
| `about.html` | Coach Daniel bio, license ladder, timeline, philosophy |

## Deploy (GitHub + Vercel)

1. Create a new GitHub repo (e.g. `360-soccer-training`) and push this folder's contents to the repo root.
2. In Vercel: **Add New → Project → Import** the repo.
3. Framework preset: **Other**. Leave build command and output directory empty. Deploy.
4. Add a custom domain in Vercel → Project → Settings → Domains when ready.

Any later edit: commit + push, Vercel redeploys automatically.

## Status

Live at https://360-soccer-training.vercel.app with forms connected through Formspree to dansoccerlab@gmail.com,
phone & email in footer, SEO files (sitemap.xml, robots.txt, JSON-LD), Search Console verified,
homepage indexed by Google. Google Business Profile created (verification pending).

## Remaining swaps

1. **Testimonials** use the four player and parent quotes supplied for the site.
2. **Instagram** currently points to instagram.com. Set Daniel's real profile URL or remove the link.
3. **Photos (optional)** can be replaced by overwriting `images/coach-huddle.jpg` and `images/coach-session.jpg`. No HTML changes are needed.
4. **Custom domain (optional)** can be added in Vercel under Settings, then Domains. Afterward, update the social URLs in all pages and `sitemap.xml`.

## Notes

- Fonts load from Google Fonts (Big Shoulders Display, Instrument Sans, Spline Sans Mono).
- The Film Room sample analysis is interactive: clicking a timestamped note switches the annotation on the tactical board (`main.js`).
- Tested at 1440px, 390px, 360px and 320px widths with no horizontal overflow. The mobile menu, film note sync, and form guard are verified.
- Accessibility: skip link, labeled inputs, `aria-current` nav state, visible focus styles, `prefers-reduced-motion` respected.
