# 🧪 Soedirman Student Summit 2025 (S3 2025) — Official Event Website

**Tech Stack:** SvelteKit 2 · Svelte 5 · TypeScript · TailwindCSS 4 · Vite 6 · Swiper.js · `@sveltejs/adapter-static` (SSG)

---

**Description:**
A fully static, multi-page event portal built for the Soedirman Student Summit 2025 (S3 2025) at Universitas Jenderal Soedirman (UNSOED), Indonesia. The site serves as the central digital hub for the event — presenting the university's 12 faculties, 6+ student organizations (UKM), regional student associations (Paguyuban), the event committee, sponsors, and a new-student guide (Gensoed Guide). Deployed as a pre-rendered static site for zero-runtime cost and instant global performance.

---

**Impact:**
- Delivers a single, canonical information source for thousands of incoming UNSOED students navigating the onboarding summit
- Zero server cost post-deployment through full static site generation (`adapter-static`), making the site resilient under high traffic spikes during the event period
- Covers all 12 UNSOED faculties with direct links and faculty-color-coded UI, reducing the friction of navigating a large and diverse university

---

**Key Contributions & Features:**
- **Dynamic slug-based routing** for UKM (`/ukm/[slug]`) and Paguyuban (`/paguyuban/[slug]`) detail pages with SSG pre-rendering, each surfacing events, galleries, and social contact links
- **Faculty explorer** with a Swiper.js carousel, unique per-faculty accent colors (Tailwind arbitrary values), and direct links to 12 official faculty sites
- **Committee showcase** page listing divisional leads (Project Officer, Secretary, Treasurer, Publications & IT, Design) with staff rosters and personal statements
- **Gensoed Guide & FAQ** pages targeted at new students, consolidating orientation content in one navigable location
- **Sponsorship & after-movies sections** on the homepage, supporting event documentation and partner visibility
- **Typed data layer** — all content (faculties, UKM, committees, events, sponsorships) modeled as typed TypeScript arrays, keeping templates logic-free and data easy to update
- **Prettier + ESLint (Svelte plugin)** enforced code style with `prettier-plugin-tailwindcss` for consistent class ordering across the component tree
