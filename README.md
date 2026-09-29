# Think ML

A password-gated, scroll-driven "film" that pitches Think ML, the AI extension of Think Neuro, to Michael. Sixteen scenes: the thesis, the gap, the lineage from Think Neuro, the audience, the two-track product (live cohort and the automated Autopilot track), the advisor model, the ten-week curriculum, the flywheel, the five-phase scale plan, an interactive revenue model, go-to-market, risks, the first ninety days, and the ask.

## Run it

It is a single static file. Open `index.html` in a browser, or serve the folder:

```
npx serve .
```

Deploy anywhere that hosts static files (GitHub Pages, Vercel, Netlify). No build step.

## Stack

- Vanilla HTML, CSS and JavaScript in one file
- GSAP 3 with ScrollTrigger for pinned, scrubbed scenes
- Lenis for smooth scrolling (falls back to native scrolling if it fails to load)
- Canvas neural field that reacts to the mouse and to scroll velocity
- Google Fonts: Bricolage Grotesque, Instrument Serif, JetBrains Mono

## The gate

The password check is client-side and exists to keep casual visitors out, not to secure the content. Anyone who reads the source can recover it. If the plan ever needs real protection, put the file behind hosting-level auth (for example Vercel password protection or Cloudflare Access).

Once entered, the unlock is remembered for the browser session.

## Notes

- All figures on the page are labelled illustrative. The revenue model in scene 12 is driven by sliders so the assumptions can be argued with live.
- The advisor companies shown are a target pool, not signed partners. The page says so.
- Motion respects `prefers-reduced-motion`. Horizontal scenes stack vertically on phones.
