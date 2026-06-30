# Abkhaz (abk) native iOS/macOS keyboards

## Language

Abkhaz (Аԥсшәа / Аԥсуа бызшәа) is a Northwest Caucasian language spoken by the Abkhaz people,
primarily in Abkhazia on the eastern coast of the Black Sea. It is known for one of the world's
richest consonant inventories, written today in a modified Cyrillic alphabet of ~64 letters
(~38 graphically distinct; the rest are digraphs formed with ⟨ь⟩ palatalization and ⟨ә⟩ labialization).

Self-name:
**Аԥсшәа**

Language codes:
- ISO 639-1: `ab`
- ISO 639-2: `abk`
- ISO 639-3: `abk`

## Abkhaz iOS

- `abk-3-rows.yaml` — primary layout. The on-screen arrangement mirrors **Gboard Android's Abkhaz
  keyboard**: the Russian ЙЦУКЕН base with seven Abkhaz letters promoted onto the visible layer
  (`ҵ ӡ ҟ ҽ ә џ ҩ`, replacing the unused `й щ э я ю`).
- `abk-4-rows.yaml` — dense variant that surfaces most Abkhaz-specific letters directly on the
  visible layer, minimizing reliance on long-press.

## Abkhaz macOS

- `abk-macos.yaml` — physical keyboard. Keeps the familiar Russian ЙЦУКЕН skeleton on the visible
  layer with the core Abkhaz letters substituted in; the remaining letters are on the Option layer.

## Long-press and Abkhaz-specific forms

Letters not on the visible layer are reached through parent-key long-press:

- `г → ӷ ҕ`  (modern descender ӷ first, legacy ҕ second)
- `к → қ`    (ҟ is on the visible layer)
- `п → ԥ ҧ`  (modern ԥ first, traditional ҧ second)
- `т → ҭ`
- `х → ҳ`
- `ч → ҷ`
- `ҽ → ҿ`   (ҽ is on the visible layer; its descender form ҿ is the long-press alternate)
- `е → ё`    (for Russian text)

Digraphs (`гь`, `гә`, `кь`, `кә`, …) are produced by typing the base letter followed by `ь` or `ә`,
so no dedicated digraph keys are required.

### Encoding notes

The 1996 orthographic reform standardized the descender variant **ӷ** (U+04F7) over **ҕ** (U+0495)
for the voiced uvular position; the modern pe-with-descender **ԥ** (U+0525) is used in preference to
the legacy **ҧ** (U+04A7). Both legacy forms remain available on long-press for compatibility.
