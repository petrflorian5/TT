# 🚀 Tobíkův a Timčin koutek

Vzdělávací web pro děti — mapa světa, matematika, písmenka, hodiny a angličtina. Vše česky, hravé a bez reklam.

## Sekce

- **🌍 Mapa světa** (`mapa.html`) — interaktivní mapa: najetím na stát vlajka a hlavní město, hádání vlajek a hlavních měst, zoom na kontinenty, přepínač barevný atlas / satelit (NASA).
- **🧮 Matematika** (`matematika.html`) — Timča: počítání obrázků, větší–menší, sčítání a odčítání do 10; Tobík: sčítání/odčítání do 100 (i tři čísla), násobení (řada × čísla do 100), dělení beze zbytku a velký mix.
- **🔤 Písmenka a slova** (`pismenka.html`) — první písmeno podle obrázku, slabiky, skládání slov, čtení s porozuměním. Slovníček 60 slov.
- **🕐 Hodiny** (`hodiny.html`) — čtení času z ručiček (24h formát) a nastavování ručiček podle digitálního času.
- **🇬🇧 Angličtina** (`anglictina.html`) — Timča: barvy, čísla, zvířata s poslechem; Tobík: poslech, překlady oběma směry, psaní slovíček a jednoduché věty. Výslovnost = skutečné nahrávky rodilých mluvčích (Wikislovník).

Ve všech hrách se sbírají ⭐ hvězdy a 🔥 série, ukládají se v prohlížeči.

## Spuštění

Web potřebuje internet (mapová data, vlajky, nahrávky výslovnosti z CDN). Lokálně stačí otevřít `index.html`. Na GitHub Pages: Settings → Pages → Deploy from a branch → `main` / root.

## Technika

- Mapa: [D3.js](https://d3js.org/) + [world-atlas](https://github.com/topojson/world-atlas) (1:50m), vlajky [flagcdn.com](https://flagcdn.com/), satelit NASA Blue Marble + GIBS dlaždice
- Výslovnost: nahrávky z Wikimedia Commons (anglický Wikislovník), záložně Web Speech API
- Česká data zemí: `data.js`; Somaliland zobrazen jako neuznaný stát, sporná území jako součást uznaných států
- Bez frameworků a bez sledování — jen HTML, CSS a JavaScript
