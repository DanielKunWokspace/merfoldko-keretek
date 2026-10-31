# Mérföldkő Keret – keretbolt

Ebből a tárolóból tölti le az app a kereteket.

- `frames.json` – a keretek listája (név, felirat, kategória 3 nyelven, ingyenes vagy prémium)
- `*.png` – a keretképek (a fotó helye átlátszó)

Új keret: töltsd fel a PNG-t, és vegyél fel egy új elemet a `frames.json`-ba.
Kép cseréje: töltsd fel ugyanazzal a névvel, és a `version` számot növeld eggyel.
Keret elrejtése: `"active": false`.
- `thumbs/*.webp` – kis előnézeti képek a listához (360 px széles). Az app induláskor csak ezeket tölti le,
  a nagy PNG-t csak akkor, amikor valaki kiválasztja a keretet.

Új keretnél a `thumb` sort is add meg (pl. `"thumb": "thumbs/uj_keret.webp"`). Ha kimarad, az app a nagy képet tölti le a listához.
