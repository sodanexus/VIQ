# VIQ — Site officiel

> Site officiel de VIQ, artiste de musique électronique et indie basé à Paris. Une expérience visuelle minimaliste et immersive — une seule page, zéro framework, zéro build.
>
> 🌐 [viqmusic.net](https://www.viqmusic.net)

![HTML/JS](https://img.shields.io/badge/stack-HTML%20%2F%20JS%20vanilla-black) ![GitHub Pages](https://img.shields.io/badge/hébergement-GitHub%20Pages-black) ![Umami](https://img.shields.io/badge/analytics-Umami-222222) ![Fourthwall](https://img.shields.io/badge/merch-Fourthwall-FF6B35)

---

## Concept

Une vidéo en fond plein écran, une typographie monumentale, et des tiroirs animés qui révèlent les liens à la demande. L'interface s'efface au profit de l'atmosphère. Tout tient dans un seul fichier `index.html`.

---

## Structure du projet

```
VIQ/
├── index.html              # Toute l'app — HTML + CSS + JS
├── 404.html                # Page d'erreur custom
├── Background.mp4          # Vidéo de fond plein écran
├── cover.jpg               # Visuel principal
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
| **LISTEN** | Spotify · Apple Music · Tidal · Deezer · Amazon · YouTube · Pandora · Bandcamp · SoundCloud |
| **REACH** | TikTok · Threads · Facebook · Instagram · Press Kit · Contact |
| **WEAR** | Boutique merch (Fourthwall — `merch.viqmusic.net`) |
| **BIO** | Biographie complète en anglais |

---

## Design & interactions

- **Fond vidéo** plein écran (`object-fit: cover`), silencieux, en boucle — relancé au premier touch sur mobile
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
| Vidéo | `<video>` natif (autoplay, muted, loop, playsinline) |
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
| **Plateformes** | Spotify · Apple Music · Tidal · Deezer · Amazon · YouTube · Bandcamp · SoundCloud |
| **Notable** | Featured sur Lofi Girl, EDM.com, KALTBLUT Magazine, Stereofox, Nightride FM, Roblox · Sorties physiques vinyl & cassette |

---

## Note légale

Le contenu de ce repo (vidéo, visuels, textes, musique) est protégé par le droit d'auteur et reste la propriété exclusive de VIQ. La licence associée s'applique uniquement au **code source**.
