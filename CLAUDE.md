# Israel–India Innovation Week · Coimbatore 2027 — event site

Live site: https://promitei-org.github.io/israel-india-hackathon2027/
Hosting: GitHub Pages from `main`, repository root. Every push to `main` goes live in about a minute.

## Structure
- `index.html` — the whole site in one file: CSS in `<style>`, small router script at the end, inline SVG artwork.
- `assets/` — images and logos (flyer logos are `fl_*.png`, English Ariel logo is `ariel_en.png`). Innovation Centre renders are `cic-*.jpg` (cut from the CIC deck with the Biopharmax watermark band cropped off); `era.png` is the ERA IT Consulting logo from the same deck. Interior stills `cic-int-*.jpg` are frames from the CIC flythrough video (WhatsApp video, 18 Nov 2026, 480p), cropped above the on-screen captions and Biopharmax logo; the video itself is not in the repo.
- The CIC deck (`Cyber_Innovation_Center_PPT.pdf`) is NOT stored in the repo: the repo is public and the deck contains the budget, cost breakdown and Biopharmax markup. Never publish budget, costs, schedule or floor programme from it.
- Views are switched by the URL hash (plain `#name` only):
  - `#` (empty) — start screen with three parallel banners
  - `#hackathon` — 1 Feb, Israel–India Global Innovators Hackathon 2027 "Long Live Data" (venue SRCW)
  - `#industry-day` — 2 Feb, Industry Day (venue SREC SPARK)
  - `#conference` — 3 Feb, International Scientific Conference (SRCW with Ariel University)
- All three event pages share the `hk` style (`class="pg-… hk"`): hero with the brand lockup and a Chakra Petch title, sticky `.hk-subnav`, `hk-sec` sections alternating white/tint, `hk-cta` band at the end. Per-day colour overrides live under `.pg-ind` / `.pg-conf`.
- Image galleries use `[data-gal]` (thumbnails, arrows, swipe, full-screen `.lb` lightbox with Esc/arrow keys). Images never open in a new tab. To add an image, add a thumbnail `<button data-src data-cap>` to `.gal-thumbs`.
- Chamber section background: tinted Israel and Tamil Nadu outlines (inline SVG, simplified from public GeoJSON: Natural Earth 10m for Israel, geohacker/india for Tamil Nadu). By Mark's decision the Israel outline includes the West Bank, the Gaza Strip and the Golan Heights.
- In-page navigation uses `<button data-go="section-id">` (smooth scroll), never `#section` links, because the hash is used for routing.

## Design rules
- Style follows the hackathon flyer: navy `#0C1A2D` to teal `#09AE80` gradients, data-dot "bokeh", four colour dots (blue `#3094FF`, white, orange `#FF9933`, green `#138808`), orange accent `#C9761B` / `#FC9732`.
- Fonts: Archivo (wide, `font-stretch:125%` for headings), Chakra Petch for "LONG LIVE DATA", Inter for body.
- Flat layout: no boxed "cards" with backgrounds and rounded corners. Use thin coloured left lines, dividers and plain logos instead. Organisers are shown as logos only.
- Colour per day: Hackathon teal, Industry Day orange, Conference blue.
- Sections without confirmed content show `<span class="hk-soon">Info available soon</span>`. Never invent facts, names, prices or dates.

## Content facts (confirmed)
- Hackathon: registration 1 Dec 2026 – 7 Jan 2027; proposal by 11 Jan; shortlisting 12–15 Jan (20 teams per track); online 17–31 Jan; final defense 1 Feb at SRCW, Coimbatore. Teams of 3–4. Tracks: FROM HEALTH RECORDS (AI, IT, data) and TO RECORD HEALTH (biotech, life science, longevity).
- Registration form (Google Forms): https://docs.google.com/forms/d/e/1FAIpQLScEMz4rVoQZzacMbOktG83VV28Fr87YQ7xnI-uB3hmg0mNEqA/viewform
- Hackathon contact: hackathon@promitei.com. Industry Day inquiries: mark@promitei.com.
- Industry Day 2 Feb at SREC SPARK (Sri Ramakrishna Engineering College, Vattamalaipalayam, Coimbatore 641022): opening of the Israel–Tamil Nadu Chamber of Commerce; foundation stone of the first AI, Data and Cyber Innovation Centre in Tamil Nadu; workshops and networking; plenary discussions. Organised by SREC, TechGuard Labs Foundation, Promitei, SNR Sons Charitable Trust, MASHAV, Consulate General of Israel to South India, Israel Economic and Trade Mission (Bengaluru).
- Innovation Centre: "TechGuard Cyber Innovation Centre", subtitle "The first AI, Data and Cyber Innovation Centre in Tamil Nadu". Initiative of TechGuard Labs Foundation (a joint Israel–India foundation), on the SREC campus, Coimbatore. Partners shown: SNR Sons Charitable Trust, SREC, Ariel University, ERA IT Consulting & Audit, Promitei, Biopharmax. Renders are labelled as architectural concept visualisations.
- Israel–Tamil Nadu Chamber of Commerce: only confirmed fact is "a new platform for business cooperation between Israel and Tamil Nadu", launched on 2 Feb. The section text is general by agreement.
- Conference content comes from the SRCW brochure (dates, plenary sessions with Prof. Izhak Michaelevski, Prof. Amit Dvir, Dr. Nadia Iermakov, fees, advisory board).

## Open items
- Industry Day: registration link, speakers, participants and sponsors (Biopharmax India confirmed), sponsorship packages and company participation fees (draft tiers proposed, not yet approved; legal entity for invoicing to be decided).
- Chamber of Commerce: founding members, membership, how to join, dedicated contact.
- Hackathon: prize amounts, mentors and jury list, rules and FAQ answers marked "Info available soon".
- Google Form confirmation message still says mark@promitei.com (change in the form settings).
