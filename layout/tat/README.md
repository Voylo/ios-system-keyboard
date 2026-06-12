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

There are 3 variants: tat-3-rows (primary), tat-3-rows-rus, and tat-4-rows.

Versions sorting for iPhone (enforced via `order:` fields in the YAML files):
* tat-3-rows.yaml
* tat-3-rows-rus.yaml
* tat-4-rows.yaml

#### Татарча — national layout

`tat-3-rows.yaml`

```
й ө у к е н г ш ә з х ү
ф ы в а п р о л д ң э һ
я ч с м и т җ ь б ю
```

3 rows layout is the national Tatar layout. Tatar letters (Ә, Ө, Ү, Җ, Ң, Һ) have dedicated keys, while the displaced Russian letters (Ц, Щ, Ж, Ё, Ъ) are accessible via longpress on related keys (Ө, Ә, Ң, Е, Ь).

#### Татарча (урыс) — Russian-based layout

`tat-3-rows-rus.yaml`

```
й ц у к е н г ш щ з х ү
ф ы в а п р о л д ж э ә
я ч с м и т ь б ю ң
```

The Russian-based version keeps the standard Russian layout, extended with dedicated Ү, Ә, Ң keys; all Tatar letters are also accessible via longpress on related Russian letters (У → Ү, О → Ө, Н → Ң, Х → Һ, А → Ә, Ж → Җ).

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

For iPad there are 2 versions: the national one (tat-3-rows, also reused by tat-4-rows) and the Russian-based one (tat-3-rows-rus), because there is enough space to put all Tatar letters in both. The 4-rows variant uses its own longpress set (`tat-4-rows-longpress.yaml`) that combines the Russian-based mappings with Ө → Ц, Ә → Щ, Ң → Ж, so the displaced Russian letters stay reachable on the national iPad layers.

## Tatar macOS

There are two macOS variants:

#### Татарча — Apple-style

`tat-macos.yaml` – standard Russian ЙЦУКЕН layout; Tatar letters are accessible via `Option` (aka `ALT`).

```
] 1 2 3 4 5 6 7 8 9 0 - =
  й ц у к е н г ш щ з х ъ ё
  ф ы в а п р о л д ж э
  я ч с м и т ь б ю .
```

#### Татарча (ПК) — PC-style

`tat-macos-pc.yaml` – the national Tatar layout known from Windows PCs; the displaced Russian letters (Ц, Щ, Ж, Ё, Ъ, Ь) are accessible via `Option`.

```
] 1 2 3 4 5 6 7 8 9 0 - =
  й ө у к е н г ш ә з х ү һ
  ф ы в а п р о л д ң э
  я ч с м и т җ б ю .
```

## Tatar keyNames

System buttons are localized into Tatar in `keynames-tat.yaml` using common system button labels, shared by all layout variants.

## References

* The national 3-row layout follows the Tatar national keyboard standard familiar from Windows PCs.
* Longpress pairings are based on letter similarity and frequency; letter frequency can be cross-checked against the Tatar National Corpus «Туган тел».

## Layout Developers' Contact Information

* Marat – https://github.com/m4rr
