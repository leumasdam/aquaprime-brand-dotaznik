# AQUAPRIME — Brand Discovery

Klikací dotazník, ktorý vyplníš (alebo pošleš klientovi) **pred tvorbou loga**. Z odpovedí sa stavia smer, osobnosť a vizuál značky AQUAPRIME.

Čistý statický web (1 súbor `index.html` + fonty) — žiadny build, žiadny backend. Ideálne pre GitHub Pages.

## Vizuál
**zenko.sk 1:1** (zdroj `portfolio-v2`) — biela + zinc sivá, **Outfit** + JetBrains Mono, veľké zaoblené karty, čierne pill CTA, zeleno-teal akcenty (`#0c4b3a` / `#8dc63f` / `#20827c`). Plus reálne zenko prvky: **logo** (brandmark + slash + „Zenko"), **konštrukčný grid** v pozadí (odkrýva sa okolo kurzora) a **živý maskot** (oči sledujú kurzor, žmurká, fúzy). Brand assety v `assets/brand/`.

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
