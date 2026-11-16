# 💻 Birds of Ohio: A Backyard Field Guide

A four-page field guide to five backyard birds of Ohio, built for Web Design I. It uses
responsive photos in AVIF, WebP, and JPEG, a captioned video, and recordings of each bird's
song, all in a mobile-first single-column layout.

This repo also includes the editor and Git configuration and the pull request template that every
assignment in this course uses.

> [!NOTE]
> `.editorconfig`, `.gitattributes`, `.gitignore`, `.noai`, and the `.github` and `.idea`
> folders are setup files that keep assignments consistent. Leave them alone. The four HTML
> pages and the `css`, `images`, `video`, and `audio` folders are the site.

## 📋 Assignment Requirements

> [!IMPORTANT]
> **Start here: [read ASSIGNMENT.md →](.github/ASSIGNMENT.md)**

It has the overview, the requirements for each page, a final checklist, and the grading rubric. Read it before you start, and check it again before you submit.

## ✅ At a Glance

Every assignment follows the same steps. Each guide has screenshots for every step.

| Step | What you do                                                                | Guide                                         |
|------|----------------------------------------------------------------------------|-----------------------------------------------|
| 0    | **First assignment only:** install and set up WebStorm                     | [WebStorm Setup](.github/WEBSTORM_SETUP.md)   |
| 1    | Create your repo from this template, clone it, and make a `develop` branch | [Getting Started](.github/GETTING_STARTED.md) |
| 2    | Build your pages in the root folder                                        | [Where Your Files Go](#-where-your-files-go)  |
| 3    | Commit and push often, then turn on GitHub Pages                           | [Publishing](.github/PUBLISHING.md)           |
| 4    | Open a pull request into `main` and submit its URL in Canvas               | [Submitting](.github/SUBMITTING.md)           |

## 📂 Where Your Files Go

Create your files in the **root folder** of this repo — the same folder as this README.
GitHub Pages publishes from the root, so `index.html` has to live there or your site will 404.
The pages sit in the root, and the media is grouped into subfolders:

```
index.html
photos.html
video.html
songs.html
css/styles.css
images/logo.svg
images/hero.jpg, hero-small.jpg (plus .avif and .webp)
images/<bird>.jpg, <bird>-small.jpg (plus .avif and .webp)
video/cardinal.webm
video/cardinal.mp4
video/cardinal-poster.jpg
video/cardinal-captions.vtt
audio/<bird>.ogg
audio/<bird>.m4a
audio/<bird>.mp3
```

`<bird>` is one of `northern-cardinal`, `carolina-wren`, `american-robin`, `blue-jay`, or
`red-winged-blackbird`. Your `src` and `srcset` paths need the folder name, like
`images/blue-jay.jpg` or `audio/blue-jay.mp3`. File names are lowercase with no spaces.

## 🤖 AI Policy

Work on this assignment must be your own. Do not use AI coding assistants — including
GitHub Copilot, Cursor, ChatGPT, Claude, or JetBrains AI Assistant — to generate,
complete, or rewrite your code.

You should be able to explain any line of your submission. You may be asked to do so.

This repo includes a `.noai` file, which disables JetBrains AI Assistant for the project
in IDEs like WebStorm. Leave it in place. It is a reminder of the policy above, not a
substitute for it — following the policy is still your responsibility.

> [!NOTE]
> The `.noai` file does **not** turn off WebStorm's local Full Line code completion. Turn that
> off yourself as part of the [one-time setup](.github/WEBSTORM_SETUP.md) (step 5).

> [!CAUTION]
> Late or missing submissions are graded on what is in the pull request at the deadline, so push your final commits
> before you submit.
