# Portfolio — Websites, SEO & AI

A single-page, static portfolio site: services, featured case study (Atharva Aqua), project grid with
completed / in-progress filter, skills, experience and contact.

## Run

No build step. Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Editing

Everything you will normally change lives in the `<script>` block at the bottom of `index.html`:

| Constant | Drives |
| --- | --- |
| `PROFILE` | Contact links (email, phone, WhatsApp, LinkedIn, GitHub). Empty string hides a link. |
| `PROJECTS` | Project cards. `status: "done"` or `"wip"`; `progress` (0–100) shows for `wip`. |
| `TESTIMONIALS` | Client reviews. The section stays hidden while this is empty. |

Experience and education are plain HTML in the `#experience` section. Project thumbnails live in `images/`.

## Deploy

Static files only, so any host works: GitHub Pages (Settings → Pages → deploy from `main`, root),
Cloudflare Pages, Netlify, Vercel, or shared hosting such as Hostinger.
