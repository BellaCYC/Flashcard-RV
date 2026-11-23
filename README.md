# Flashcard RV

Try it: bellacyc.github.io/Flashcard-RV/

A simple, dark-mode flashcard app inspired by Knowt and Quizlet, built for personal practice (not commercial). One self-contained `index.html` — no build step, no server, with an independent account to save progress.

N0 ADS

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

## Accounts & cloud sync

- **Sign up / Log in** with a username (or an email, if you want "Forgot password?" to work) and a password of at least 6 characters.
- Sets, stars, progress and settings are saved to the signed-in user's account in **Firebase (Cloud Firestore)**, so the same account shows the same cards in every browser and on every device. Clearing browser data doesn't delete them.
- Firestore security rules (`firestore.rules`) only let each user read and write their own data.
- **Export all** downloads a `.json` backup; **Import** loads it back.

## Run it

Visit the GitHub Pages site for this repo.
