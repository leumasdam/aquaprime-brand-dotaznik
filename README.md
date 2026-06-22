# AQUAPRIME — Brand Discovery

Klikací dotazník, ktorý vyplníš (alebo pošleš klientovi) **pred tvorbou loga**. Z odpovedí sa stavia smer, osobnosť a vizuál značky AQUAPRIME.

Čistý statický web (1 súbor `index.html` + fonty) — žiadny build, žiadny backend. Ideálne pre GitHub Pages.

## Vizuál
Zenko štýl 1:1 — krémový papier `#f3eee3`, warm gold `#b0804f`, Satoshi + JetBrains Mono, hairline linky, mono eyebrowy.

## Ako to funguje
- Jedna otázka = jedna obrazovka (klikačka feeling), progress bar hore.
- Typy: text, dlhý text, single-choice (auto-posun), multi-choice, chips, sémantické škály (osobnosť značky), kontakt.
- Na konci **Zhrnutie** → *Odoslať e-mailom* (mailto), *Kopírovať*, *Stiahnuť .txt*.
- Žiadne dáta neodchádzajú, kým ich respondent sám neodošle.

## Úpravy
Všetky otázky sú v jednom poli `QUESTIONS` v `index.html`. Pridať/zmeniť otázku = jeden riadok objektu. E-mail pre odoslanie: konštanta `OWNER_EMAIL`.

## Deploy na GitHub Pages
```bash
git remote add origin https://github.com/leumasdam/aquaprime-brand-dotaznik.git
git push -u origin main
# Settings → Pages → Branch: main / root → Save
```
Live: `https://leumasdam.github.io/aquaprime-brand-dotaznik/`

## Lokálne
Otvor `index.html` v prehliadači (fonty sa načítajú relatívne). Alebo `npx serve .`
