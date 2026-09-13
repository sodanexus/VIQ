# VIQ — Site officiel

> Site officiel de VIQ, artiste de musique électronique et indie basé à Paris. Une expérience visuelle minimaliste et immersive — une seule page, zéro framework, zéro build.
>
> 🌐 [viqmusic.net](https://www.viqmusic.net)

![HTML/JS](https://img.shields.io/badge/stack-HTML%20%2F%20JS%20vanilla-black) ![GitHub Pages](https://img.shields.io/badge/hébergement-GitHub%20Pages-black) ![Umami](https://img.shields.io/badge/analytics-Umami-222222) ![Fourthwall](https://img.shields.io/badge/merch-Fourthwall-FF6B35)

---

## 🎧 Écouter

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

**Dernière sortie →** [go.viqmusic.net/stn](https://go.viqmusic.net/stn)

## 📡 Suivre

[![Instagram](https://img.shields.io/badge/Instagram-E4405F?logo=instagram&logoColor=white)](https://www.instagram.com/viqmusic/)
[![TikTok](https://img.shields.io/badge/TikTok-000000?logo=tiktok&logoColor=white)](https://www.tiktok.com/@viqmusic)
[![Threads](https://img.shields.io/badge/Threads-000000?logo=threads&logoColor=white)](https://www.threads.com/@viqmusic)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?logo=facebook&logoColor=white)](https://www.facebook.com/Viqmusic)

**Merch →** [merch.viqmusic.net](https://merch.viqmusic.net/) · **Press kit →** [viq-press-kit.zip](./viq-press-kit.zip) · **Contact →** [contact@viqmusic.net](mailto:contact@viqmusic.net)

---

## Concept

Une image en fond plein écran, une typographie monumentale, et des tiroirs animés qui révèlent les liens à la demande. L'interface s'efface au profit de l'atmosphère. Tout tient dans un seul fichier `index.html`.

---

## Structure du projet

```
VIQ/
├── index.html              # Toute l'app — HTML + CSS + JS
├── 404.html                # Page d'erreur custom
├── fond.jpg                # Visuel de fond plein écran
├── og-image.jpg            # Image Open Graph (1260×630)
├── favicon.png
├── viq-press-kit.zip       # Press kit téléchargeable
├── llms.txt                # Fiche artiste pour LLMs (ChatGPT, Perplexity…)
├── sitemap.xml
├── robots.txt
└── CNAME                   # viqmusic.net
```

---

## Sections

| Bouton | Contenu |
|---|---|
| **OUT NOW** | Lien direct vers la dernière release |
| **LISTEN** | Spotify · Apple Music · Tidal · Deezer · Qobuz · Amazon · YouTube · Pandora · Bandcamp · SoundCloud |
| **REACH** | TikTok · Threads · Facebook · Instagram · Press Kit · Contact |
| **WEAR** | Boutique merch (Fourthwall — `merch.viqmusic.net`) |
| **BIO** | Biographie complète en anglais |

---

## Design & interactions

- **Fond image** plein écran (`object-fit: cover`)
- **Overlay d'assombrissement** au survol/ouverture des tiroirs Listen, Reach et Bio, pour la lisibilité
- **Typographie** Playfair Display — majuscules, taille fluide (`clamp`)
- **Tiroirs animés** — chaque section s'ouvre avec une animation séquentielle (`translateY`) et se ferme proprement
- **Effet de vague SVG** (`feTurbulence` + `feDisplacementMap`) animé en `requestAnimationFrame` au clic sur les boutons actifs
- **Hover links** — décalage horizontal (`translateX`) + opacité réduite sur les autres liens dans le tiroir
- **Transitions de page** — fondu noir vers une release · fondu blanc vers le shop
- **Entrance fade** — fondu noir au chargement initial

---

## Stack technique

| Élément | Détail |
|---|---|
| Frontend | HTML + CSS + JS vanilla — zéro dépendance |
| Typographie | Google Fonts — Playfair Display |
| Animations | CSS `@keyframes` + SVG Filter (`feTurbulence`) + `requestAnimationFrame` |
| Analytics | [Umami](https://umami.is/) (privacy-first, sans cookies) |
| Email | Obfuscation Cloudflare (`email-decode`) |
| Merch | [Fourthwall](https://fourthwall.com) |
| Hébergement | GitHub Pages + CNAME `viqmusic.net` |

---

## SEO & découvrabilité

- Données structurées **Schema.org** (`MusicGroup`) avec genres, liens plateformes et membres
- Balises **Open Graph** et **Twitter Card** complètes
- Balise `canonical` → `https://www.viqmusic.net/`
- `robots: index, follow` + `sitemap.xml`
- **`llms.txt`** — fiche artiste structurée pour les moteurs IA (ChatGPT, Perplexity, etc.)

---

## Artiste

| | |
|---|---|
| **Nom** | VIQ (Julien Pannetier) |
| **Basé à** | Paris, France |
| **Actif depuis** | 2019 |
| **Labels** | Stratford.Ct · Lofi Girl |
| **Genres** | Synthwave · Dreampop · Indie Electronic · Chillwave · Atmospheric |
| **Influences** | Lorn · Justice · Daft Punk · Mk.gee |
| **Plateformes** | Spotify · Apple Music · Tidal · Deezer · Qobuz · Amazon · YouTube · Bandcamp · SoundCloud |
| **Notable** | Featured sur Lofi Girl, EDM.com, KALTBLUT Magazine, Stereofox, Nightride FM, Roblox · Sorties physiques vinyl & cassette |

---

## Note légale

Le contenu de ce repo (visuels, textes, musique) est protégé par le droit d'auteur et reste la propriété exclusive de VIQ. La licence associée s'applique uniquement au **code source**.
