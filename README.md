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

A full-screen photograph and monumental typography set in `mix-blend-mode: difference`: the words invert the colors of the image beneath them, so the menu becomes part of the picture. Drawers reveal links on demand, and the BIO section adds a portrait. Everything lives in a single `index.html` file.

---

## Project structure

```
VIQ/
├── index.html              # The whole app — HTML + CSS + JS
├── 404.html                # Custom error page
├── fond.jpg                # Full-screen background visual (3840×3248)
├── profil.jpg              # Portrait shown in the BIO section (1193×1800)
├── og-image.jpg            # Open Graph image (1260×630)
├── favicon.png             # Square 512×512, transparent
├── apple-touch-icon.png    # 180×180 on the night colour (iOS home screen)
├── viq-press-kit.zip       # Downloadable press kit
├── llms.txt                # Artist fact sheet for LLMs (ChatGPT, Perplexity…)
├── sitemap.xml
├── robots.txt
└── CNAME                   # www.viqmusic.net
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

- **Difference blending** — the whole UI layer uses `mix-blend-mode: difference`, so type inverts the photo underneath (teal ↔ orange, dark → white)
- **Monumental menu** — five lowercase words in Archivo Expanded ExtraBold, always on a single line. A small script (`fit()`) scales the menu down if a word would ever overflow the screen (narrow phones, slow font loading)
- **Cursor lens** — a white disc, also in `difference`, that grows over links (desktop only)
- **Photo drift** — the background follows the pointer with a slight parallax; **film grain** overlay (animated SVG noise)
- **Drawers** — LISTEN, REACH and BIO open below the menu, which shrinks to make room; items appear in sequence, hover dims the siblings, Esc closes
- **BIO** — the photo stays as the backdrop under a soft graded shade (dark on the text side, opening toward the portrait; no blur). The portrait is revealed on the right (desktop) or above the text with a dark gradient (mobile)
- **Footer row** — coordinates + `©VIQ <current year>` (the year updates itself) and the sound button share one axis (desktop: bottom-right; mobile: coordinates bottom-left, button bottom-right), both in `difference`
- **Ambient sound** — SoundCloud widget loaded on first click of the bottom-right button, looped, 35 % volume
- **Page transitions** — black fade to a release · white fade to the shop
- **Entrance** — black curtain lifting, then the words rise one after the other
- `prefers-reduced-motion` is respected (no grain animation, no drift, no reveal)

---

## Tech stack

| Item | Detail |
|---|---|
| Frontend | HTML + CSS + JS vanilla — zero dependencies |
| Typography | Google Fonts — Archivo (variable: width + weight axes) |
| Animations | CSS transitions / `@keyframes` + SVG noise (`feTurbulence`) + `requestAnimationFrame` |
| Analytics | [Umami](https://umami.is/) (privacy-first, cookieless) |
| Email | Cloudflare obfuscation (`email-decode`) |
| Merch | [Fourthwall](https://fourthwall.com) |
| Hosting | GitHub Pages + CNAME `viqmusic.net` |

---

## SEO & discoverability

- **Schema.org** structured data (`WebSite` + `MusicGroup` in one `@graph`) with genres, image, founding date, member and all platform links (`sameAs`)
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
