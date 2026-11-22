# 📄 Birds of Ohio: A Backyard Field Guide

## 🎯 Overview

Build a four-page field guide to five backyard birds of Ohio, with responsive photos, a
captioned video, and recordings of each bird's song.

Most birders hear a bird long before they see it, so a good field guide needs more than
pictures. In this assignment you build a small multi-page site that uses every kind of media
covered so far: images served in modern formats at the right size, a video with captions,
and audio with a written description for visitors who can't listen.

The layout is mobile-first: one stacked column with a header, navigation, main content, and
footer. You won't use Flexbox or Grid yet. Everything is built with the HTML and CSS from
Weeks 4–6.

### 🧠 What You'll Practice

By completing this assignment, you will practice how to:

- Link several pages together with shared navigation and mark the current page with a
  `current` class
- Serve images in AVIF, WebP, and JPEG with `picture` and `source`
- Let the browser pick an image size with `srcset` and `sizes`
- Prevent layout shift with `width` and `height`, and defer offscreen images with
  `loading="lazy"`
- Write useful `alt` text, and know when an image should have an empty `alt=""`
- Embed video with `video`, multiple `source` formats, a `poster`, and a WebVTT captions
  `track`
- Embed a YouTube video with an `iframe` and a descriptive `title`
- Embed audio with `audio` and multiple `source` formats, with a fallback link and a text
  description
- Credit photos, video, and recordings with their license
- Keep media inside its column with `max-width: 100%`, and keep an embedded video at 16:9 with
  `aspect-ratio`

## 📋 Requirements

Your site must have these four pages in the root folder, each with the same header,
navigation, and footer:

| Page | What it contains |
| --- | --- |
| `index.html` | A full-width hero image, an intro paragraph, links to the other three pages, and a "Meet the Birds" list that links to each bird on the Songs page |
| `photos.html` | One photo card per bird (five total), each a `figure` with a `figcaption` and a photo credit |
| `video.html` | A captioned video of a Northern Cardinal in a `figure`, an embedded YouTube video in a second `figure`, plus a short "What to Watch For" section |
| `songs.html` | One card per bird with an `id`, a "Listen for" line, an audio player, a written description, and a recording credit |

### Every page

- [ ] Valid HTML5 with `lang="en"`, `charset`, `viewport`, a unique `title`, and a
      `meta name="description"`
- [ ] Links to the Google Fonts (Bitter and Source Sans 3) and to `css/styles.css`
- [ ] A `header` with the logo and site name (linking to `index.html`), a tagline, and a
      `nav` list linking to all four pages
- [ ] The current page's nav link has `class="current"`
- [ ] One `h1`, with `h2`s for sections
- [ ] A `footer` with the state bird fact, a media credit note, and a copyright line

### Images

- [ ] Every photo uses a `picture` element with AVIF and WebP `source`s and a JPEG `img`
      fallback
- [ ] Every format lists a small and a large file in `srcset` with `w` descriptors, plus
      `sizes`
- [ ] Every `img` has `width` and `height`
- [ ] Photos on `photos.html` use `loading="lazy"`. The hero on the home page does not.
- [ ] Every photo has descriptive `alt` text. The decorative logo next to the site name has
      `alt=""`.

### Video

- [ ] A `video` element with `controls`, `preload="metadata"`, a `poster`, `width`, and
      `height`
- [ ] WebM and MP4 `source`s, in that order
- [ ] A captions `track` that loads `video/cardinal-captions.vtt`, with `srclang`, `label`,
      and `default`
- [ ] A fallback paragraph with a download link
- [ ] A YouTube video embedded with an `iframe` in a `figure`, with a descriptive `title`,
      `width`, `height`, `loading="lazy"`, and `allowfullscreen`, plus a `figcaption` and credit

### Audio

- [ ] Each of the five birds has an `audio` element with `controls` and `preload="none"`
- [ ] OGG, M4A (`type="audio/mp4"`), and MP3 `source`s, in that order
- [ ] A fallback paragraph with a download link
- [ ] A written "What you'll hear" description for each recording
- [ ] Each card's `id` matches the bird's link on the home page (for example,
      `songs.html#carolina-wren`)

### CSS

- [ ] One shared stylesheet, `css/styles.css`, used by every page
- [ ] Images and video never overflow their column (`max-width: 100%; height: auto`), the
      YouTube `iframe` fills the column at 16:9 (`width: 100%; aspect-ratio: 16 / 9`), and
      audio players fill the column width
- [ ] Media is grouped into cards with a shared `.card` style
- [ ] Credits use a shared `.credit` style
- [ ] No Flexbox or Grid

### ✅ Before You Submit

- [ ] All four pages open from the navigation on every page, and the current page is marked
- [ ] Every photo loads, and your browser's dev tools show it picked an AVIF or WebP file
- [ ] The video plays, and captions show when you turn on **CC**
- [ ] The YouTube video plays and fits the column at phone width
- [ ] All five recordings play
- [ ] The "Meet the Birds" links on the home page jump to the right card on the Songs page
- [ ] Nothing overflows the page at phone width
- [ ] Every page passes the [W3C Markup Validation Service](https://validator.w3.org/)
- [ ] File names are lowercase with no spaces, and they match your `src` paths exactly
- [ ] The site is live on GitHub Pages, every media file works there, and the URL is in your
      pull request

## 🖼️ Example Output

When you're done, open `index.html` in a browser and click through every page. Resize the
window to phone width: the hero should bleed to the screen edges, and every photo, video, and
audio player should stay inside the single column.

## 📂 Starter Files

| File / Folder | Purpose |
| --- | --- |
| `index.html` | Home page: hero, intro, and links to each bird |
| `photos.html` | Photos of the five birds |
| `video.html` | Captioned Northern Cardinal video |
| `songs.html` | Song recordings with descriptions |
| `css/styles.css` | The shared stylesheet for every page |
| `images/logo.svg` | The site logo |
| `images/hero*.{avif,webp,jpg}` | The home page hero, at 800 and 1600 pixels wide |
| `images/<bird>*.{avif,webp,jpg}` | One photo per bird, at 600 (`-small`) and 1200 pixels wide |
| `video/cardinal.{webm,mp4}` | The cardinal video in two formats |
| `video/cardinal-poster.jpg` | The image shown before the video plays |
| `video/cardinal-captions.vtt` | The video's WebVTT captions |
| `audio/<bird>.{ogg,m4a,mp3}` | Each bird's song in three formats |

The five birds are `northern-cardinal`, `carolina-wren`, `american-robin`, `blue-jay`, and
`red-winged-blackbird`. Use those names in every file path and `id`.

> [!NOTE]
> The photos, video, and recordings are placeholders. Their credits read "placeholder"
> until licensed media replaces them.

## 🧮 Grading

| Criteria | Full credit looks like | Points |
| --- | --- | --- |
| **Page structure & navigation** | Four valid pages with a matching header, nav, and footer, a unique `title` and description, and the `current` class on the current link | 5 |
| **Responsive images** | Every photo uses `picture` with AVIF, WebP, and JPEG, a `srcset` with two sizes, `sizes`, `width`/`height`, and lazy loading where required | 6 |
| **Alt text & credits** | Descriptive `alt` on every photo, `alt=""` on the decorative logo, and a credit on every photo, video, and recording | 3 |
| **Video** | Plays with controls, a poster, WebM and MP4 sources, working captions, and a fallback link; the YouTube `iframe` plays and has a descriptive `title` | 4 |
| **Audio** | All five birds play with OGG, M4A, and MP3 sources, a fallback link, a written description, and a working `id` link from the home page | 4 |
| **CSS** | One shared stylesheet; media stays inside the column; shared `.card` and `.credit` styles; no Flexbox or Grid | 2 |
| **Published and submitted** | Live on GitHub Pages with working media, and the pull request is filled in and submitted in Canvas | 1 |
| | **Total** | **25** |

## 📚 Resources

- [MDN — Responsive images](https://developer.mozilla.org/en-US/docs/Web/HTML/Guides/Responsive_images)
- [MDN — `<picture>`: The Picture element](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/picture)
- [MDN — Video and audio content](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Structuring_content/HTML_video_and_audio)
- [MDN — `<iframe>`: The Inline Frame element](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/iframe)
- [MDN — `<track>`: The Embed Text Track element](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/track)
- [MDN — WebVTT format](https://developer.mozilla.org/en-US/docs/Web/API/WebVTT_API/Web_Video_Text_Tracks_Format)
- [W3C — Alt decision tree](https://www.w3.org/WAI/tutorials/images/decision-tree/)
- [W3C Markup Validation Service](https://validator.w3.org/)

## 🆘 Getting Help

Ask during class or office hours, or post on the Canvas discussion board.

Before you ask, check these common problems:

- **A photo or media file doesn't load on GitHub Pages but works locally?** GitHub Pages is
  case-sensitive. `Blue-Jay.jpg` won't find `blue-jay.jpg`.
- **Captions don't show?** Check the `track` path, and test from a local server or GitHub
  Pages. Some browsers block `.vtt` files opened straight from your hard drive.
- **The browser always loads the JPEG?** Make sure the `source`s come *before* the `img`
  inside `picture`, and that each `type` is spelled `image/avif` or `image/webp`.
- **A "Meet the Birds" link goes to the top of the Songs page?** The part after `#` must
  match the card's `id` exactly.
- **An image is wider than the screen?** Check that `img, video { max-width: 100%; height: auto; }`
  is in your stylesheet.

---

The AI policy and submission instructions are in the [README](../README.md).
