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
* `bua-rus-ext-3-rows.yaml` — Russian-based extended (dedicated Ө Ү Һ keys)

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

### 3. Russian-based extended (`bua-rus-ext`) — iOS only

The Russian ЙЦУКЕН layout with the Buryat letters `Ө Ү Һ` as **dedicated keys**
next to their look-alikes, following the Bashkir (`bak`) approach of 12 keys per row:

* `ү` right after `у` (top row, 12 keys)
* `ө` right after `о` (middle row, 12 keys)
* `һ` between `т` and `ь` (bottom row, same position as in the Mongolian-based layout)

Rationale: `ү`, `ө` and especially `һ` are high-frequency letters in Buryat
(vowel harmony, suffixes like *-һаа, -үүд, -өөр, -гүй*), so hiding them behind
long-press slows typing noticeably. This variant keeps the familiar Russian
arrangement — no relearning — while frequent Buryat letters are one tap away.
Rare letters moved to long-press: `ё` (on `е`), `ъ` (on `ь`).

iOS only: on hardware keyboards (macOS) the number of physical keys is fixed,
so the `⌥`-based `bua-rus-macos.yaml` already covers this use case.

Files: `bua-rus-ext-3-rows.yaml` (iOS), `bua-rus-ext-longpress.yaml`.

The alphabet has 36 letters: 33 Russian + 3 Buryat-specific (Ө, Ү, Һ).

## Developer

* Али Кужугет / Ali Kuzhuget
* Булат Дамдинов / Bulat Damdinov

## References

- [Buryat language — Wikipedia](https://en.wikipedia.org/wiki/Buryat_language)
- [Бурятский язык — Википедия](https://ru.wikipedia.org/wiki/Бурятский_язык)
