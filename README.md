# My Flashcards

A simple, dark-mode flashcard app inspired by Knowt and Quizlet, built for personal practice (not commercial). One self-contained `index.html` — no build step, no server, no account.

## Features

- **Create sets** – term / definition cards, Tab/Enter to jump to the next field, reorder, delete, swap terms and definitions
- **Bulk import** – paste lists separated by tab, comma, dash or a custom separator (works with Quizlet/Knowt exports)
- **Accent keys** – `¡ ¿ ° á é í ñ ó ú ü` + ⇧ for capitals; customizable per set
- **Flashcards** – flip with Space, ← still learning / → know, shuffle, stars, undo
- **Learn** – rounds of 7: multiple choice → written → mastered
- **Test** – true/false, multiple choice and written questions with a scored review
- **Match** – timed tile game with personal best

## Smart grading

| Rule | Example |
|---|---|
| Accents count (toggle) | `marroqui` → accent mistake, missing letter highlighted |
| Small typos forgiven | `morocan` ✓ for *Moroccan* (1 letter ≤7 chars, 2 for longer) |
| Any alternative accepted | `francesa` ✓ for *francés / francesa*; both in any order ✓ |
| Articles (toggle) | `pasaporte` for *el pasaporte* → "check the article" |
| Always ignored | case, extra spaces, `¡! ¿? . , ;`; text in (parentheses) is optional |

Wrong answers can always be overridden with **I was correct**.

## Storage

Sets, stars and progress are saved in your browser (`localStorage`). Use **Export all** to download a `.json` backup and **Import** to restore it on another device or browser.

## Run it

Open `index.html` in any browser, or visit the GitHub Pages site for this repo.
