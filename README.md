# Vatsal Gandhi — Portfolio

A single-file, zero-build portfolio styled as a clinical monitoring display — a nod to the ICU mortality-prediction research it showcases. Dark ink background, cyan/amber monitor palette, animated ECG hero trace, Syne + IBM Plex type system. Fully responsive, respects `prefers-reduced-motion`.

## Deploy to GitHub Pages (5 minutes)

1. Create a new repo named **`Vats10987.github.io`** (using your GitHub username makes it your root site).
2. Push this folder:
   ```bash
   cd portfolio
   git init
   git add .
   git commit -m "Launch portfolio"
   git branch -M main
   git remote add origin https://github.com/Vats10987/Vats10987.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Source: Deploy from a branch → main / root → Save**.
4. Your site goes live at **https://vats10987.github.io** within a minute or two.

## Iterating with Claude Code

Open this folder in Claude Code and use prompts like:

> "This is my portfolio site (index.html). Keep the clinical-monitor design system — ink background, cyan #4FD6C6 traces, amber #FFB454 alerts, Syne display font, IBM Plex Mono for data labels. Add a [new section / dark-light toggle / project detail page] consistent with that system."

Design tokens live at the top of the `<style>` block in `:root` — change colors and fonts in one place.

## Structure

- `index.html` — everything: markup, styles, and the ECG canvas animation. No build step, no dependencies beyond Google Fonts.
