# Assignment 1 — SEG3125

**Owen Ritchie** · #300299722
May 19, 2026

---

## 1. Previous experience and learning

I have prior experience writing JavaScript, primarily in the context of data scripts and small browser tools rather than full UI work. To build the necessary front-end and visual-design skills for this assignment, I worked through the following resources:

- **Net Ninja — Bootstrap 5 tutorial** ([YouTube playlist](https://www.youtube.com/playlist?list=PL4cUxeGkcC9joIM91nLzd_qaH_AimmdAR)) for grid, components, and utility classes.
- **W3Schools — Bootstrap 5 reference** ([w3schools.com/bootstrap5](https://www.w3schools.com/bootstrap5/index.php)) as a quick lookup for specific classes while building.elow.

## 2. Inspiration

Three portfolio sites that informed my design direction:

- **[seanhalpin.xyz](https://www.seanhalpin.xyz/)** — Liked. Restrained palette, generous whitespace, and a single typographic voice. The hierarchy comes from scale and spacing rather than ornament. Reinforced my decision to keep the layout tight and let typography do the work.
- **[francescofagioli.me](https://www.francescofagioli.me/)** — Liked. A personal, hand-built feel without sacrificing legibility. Showed me that a portfolio can feel distinct through small accent choices (color, italics) instead of heavy visual elements.
- **[eharshit.cfd](https://www.eharshit.cfd/)** — Liked. Very dense and information-rich, which is the opposite of where I landed. Useful as a contrast — it confirmed that I wanted a calmer page where each case study could stand on its own.

## 3. UI link

Live site: **[seg3125-six.vercel.app](https://seg3125-six.vercel.app/)**

## 4. Source code

GitHub repository: **[github.com/owenritchie/seg3125-a1](https://github.com/owenritchie/seg3125-a1)**

## 5. Design choices

### Colors

I used three colors:

- Off-white background `#f5f3ed`
- Near-black text `#1c1b18`
- Blue accent `#2c4fcc`

Plus two soft greys for secondary text and dividers.

I picked off-white instead of pure white and near-black instead of pure black because they're easier on the eyes for reading. The blue accent is the only bright color on the page — I use it for links, the section labels ("About", "How I work", "Case studies"), and the case-number tags. Keeping the accent to one color means anything blue on the page is either clickable or a heading, so the user knows where to look.

### Typography

The whole site uses **Bricolage Grotesque** from Google Fonts. I chose it because:

- It looks modern and personal without being too corporate or too playful.
- It has a nice italic, which I use for the word "data" in the hero so it stands out without needing a second font.
- It comes in many weights, so I can use one font for both big headlines and small labels.

Body text is 17px so it's easy to read. Section labels are smaller (13px) and uppercase so they look different from regular text.

### Screen layout

The page is a single column, 660px wide, centered on the screen. The nav menu sits vertically on the left side. Sections are separated by thin horizontal lines.

**Scale.** The hero headline is huge (80px) and the section labels are tiny (13px). This big difference makes the hero the first thing you see, while the labels stay out of the way.

**Visual hierarchy.** Reading top to bottom, the size and color guide your eye: big blue hero → small blue section label → body text → muted grey secondary text. The blue is only used on important things, so color helps show what matters most.

**Balance.** The nav is small and on the left; the content is the main weight in the middle. They balance each other even though they're not the same size. The case studies are arranged in a 2×2 grid with same-size images so the bottom of the page feels solid and even.

**Contrast.** I get contrast three ways: color (blue vs. cream), weight (bold headings vs. regular body text), and case (UPPERCASE labels vs. normal text). Together, these make the page easy to scan — you can find a section just by looking for the bold blue text.

## 6. Implementation notes

The site is hand-written HTML and CSS layered on **Bootstrap 5.3.3**. Bootstrap carries the layout grid (`row` / `col` / `row-cols-*`), the `list-group` for learning resources, `ratio` for image aspect ratios, `stretched-link` for whole-card clickability, `breadcrumb` and `alert` on case-study pages, and the full spacing/flex/text utility class system. Custom CSS overrides Bootstrap's component-level `--bs-*` CSS variables (e.g. `--bs-btn-color`, `--bs-list-group-bg`, `--bs-breadcrumb-divider-color`) to retheme the components in the project palette without rewriting their structure.
