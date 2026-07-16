# Náš výlet – Białka Tatrzańska (web)

Hotový web s průvodcem na výlet **22.–24. 7. 2026** (Adámek & Karin).

## Co je ve složce

- **`index.html`** — celý web (průvodce)
- **`manifest.json`** — nastavení pro „appku na plochu" telefonu
- **`icon-180.png`, `icon-192.png`, `icon-512.png`** — ikona (hory + srdíčko), co se zobrazí na ploše telefonu
- **`README.md`** — tenhle návod

**Všechny soubory musí zůstat pohromadě v jedné složce** a `index.html` se nesmí přejmenovat.
Otevřít lokálně: dvojklik na `index.html`.

---

## 1) Jak to dostat online přes Vercel

Web musí být online (mít odkaz), aby šel přidat na plochu telefonu. Vyber si jeden způsob:

### Varianta A — Vercel CLI (nejrychlejší, bez GitHubu)
1. Nainstaluj **Node.js** z nodejs.org (verze „LTS").
2. Otevři terminál a nainstaluj Vercel:
   ```
   npm i -g vercel
   ```
3. Přejdi do téhle složky, např.:
   ```
   cd Plocha/bialka-web
   ```
4. Spusť:
   ```
   vercel
   ```
5. Přihlásí tě, párkrát potvrdíš Enter (výchozí volby stačí) a **dostaneš živý odkaz** typu `https://nas-vylet.vercel.app`.

Když web upravíš, spusť znovu `vercel --prod`.

### Varianta B — přes GitHub (doporučeno pro trvalý web)
1. Založ účet na **github.com**, vytvoř nový repozitář (např. `nas-vylet`).
2. Nahraj do něj **všechny soubory z téhle složky** (Add file → Upload files → přetáhni → Commit).
3. Jdi na **vercel.com**, přihlas se přes GitHub.
4. **Add New… → Project → Import** ten repozitář, dej **Deploy**.
5. Za pár vteřin máš odkaz `https://nas-vylet.vercel.app`.

### Nejjednodušší alternativa (bez Vercelu)
Jdi na **app.netlify.com/drop**, přetáhni celou složku a hned máš živý odkaz.

---

## 2) Přidání na plochu telefonu (appka s ikonou)

Když je web online, přidáš si ho na plochu jako normální aplikaci — žádné programování navíc, iPhone i Android to umí sami. Ikona (hory + srdíčko) a název „Náš výlet" jsou už nastavené v souborech.

**iPhone (Safari):**
1. Otevři odkaz webu v **Safari**.
2. Ťukni na tlačítko **Sdílet** (čtvereček se šipkou dole).
3. Vyber **Přidat na plochu**.
4. Potvrď — na ploše se objeví ikona „Náš výlet". Otevře se na celou obrazovku jako appka.

**Android (Chrome):**
1. Otevři odkaz v **Chromu**.
2. Menu (tři tečky) → **Přidat na plochu / Nainstalovat aplikaci**.
3. Potvrď.

> Tip: musí to být přes ten **online odkaz** (vercel.app), ne přes soubor v počítači.

---

## 3) Vlastní doména (nepovinné)

Zdarma dostaneš `neco.vercel.app`. Když budeš chtít vlastní adresu (např. `nasvylet.cz`),
kup si doménu (Wedos, Forpsi…) a ve Vercelu ji připojíš v **Settings → Domains**.

---

*Ceny a otevírací doby jsou z oficiálních zdrojů (léto 2026). Pár dní před výletem si je pro jistotu ověř —
lanovky, hrady a půjčovny mění sezónní ceníky, počasí zkontroluj na yr.no / meteo.pl.*
