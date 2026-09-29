# New Era Studios Website

Static website for New Era Studios: an AI-native creative studio for series slates and brand campaigns.

## Pages

| File | Page |
|---|---|
| `index.html` | Home: scroll intro, portfolio panels, services, clients, process, signals, footer |
| `work.html` | Projects index: filterable grid, full-length video player |
| `contact.html` | Contact page |

No build step. Open `index.html` in a browser or serve the folder with any static host.

## Videos (hosted on Bunny.net)

Video files are **not** stored in this repository (see `.gitignore`). The pages expect them at these paths:

```
videos/hero.mp4                  home hero + Porsche panel
videos/viking.mp4                portfolio panel
videos/zara-commercial.mp4       portfolio panel
videos/hm.mp4                    portfolio panel
videos/*-30.mp4                  30-second silent loops (Signals tiles, Projects grid)
videos/burning-car.mp4           Projects page closing banner
videos/contact-banner.mp4        Contact page background
videos/cta-logo.mp4              3D logo loop (currently unused)
videos/full/*.mp4                full-length versions with audio (Projects page player)
```

Upload the local `videos/` folder to a Bunny Storage Zone with the **same folder structure**, then point the `videos/...` paths in the three HTML files at the Bunny CDN (Pull Zone) URL.

Poster images (`videos/posters/*.jpg`) are small and live in this repository.

## Libraries (loaded from CDNs)

- three.js r128 (home intro rock field)
- GSAP 3.12.5 + ScrollTrigger (parallax)
- Lenis 1.1.13 (smooth scrolling)
- Familjen Grotesk (Google Fonts)
