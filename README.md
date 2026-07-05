# 🏗️ EGC El Gezawy Construction Website

Complete responsive multi-page website for EGC (El Gezawy Construction) — an Egyptian construction and finishing company.

## 📄 Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Hero, badges, about teaser, services, projects, why us, CTA |
| Services | `services.html` | 16 construction services in a responsive grid — click any card to open a detail popup |
| Projects | `projects.html` | 12 projects with category filter — click any card to open a detail popup |
| About | `about.html` | Company story, stats counter, team, vision & mission |
| Contact | `contact.html` | Working contact form, contact info, embedded Google Map |

## 🎨 Design System

- **Colors:** Gold (#C9A258), Navy Dark (#0B1120)
- **Font:** Cairo (Google Fonts)
- **Direction:** Arabic RTL
- **Framework:** Pure HTML + CSS + Vanilla JS (no dependencies)

## 🚀 Deploy to GitHub Pages

1. Create a new repository on GitHub
2. Upload these 5 HTML files to the root of the repository (not inside a subfolder)
3. Add an empty file named `.nojekyll` to the root (prevents Jekyll from interfering with plain HTML)
4. Go to **Settings → Pages** → Source: "Deploy from a branch" → Branch: `main` / `(root)`
5. Your site will be live at: `https://yourusername.github.io/repo-name/`

> If a deployment ever fails with **"Deployment failed, try again later"**, this is a known, temporary GitHub-side issue — not a problem with the files. Toggling Source to "GitHub Actions" and back to "Deploy from a branch" in Settings → Pages usually resolves it, or simply retry after a few minutes.

## 📱 Responsive Breakpoints

- Desktop: > 1100px
- Tablet: ≤ 1100px / ≤ 900px
- Mobile: ≤ 600px

## ✅ Features

- [x] Fixed navbar with scroll effect + mobile hamburger menu
- [x] 16 service cards, each opening a detail popup (image, icon, description, CTA)
- [x] 12 project cards with category filter, each opening a detail popup (image, category, location, year, description)
- [x] Animated stats counter (IntersectionObserver)
- [x] Contact form that actually sends submissions via [FormSubmit](https://formsubmit.co) — no backend required
- [x] Embedded Google Map on the contact page
- [x] Self-contained inline SVG placeholder graphics (no broken images, no external dependency)
- [x] Full SEO meta tags (per page)
- [x] Schema.org JSON-LD
- [x] Open Graph / Twitter Cards
- [x] Semantic HTML structure

## ⚙️ Before going live — update these placeholders

| What | Where | Current placeholder |
|------|-------|----------------------|
| Phone / WhatsApp | all pages (footer, contact page, `tel:`/`wa.me` links) | `01000725551` |
| Contact form destination email | `contact.html` (form `action` + JS `fetch` URL) | `ahmed.capito@gmail.com` |
| Facebook / Instagram links | footer + contact page | `#` (not linked yet) |
| Exact company address | `contact.html` map embed | generic "Cairo, Egypt" |
| Real project & team photos | `services.html`, `projects.html`, `about.html` | inline SVG / stock placeholders |

**Note on the contact form:** the first time someone submits it, FormSubmit sends a one-time confirmation email to the destination address — it must be clicked once to activate delivery of future submissions.
