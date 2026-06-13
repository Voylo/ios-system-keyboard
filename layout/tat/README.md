# Tatar (tat) native iOS/macOS keyboards

## Language

Tatar (Volga Tatar) is a Kipchak Turkic language spoken by about 10 million people, primarily in the Republic of Tatarstan and across the Volga–Ural region, as well as by Tatar communities worldwide.

Self-name: **Татар теле / Татарча**

Language codes:
- ISO 639-1: `tt`
- ISO 639-2: `tat`
- ISO 639-3: `tat`

## Alphabet

`а ә б в г д е ё ж җ з и й к л м н ң о ө п р с т у ү ф х һ ц ч ш щ ъ ы ь э ю я`

39 letters: the 33 Russian letters plus 6 Tatar letters `ә ө ү җ ң һ`.

**Mainly in Russian loanwords**: `ё ц щ ъ`

## Tatar iOS

There are 2 variants: tat-3-rows (primary) and tat-4-rows.

Versions sorting for iPhone (the primary `tat-3-rows` sorts first; `tat-4-rows` follows):
* tat-3-rows.yaml
* tat-4-rows.yaml

#### Татарча — national layout

`tat-3-rows.yaml`

```
й ө у к е н г ш ә з х ү
ф ы в а п р о л д ң э һ
я ч с м и т җ ь б ю
```

3 rows layout is the national Tatar layout. Tatar letters (Ә, Ө, Ү, Җ, Ң, Һ) have dedicated keys, while the displaced Russian letters (Ц, Щ, Ж, Ё, Ъ) are accessible via longpress on related keys (Ө, Ә, Ң, Е, Ь).

#### Татарча (4 рәт) — 4 rows

`tat-4-rows.yaml`

```
! ё һ ө ә җ ң ү ъ , .
й ц у к е н г ш щ з х
ф ы в а п р о л д ж э
я ч с м и т ь б ю
```

4 rows keyboard is an additional version for people who don't like to longpress letters. It features a dedicated top row for Tatar letters (ә, ө, ү, җ, ң, һ) plus ё and ъ, while its 2-4 rows are exactly the same as the standard Russian keyboard – so it can be called `Tatar based on Russian`.

Siberian Tatar letters Ҡ and Ғ are additionally available via longpress on К and Г in all variants.

Each variant has its own iPad layers. The national (tat-3-rows) version uses the standard 3-row iPad design, because there is enough space to put all Tatar letters. The 4-rows version keeps its dedicated Tatar letter row on iPad as well: 4 letter rows on 9–11″ iPads and 5 rows (including the number row) on 12.9″ iPads. Thanks to that, its longpress set (`tat-4-rows-longpress.yaml`) stays minimal — only Ҡ, Ғ and the common symbol longpresses — since all Tatar letters and the displaced Russian letters have dedicated keys on every layout.

## Tatar macOS

`tat-macos.yaml` — the national Tatar layout known from Windows PCs. Tatar letters Ә, Ө, Ү, Ң, Җ, Һ have dedicated keys; the displaced Russian letters (Ц, Щ, Ж, Ё, Ъ, Ь) are accessible via `Option` (aka `ALT`).

```
] 1 2 3 4 5 6 7 8 9 0 - =
  й ө у к е н г ш ә з х ү һ
  ф ы в а п р о л д ң э
  я ч с м и т җ б ю /
```

## Tatar keyNames

System buttons are localized into Tatar in `tat-keynames.yaml` using common system button labels, shared by all layout variants.

## References

* The national 3-row layout follows the Tatar national keyboard standard familiar from Windows PCs.
* Longpress pairings are based on letter similarity and frequency; letter frequency can be cross-checked against the Tatar National Corpus «Туган тел».

## Layout Developers' Contact Information

* Marat – https://github.com/m4rr
