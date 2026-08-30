# Násobilka s Lulu a Oskarem

Webová appka na trénink malé násobilky (1×1 až 10×10) pro děti na prvním stupni.

Není postavená na správnosti, ale na **reakčním čase**: správná odpověď za šest vteřin
znamená, že si ji dítě dopočítalo, ne že si ji vybavilo. Limit je proto pět vteřin
na všech úrovních — na dopočítání není čas.

## Jak to funguje

- **55 příkladů, ne sto.** Díky komutativitě je 7 × 8 a 8 × 7 jeden fakt. Devatenáct
  z nich jsou jedničky a desítky, takže skutečného učiva je 36.
- **Tři úrovně obtížnosti** pro každý příklad zvlášť: vybrat z možností → najít výsledek
  v tabulce → napsat ho. Zelené políčko v mapě se získává až za třetí úroveň.
- **Spaced repetition** podle Leitnerových boxů, s odstupy uvnitř relace i mezi dny.
- **Nejvýš šest příkladů v učení současně.** Nové se přidávají, až když je předchozí
  zvládnutý.
- **Pevný konec relace.** První kolo dne 40 příkladů, druhé 20, další 10 — ochrana proti
  přesycení.
- Nikdy červené křížky ani odečítání bodů. Po chybě se ukáže správná odpověď, přečte se
  nahlas a jede se dál.

## Spuštění

Jeden soubor bez jediné externí závislosti — žádné skripty, fonty ani CDN. Stačí otevřít
`index.html` v prohlížeči, funguje i offline. Postup se ukládá do `localStorage`
daného zařízení.

Na iPadu a iPhonu doporučuji **Sdílet → Přidat na plochu**: Safari maže uložená data
webům, se kterými se týden neinteragovalo, a aplikace spuštěná z ikony tomu podléhá míň.
V nastavení je navíc tlačítko na zálohu a obnovu postupu.

## Testy

Otevřete stránku s `#testy` v adrese — spustí se sada testů čisté logiky
(distraktory, výběr dalšího příkladu, postupová logika, dávkování, načtení
poškozeného stavu).

## Ladění

Konfigurační blok `K` na začátku souboru obsahuje všechny laditelné hodnoty:
časové limity, délky relací, prahy postupu, odstupy opakování.
