# Buryat language (Буряад хэлэн) — `bua`

Keyboard layout for the **Buryat language** (ISO 639-3: `bua`), Mongolic language family.

**Language codes**:

* **ISO 639-3**: `bua`
* **ISO 15924**: `Cyrl`

## Layouts

Two layouts, each for iOS and macOS.
The order in the list is the sort order — **the first layout is the default one.**

Versions sorting for iPhone:
* `bua-3-rows.yaml` — Mongolian-based (default)
* `bua-rus-3-rows.yaml` — Russian-based

Versions sorting for macOS:
* `bua-macos.yaml` — Mongolian-based (default)
* `bua-rus-macos.yaml` — Russian-based

### 1. Mongolian-based — default

The letter arrangement follows the national Mongolian keyboard
(Windows KBDMON / MNS standard): `ө` on the `F` key, `ү` on `O`, `е`/`щ` on `-`/`=`.
`Һ` is added for Buryat.

On both platforms this is the main Buryat layout, named simply **"Buryat"**
(the Russian-based variant is marked as "(Russian)").

* **macOS** — `Һ` on the `\` key; the number row follows the Mongolian pattern: without `Shift` — punctuation and `₽` (ruble instead of the Mongolian tugrik), digits via `Shift`.
* **iOS** — `Һ` in the bottom row between `Т` and `Ь`; `щ`/`ъ` via long-press (`ш → щ`, `ь → ъ`).

Files: `bua-3-rows.yaml` (iOS), `bua-macos.yaml` (macOS), `bua-longpress.yaml`.

Source of the Mongolian layout: <https://learn.microsoft.com/globalization/keyboards/kbdmon>

### 2. Russian-based (`bua-rus`)

The full Russian ЙЦУКЕН layout without changes — all Russian letters stay in place.
The Buryat letters `Ө Ү Һ` are typed on the look-alike Russian keys:

* **iOS** — long-press: `у → ү`, `о → ө`, `х → һ`
* **macOS** — Option (⌥): `⌥у → ү`, `⌥о → ө`, `⌥х → һ` (uppercase via `⌥⇧`)

Files: `bua-rus-3-rows.yaml` (iOS), `bua-rus-macos.yaml` (macOS), `bua-rus-longpress.yaml`.

The alphabet has 36 letters: 33 Russian + 3 Buryat-specific (Ө, Ү, Һ).

## Developer

* Али Кужугет / Ali Kuzhuget
* Булат Дамдинов / Bulat Damdinov

## References

- [Buryat language — Wikipedia](https://en.wikipedia.org/wiki/Buryat_language)
- [Бурятский язык — Википедия](https://ru.wikipedia.org/wiki/Бурятский_язык)
