# VIQ — Official Website

> Official website of VIQ, an electronic and indie music artist based in Paris. A minimal, immersive visual experience — single page, zero framework, zero build.
>
> 🌐 [viqmusic.net](https://www.viqmusic.net)

![HTML/JS](https://img.shields.io/badge/stack-HTML%20%2F%20JS%20vanilla-black) ![GitHub Pages](https://img.shields.io/badge/hosting-GitHub%20Pages-black) ![Umami](https://img.shields.io/badge/analytics-Umami-222222) ![Fourthwall](https://img.shields.io/badge/merch-Fourthwall-FF6B35)

---

## 🎧 Listen

[![Spotify](https://img.shields.io/badge/Spotify-1ED760?logo=spotify&logoColor=white)](https://open.spotify.com/artist/6XpN8mRlhuOXuvEyva4yjZ)
[![Apple Music](https://img.shields.io/badge/Apple%20Music-FA243C?logo=applemusic&logoColor=white)](https://music.apple.com/us/artist/viq/1467177415)
[![Tidal](https://img.shields.io/badge/Tidal-000000?logo=tidal&logoColor=white)](https://tidal.com/artist/14851275)
[![Deezer](https://img.shields.io/badge/Deezer-FEAA2D?logo=deezer&logoColor=black)](https://www.deezer.com/fr/artist/53988822)
[![Qobuz](https://img.shields.io/badge/Qobuz-000000?logoColor=white)](https://play.qobuz.com/artist/5200555)
[![Amazon Music](https://img.shields.io/badge/Amazon%20Music-00A8E1?logo=amazonmusic&logoColor=white)](https://music.amazon.fr/artists/B07SVHSJ37/viq)
[![YouTube Music](https://img.shields.io/badge/YouTube%20Music-FF0000?logo=youtubemusic&logoColor=white)](https://music.youtube.com/@VIQmusic)
[![Pandora](https://img.shields.io/badge/Pandora-224099?logoColor=white)](https://www.pandora.com/artist/viq/AR7v5wJfcr9gkKX)
[![Bandcamp](https://img.shields.io/badge/Bandcamp-408294?logo=bandcamp&logoColor=white)](https://viqmusic.bandcamp.com/music)
[![SoundCloud](https://img.shields.io/badge/SoundCloud-FF5500?logo=soundcloud&logoColor=white)](https://soundcloud.com/viqmusic)

**Latest release →** [go.viqmusic.net/stn](https://go.viqmusic.net/stn)

## 📡 Follow

[![Instagram](https://img.shields.io/badge/Instagram-E4405F?logo=instagram&logoColor=white)](https://www.instagram.com/viqmusic/)
[![TikTok](https://img.shields.io/badge/TikTok-000000?logo=tiktok&logoColor=white)](https://www.tiktok.com/@viqmusic)
[![Threads](https://img.shields.io/badge/Threads-000000?logo=threads&logoColor=white)](https://www.threads.com/@viqmusic)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?logo=facebook&logoColor=white)](https://www.facebook.com/Viqmusic)

**Merch →** [merch.viqmusic.net](https://merch.viqmusic.net/) · **Press kit →** [viq-press-kit.zip](./viq-press-kit.zip) · **Contact →** [contact@viqmusic.net](mailto:contact@viqmusic.net)

---

## Concept

A full-screen background image, monumental typography, and animated drawers that reveal links on demand. The interface fades away in favor of the atmosphere. Everything lives in a single `index.html` file.

---

## Project structure

```
VIQ/
├── index.html              # The whole app — HTML + CSS + JS
├── 404.html                # Custom error page
├── fond.jpg                # Full-screen background visual
├── og-image.jpg            # Open Graph image (1260×630)
├── favicon.png
├── viq-press-kit.zip       # Downloadable press kit
├── llms.txt                # Artist fact sheet for LLMs (ChatGPT, Perplexity…)
├── sitemap.xml
├── robots.txt
└── CNAME                   # viqmusic.net
```

---

## Sections

| Button | Content |
|---|---|
| **OUT NOW** | Direct link to the latest release |
| **LISTEN** | Spotify · Apple Music · Tidal · Deezer · Qobuz · Amazon · YouTube · Pandora · Bandcamp · SoundCloud |
| **REACH** | TikTok · Threads · Facebook · Instagram · Press Kit · Contact |
| **WEAR** | Merch store (Fourthwall — `merch.viqmusic.net`) |
| **BIO** | Full biography (English) |

---

## Design & interactions

- **Full-screen background image** (`object-fit: cover`)
- **Dim overlay** on hover/open of the Listen, Reach and Bio drawers, for readability
- **Typography** Playfair Display — uppercase, fluid sizing (`clamp`)
- **Animated drawers** — each section opens with a sequential animation (`translateY`) and closes cleanly
- **SVG wave effect** (`feTurbulence` + `feDisplacementMap`) animated with `requestAnimationFrame` on active button clicks
- **Hover links** — horizontal shift (`translateX`) + reduced opacity on the other links in the drawer
- **Page transitions** — black fade to a release · white fade to the shop
- **Entrance fade** — black fade on initial load

---

## Tech stack

| Item | Detail |
|---|---|
| Frontend | HTML + CSS + JS vanilla — zero dependencies |
| Typography | Google Fonts — Playfair Display |
| Animations | CSS `@keyframes` + SVG Filter (`feTurbulence`) + `requestAnimationFrame` |
| Analytics | [Umami](https://umami.is/) (privacy-first, cookieless) |
| Email | Cloudflare obfuscation (`email-decode`) |
| Merch | [Fourthwall](https://fourthwall.com) |
| Hosting | GitHub Pages + CNAME `viqmusic.net` |

---

## SEO & discoverability

- **Schema.org** structured data (`MusicGroup`) with genres, platform links and members
- Full **Open Graph** and **Twitter Card** tags
- `canonical` tag → `https://www.viqmusic.net/`
- `robots: index, follow` + `sitemap.xml`
- **`llms.txt`** — structured artist fact sheet for AI engines (ChatGPT, Perplexity, etc.)

---

## Artist

| | |
|---|---|
| **Name** | VIQ (Julien Pannetier) |
| **Based in** | Paris, France |
| **Active since** | 2019 |
| **Labels** | Stratford.Ct · Lofi Girl |
| **Genres** | Synthwave · Dreampop · Indie Electronic · Chillwave · Atmospheric |
| **Influences** | Lorn · Justice · Daft Punk · Mk.gee |
| **Platforms** | Spotify · Apple Music · Tidal · Deezer · Qobuz · Amazon · YouTube · Bandcamp · SoundCloud |
| **Notable** | Featured on Lofi Girl, EDM.com, KALTBLUT Magazine, Stereofox, Nightride FM, Roblox · Physical releases on vinyl & cassette |

---

## Legal notice

The content of this repo (visuals, text, music) is protected by copyright and remains the exclusive property of VIQ. The associated license applies to the **source code** only.
