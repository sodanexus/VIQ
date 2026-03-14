# VIQ — Official Website

> Site officiel de **VIQ**, artiste de musique électronique et indie basé à Paris. Conçu comme une expérience visuelle minimaliste et immersive.
>
> 🌐 [viqmusic.net](https://www.viqmusic.net)

---

## ✨ Concept

Le site repose sur une seule page (`index.html`) — pas de framework, pas de build. Une vidéo en fond plein écran, une typographie monumentale, et des tiroirs animés qui révèlent les liens à la demande. L'interface s'efface au profit de l'atmosphère.

---

## 🏗️ Structure

```
/
├── index.html              ← Page principale (standalone)
├── 404.html                ← Page d'erreur custom
├── Background.mp4          ← Vidéo de fond
├── favicon.png
├── cover.jpg               ← Visuel principal
├── og-image.jpg            ← Image Open Graph (1260×630)
├── viq-press-kit.zip       ← Press kit téléchargeable
├── llms.txt                ← Fiche artiste pour LLMs / IA
├── sitemap.xml
└── robots.txt
```

---

## 🎨 Design & interactions

- **Fond vidéo** plein écran (`object-fit: cover`), silencieux, en boucle
- **Typographie** : Playfair Display — majuscules, taille fluide (`clamp`)
- **Navigation par tiroirs** : chaque section (Listen, Reach, Bio) s'ouvre avec une animation séquentielle entrée/sortie (`translateY`)
- **Effet de vague SVG** (`feTurbulence` + `feDisplacementMap`) animé au clic sur les boutons actifs
- **Transitions de page** : fondu noir (sortie vers une release) / fondu blanc (sortie vers le shop)
- **Entrance fade** : fondu noir au chargement initial
- **Hover** : décalage horizontal (`translateX`) + opacité réduite sur les autres liens

---

## 📋 Sections

| Bouton | Contenu |
|---|---|
| **OUT NOW** | Lien direct vers la dernière release |
| **LISTEN** | Spotify, Apple Music, Tidal, Deezer, Amazon, YouTube, Pandora, Bandcamp, SoundCloud |
| **REACH** | TikTok, Threads, Facebook, Instagram + Press Kit + Contact |
| **WEAR** | Boutique merch (Fourthwall — `merch.viqmusic.net`) |
| **BIO** | Biographie complète en anglais |

---

## 🛠️ Stack technique

| Élément | Détail |
|---|---|
| **Frontend** | HTML / CSS / JS vanilla — zéro dépendance |
| **Typographie** | Google Fonts (Playfair Display) |
| **Animations** | CSS `@keyframes` + SVG Filter (`feTurbulence`) |
| **Vidéo** | `<video>` natif (autoplay, muted, loop) |
| **SEO** | Meta OG, Twitter Card, Schema.org `MusicGroup`, canonical |
| **Analytics** | [Umami](https://umami.is/) |
| **Email** | Obfuscation Cloudflare (`email-decode`) |
| **Merch** | [Fourthwall](https://fourthwall.com) |

---

## 🔍 SEO & découvrabilité

- Données structurées **Schema.org** (`MusicGroup`) avec genres, liens plateformes et membre
- Balises **Open Graph** et **Twitter Card** complètes
- Balise `canonical` vers `https://www.viqmusic.net/`
- `robots: index, follow` + `sitemap.xml`
- **`llms.txt`** — fiche artiste structurée pour les moteurs IA (ChatGPT, Perplexity, etc.)

---

## 🎵 Artiste

- **Labels** : Stratford.Ct, Lofi Girl
- **Genres** : Synthwave · Dreampop · Indie Electronic · Chillwave · Atmospheric
- **Actif depuis** : 2019
- **Notable** : Featured sur Lofi Girl, EDM.com, KALTBLUT Magazine, Stereofox, Nightride FM · Collaborations industrie du jeu vidéo · Sorties physiques (vinyle, cassette)

---

## ⚠️ Note

Le contenu de ce repo (vidéo, visuels, textes, musique) est protégé par le droit d'auteur et reste la propriété exclusive de VIQ. La licence ci-dessous s'applique uniquement au **code source**.
