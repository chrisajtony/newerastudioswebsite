# New Era Studios Website

Static website for New Era Studios: an AI-native creative studio for series slates and brand campaigns.

## Pages

| File | Page |
|---|---|
| `index.html` | Home: scroll intro, portfolio panels, services, clients, process, signals, footer |
| `work.html` | Projects index: filterable grid, full-length video player |
| `contact.html` | Contact page |

No build step. Open `index.html` in a browser or serve the folder with any static host.

## Videos (hosted on Bunny Stream)

All videos stream from Bunny Stream library `715659` via its CDN host
`https://vz-382c5475-4dd.b-cdn.net/<video-id>/play_<720|1080>p.mp4`.

- Full-screen backgrounds and the full-length player use `play_1080p.mp4`.
- Grid and Signals tiles use `play_720p.mp4`.
- Poster images (`videos/posters/*.jpg`) live in this repository.

**Allowed domains:** the Bunny library blocks requests from unlisted websites (403).
Add every domain the site runs on (e.g. `newerastudioswebsite.vercel.app` and any custom domain)
under Bunny → Stream → library → Security → Allowed Domains.

## Libraries (loaded from CDNs)

- three.js r128 (home intro rock field)
- GSAP 3.12.5 + ScrollTrigger (parallax)
- Lenis 1.1.13 (smooth scrolling)
- Familjen Grotesk (Google Fonts)
