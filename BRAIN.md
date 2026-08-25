# BRAIN.md — Portfolio Project Notes

> Ye file project ka memory hai. Har session mein pehle ye padho,
> aur jab bhi koi update ho to neeche "Update Log" mein likhna.

## Project

- **Kiska portfolio:** Krishna Singh — Data Science Student & Builder
- **Folder:** `D:\krishna portfoli`
- **Files:** sirf `index.html` (sab kuch andar: HTML + CSS + JS, no framework)
- **Design (v2):** dark glassmorphism theme — film-grain overlay, floating blur orbs, pill navbar (active-link highlight), hero with typing effect + glass panel + stats, bento about-grid (profile / skill bars / education / hackathons / focus), full Certifications section, 3D-tilt project cards with per-card accent colors + shine hover, contact form (FormSubmit AJAX → mailto fallback), footer w/ quick links + socials, back-to-top btn, scroll progress bar. Fonts: Space Grotesk + Inter + JetBrains Mono. Reference: ameyajarvis.qzz.io ka structure, apna violet/cyan identity.
- **Vanta.js background (theme-wise):** fixed full-page 3D bg, theme ke hisaab se effect badalta hai — DAY = **BIRDS** (flock flying, cream bg #f6f1e6, birds violet #7c3aed + teal #0891b2), NIGHT = **NET** (plexus net, violet on dark). Theme toggle pe destroy + re-init. three.js r134 + vanta.net + vanta.birds CDN. prefers-reduced-motion ya CDN fail hone pe gracefully skip.
- **Theme toggle (day/night):** navbar mein sun/moon button. DAY = "Dark Charcoal on Warm Cream" (#f6f1e6 bg, #292419 charcoal text — user ne khud specify kiya). NIGHT = original dark. **DEFAULT = LIGHT (Warm Cream)** — user ne confirm kiya, system-pref ignore, localStorage `ks-theme` hi follow hota hai. Saare colors CSS vars se: `:root` = light values, `html[data-theme="dark"]` = dark override.
- **Hosting plan:** Cloudflare Pages / Vercel / GitHub Pages (free) — abhi local hi hai

## Content (source of truth)

| Item | Value |
|------|-------|
| Name | Krishna Singh |
| Role | Data Science Student & Builder |
| Degree | BSc Data Science @ BK Birla College, Kalyan (2024–27, pursuing) |
| Internship | ShadowFox DS intern, Jul 2026 (1 month) |
| Email | itsmekrishna1307@gmail.com |
| Phone | +91 86526 26657 |
| GitHub | github.com/itsmekrishna13-code |
| LinkedIn | linkedin.com/in/krishnasingh13 |

### Projects
1. **Vecna AI** — Jarvis-style voice desktop assistant (LiveKit voice, Gemini/Groq/OpenRouter routing, PC control). Built for TechXpression 2026. → github.com/itsmekrishna13-code/vecna-ai
2. **CineScore AI** (repo: netflix-rating-analysis) — Netflix EDA (30+ tasks) + IMDb rating prediction (Linear Regression, Random Forest), Tkinter GUI dashboard. → github.com/itsmekrishna13-code/netflix-rating-analysis
3. **Customer Churn Predictor** — Telco Kaggle dataset (7043 rows), Logistic Regression + Random Forest ~80% accuracy, feature importance + dashboard. → github.com/itsmekrishna13-code/customer-churn-prediction
4. **DataForge AI** — AI-powered data tooling backend → github.com/itsmekrishna13-code/dataforge-ai-backend

### Hackathons
- **SIH 2026 (Smart India Hackathon)** — abhi kar raha hai, ongoing
- **Hackverse 2026** — 12-hour National Level hackathon, **28 Jun 2026**, Team **AuraX** (Rohan Naik, Shubh Dwivedi, Aryan Rane + Krishna). Krishna ka pehla hackathon.
  - Project: **GlobeX** — AI-powered B2B global expansion platform; specialized AI agents (Market Research, Buyer Discovery, Lead Scoring, Trade Compliance, Outreach), 200+ countries data. Stack: React+Vite+Tailwind, Express+TS+Prisma+PostgreSQL(Supabase), FastAPI+Groq+ChromaDB agents.
  - GitHub: github.com/shubhdwd/GlobeX (teammate Shubh ke account pe) · Live: globe-x-ai.vercel.app
  - LinkedIn post: linkedin.com/posts/krishnasingh13_hackverse2026-hackathon-artificialintelligence-ugcPost-7481594813734367234-YrVc/
  - NOTE: Vecna AI TechXpression 2026 ke liye tha, Hackverse ke liye NAHI.
### Certifications (8)
Hackverse · Data Analysis & Visualization Using Python · Tata GenAI Job Sim · Commonwealth Bank Job Sim · British Airways Job Sim · Deloitte Australia Job Sim · AI Skills Passport · AI Fundamentals

## Pending / TODO (refresh list)

- [ ] **Photo** — milne pe `.avatar` div (hero section) ki jagah `<img src="Assets/photo.jpg" class="avatar">` lagana (index.html mein comment marked hai)
- [ ] **Resume PDF** — `Assets/Resume.pdf` daalo, hero mein "Download Resume" button add hoga
- [x] ~~DataForge AI~~ — link added: github.com/itsmekrishna13-code/dataforge-ai-backend
- [ ] **FormSubmit activation** — contact form ki PEHLI submission ke baad Krishna ke email pe activation link aayega, uspe click karna hoga
- [ ] **Hosting deploy** — site finalize hone ke baad Cloudflare Pages/Vercel pe push
- [x] ~~LinkedIn URL~~ — mil gaya: linkedin.com/in/krishnasingh13 (contact card + footer socials + footer links mein added)
- Note: user ne bola location/map NAHI chahiye — Kalyan map tile, location pill, location contact-card sab removed. Dobara mat daalna.
- [ ] Optional: custom domain, Google Analytics

## Update Log

| Date | Kya kiya |
|------|----------|
| 2026-08-23 | v1 banaya: single `index.html` — hero, stats, about, skills (13), 4 projects (READMEs se real descriptions), education+internship timeline, 8 certifications, contact cards, footer. Browser mein open karke check kiya. |
| 2026-08-23 | v2 rewrite: reference site jaisi premium glass/bento design. Naya: grain+orbs bg, pill navbar, typing hero, bento about w/ animated skill bars + Kalyan map tile, tilt project cards, contact form via formsubmit.co/ajax/itsmekrishna1307@gmail.com (PEHLI submission pe FormSubmit activation email Krishna ke inbox mein aayegi — uspe click karna zaroori, warna form fail hoga; fail hone pe mailto fallback hai), footer + back-to-top + progress bar. |
| 2026-08-23 | Location/map tile hataya (user request) — bento grid ab profile/craft/education/focus. LinkedIn add kiya: contact card (ci-blue), footer social icon, footer Say Hello link. URL: linkedin.com/in/krishnasingh13 |
| 2026-08-23 | Certifications ko full section banaya (user request, location ki jagah conceptually): `#certifications` section Projects ke baad — 8 cert cards (accent colors cycle cyan/purple/green/amber, award icon + number), About ke andar wala purana cert-strip removed. Nav pill/mobile menu/footer quick links mein "Certs/Certifications" add. |
| 2026-08-23 | Bento grid mein Focus ke bagal mein naya "Hackathons" tile: SIH 2026 (ongoing) + Hackverse 2026 (completed). Grid areas update: desktop `"profile craft craft" / "education hack focus"`. |
| 2026-08-23 | Hackverse tile real info se update: Team AuraX, 28 Jun 2026 12-hr national hackathon, project GlobeX (GitHub link shubhdwd/GlobeX + LinkedIn post link tile mein). Vecna/Hackverse wali galat line hatayi. |
| 2026-08-23 | Day/Night theme toggle add (user request): sun/moon btn navbar mein, DAY = Dark Charcoal on Warm Cream, NIGHT = original dark, system-pref default + localStorage persist. Saari hardcoded dark colors CSS vars mein convert kiye. |
| 2026-08-23 | Warm Cream ko DEFAULT theme banaya (user request) — site ab hamesha cream mode mein khulti hai, toggle se night ho sakti hai. |
| 2026-08-23 | Vanta.js NET effect add (user ne vantajs.com/?effect=net bheja): fixed full-page animated net bg, theme-aware colors, toggle pe re-init. NOTE: three.js r134 + vanta CDN chahiye — internet ke bina net effect nahi dikhega, baaki sab chalega. |
| 2026-08-23 | Day mode ka effect BIRDS pe switch kiya (user ne vantajs.com/?effect=birds bheja): light = birds flock, dark = net. Toggle pe effect bhi swap hota hai. |
| 2026-08-23 | PERFORMANCE FIX (user bola site laggy hai): saare cards/tiles/form se backdrop-filter blur hataya (sirf nav-pill pe rakha), surface alpha badhaya (.78/.82) taaki bina blur bhi readable rahe, .rv classes se will-change removed (~30 layers freed), orbs pe will-change:transform, Vanta frames ~40fps pe capped (rAF limiter), NET points 14→11 + maxDistance 24→20, BIRDS speedLimit 4→3. |
| 2026-08-23 | BUG FIX: pehla rAF limiter galat tha — throttled frame pe callback drop karta tha jisse Vanta ki animation loop permanently mar jaati thi (bg ek jagah freeze). Naya limiter setTimeout-based hai jo callback ko delay karke execute karta hai, loop zinda rehti hai. |
| 2026-08-23 | rAF monkey-patch POORE tarah remove kar diya (Chrome mein vanta break ho raha tha) — global rAF ko patch karna three.js/vanta ke liye risky hai. Perf ab backdrop-filter removal + lighter vanta config se hi handle hota hai. |

---
*Last updated: 2026-08-23*
