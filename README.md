# CLVC landing page

Vstupní stránka pro školení **Claude AI – Vibe Coding a tvorba aplikací bez programování (CLVC)**. Je to jeden samostatný soubor `index.html` (HTML + CSS + vanilla JS), takže funguje bez jakéhokoli build kroku.

## Publikace na GitHub Pages

1. Vytvořte na GitHubu nový repozitář (např. `clvc-landing`).
2. Do repozitáře nahrajte soubor `index.html` (musí být v kořeni repozitáře nebo ve složce `/docs`).
   ```bash
   git init
   git add index.html README.md
   git commit -m "Landing page pro školení CLVC"
   git branch -M main
   git remote add origin https://github.com/<vas-ucet>/clvc-landing.git
   git push -u origin main
   ```
3. V nastavení repozitáře na GitHubu jděte do **Settings → Pages**.
4. U "Build and deployment" zvolte **Deploy from a branch**, větev `main` a složku `/ (root)`.
5. Uložte — GitHub vygeneruje adresu typu `https://<vas-ucet>.github.io/clvc-landing/`.

Případně lze totéž udělat příkazem `gh repo create` a `gh` CLI, pokud jej máte nainstalovaný.

## Úprava obsahu

Všechny texty (termíny, ceny, kontakt) jsou přímo v `index.html`. Countdown v sekci "Nejbližší termín" počítá k datu `2026-10-26T09:00:00` — při změně termínu upravte proměnnou `target` ve `<script>` na konci souboru.
