<div align="center">

# VIQ — My Official Artist Website

This is my official website as VIQ, an electronic and indie music artist based in Paris. A minimal, immersive visual experience — single page, zero framework, zero build — that I designed and built myself.

🌐 [viqmusic.net](https://www.viqmusic.net)

![HTML/JS](https://img.shields.io/badge/stack-HTML%20%2F%20JS%20vanilla-black) ![GitHub Pages](https://img.shields.io/badge/hosting-GitHub%20Pages-black) ![Umami](https://img.shields.io/badge/analytics-Umami-222222) ![Fourthwall](https://img.shields.io/badge/merch-Fourthwall-FF6B35)

</div>

---

<div align="center">

## 🎧 Listen

[![Spotify](https://img.shields.io/badge/Spotify-1ED760?logo=spotify&logoColor=white)](https://open.spotify.com/artist/6XpN8mRlhuOXuvEyva4yjZ)
[![Apple Music](https://img.shields.io/badge/Apple%20Music-FA243C?logo=applemusic&logoColor=white)](https://music.apple.com/us/artist/viq/1467177415)
[![Tidal](https://img.shields.io/badge/Tidal-000000?logo=tidal&logoColor=white)](https://tidal.com/artist/14851275)
[![Deezer](https://img.shields.io/badge/Deezer-FEAA2D?logo=deezer&logoColor=black)](https://www.deezer.com/fr/artist/53988822)
[![Bandcamp](https://img.shields.io/badge/Bandcamp-408294?logo=bandcamp&logoColor=white)](https://viqmusic.bandcamp.com/music)
[![SoundCloud](https://img.shields.io/badge/SoundCloud-FF5500?logo=soundcloud&logoColor=white)](https://soundcloud.com/viqmusic)

**Latest release →** [go.viqmusic.net/stn](https://go.viqmusic.net/stn)

## 📡 Follow

[![Instagram](https://img.shields.io/badge/Instagram-E4405F?logo=instagram&logoColor=white)](https://www.instagram.com/viqmusic/)
[![TikTok](https://img.shields.io/badge/TikTok-000000?logo=tiktok&logoColor=white)](https://www.tiktok.com/@viqmusic)

**Merch →** [merch.viqmusic.net](https://merch.viqmusic.net/) · **Press kit →** [viq-press-kit.zip](./viq-press-kit.zip) · **Contact →** [contact@viqmusic.net](mailto:contact@viqmusic.net)

</div>

---

## Concept

A full-screen photograph and monumental typography set in `mix-blend-mode: difference`: the words invert the colors of the image beneath them, so the menu becomes part of the picture. Drawers reveal links on demand, and the BIO section adds a portrait. Everything lives in a single `index.html` file.

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
- **Monumental menu** — five lowercase words in Archivo Expanded ExtraBold, always on a single line, auto-scaled to never overflow
- **Cursor lens** — a white disc, also in `difference`, that grows over links (desktop only)
- **Photo drift & grain** — the background follows the pointer with a slight parallax, under an animated film-grain overlay
- **Drawers** — LISTEN, REACH and BIO open below the menu; items appear in sequence, hover dims the siblings, Esc closes
- **BIO reveal** — soft graded shade over the backdrop, portrait revealed on the side (desktop) or above the text (mobile)
- **Sound design** — ambient SoundCloud loop on click, plus soft synthesized electric-piano chords for opening/closing drawers
- **Transitions** — black curtain entrance, black fade to a release, white fade to the shop

---

## Tech stack

HTML + CSS + JS vanilla, zero dependencies · Google Fonts (Archivo variable) · Umami analytics (cookieless) · Fourthwall for merch · hosted on GitHub Pages.

Also handles the basics for discoverability: Schema.org structured data, Open Graph / Twitter Card tags, sitemap, and an `llms.txt` fact sheet for AI engines.

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

The content of this repo (visuals, text, music) is protected by copyright and remains my exclusive property as VIQ. The associated license applies to the **source code** only.
