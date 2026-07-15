# 🌍 Tobíkova a Timčina mapa světa

Interaktivní mapa světa s hrami na procvičování vlajek a hlavních měst.

## Co umí

- **🔎 Objevuj** – najetím myši na stát se vykreslí jeho vlajka, zobrazí se hlavní město na mapě i jeho název. Kliknutím se stát přiblíží.
- **🚩 Hádej vlajku** – zobrazí se vlajka a hledá se země na mapě (3 pokusy, nápověda kontinentu).
- **🏙️ Najdi zemi města** – zobrazí se hlavní město a kliká se na správnou zemi.
- **✏️ Napiš hlavní město** – zvýrazní se země a píše se název hlavního města (funguje i bez diakritiky a toleruje drobný překlep).
- **Zoom a centrování** – kolečko myši, tlačítka +/− a rychlé přiblížení na kontinenty (Evropa, Asie, Afrika, Severní i Jižní Amerika, Austrálie a Oceánie).
- **Přepínač podkladu** – 🎨 barevný atlas (kontinenty odlišené barvami) nebo 🛰️ satelitní snímek Země (NASA Blue Marble).
- **Skóre** – body (3/2/1 podle počtu pokusů), série správných odpovědí a rekord se ukládají v prohlížeči.

## Jak spustit

Web potřebuje připojení k internetu (mapová data a vlajky se načítají z CDN).

**Lokálně:** stačí otevřít `index.html` v prohlížeči.

**Na GitHub Pages:**

1. Vytvoř nový repozitář na github.com (např. `mapa-sveta`).
2. Nahraj do něj soubory `index.html`, `data.js` a `README.md` (Add file → Upload files).
3. V repozitáři otevři **Settings → Pages**, v sekci *Build and deployment* zvol Source: **Deploy from a branch**, větev `main`, složku `/ (root)` a ulož.
4. Za minutu bude web na `https://<tvoje-jmeno>.github.io/mapa-sveta/`.

## Technika

- [D3.js](https://d3js.org/) + [world-atlas](https://github.com/topojson/world-atlas) (hranice zemí, rozlišení 1:50m)
- Vlajky: [flagcdn.com](https://flagcdn.com/)
- Satelitní podklad: NASA Blue Marble (Wikimedia Commons)
- Česká data 196 zemí + závislých území: `data.js` (názvy, hlavní města, souřadnice, kontinenty)
- Somaliland je zobrazen samostatně jako mezinárodně neuznaný stát (vlastní vlajka a hlavní město Hargeysa, ve hrách se neobjevuje); ostatní sporná území (Severní Kypr…) se zobrazují jako součást mezinárodně uznaných států
