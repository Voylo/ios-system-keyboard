# **Tatar (tat) native iOS/macOS keyboards.**

## Tatar iOS

There are 3 variants: tat-3-rows (primary), tat-3-rows-rus, and tat-4-rows.

3 rows layout is the national Tatar layout. Tatar letters (Ә, Ө, Ү, Җ, Ң, Һ) have dedicated keys, while the displaced Russian letters (Ц, Щ, Ж, Ё, Ъ) are accessible via longpress on related keys (Ө, Ә, Ң, Е, Ь).

The Russian-based version (tat-3-rows-rus) keeps the standard Russian layout, extended with dedicated Ү, Ә, Ң keys; all Tatar letters are also accessible via longpress on related Russian letters (У → Ү, О → Ө, Н → Ң, Х → Һ, А → Ә, Ж → Җ).

4 rows keyboard is an additional version for people who don't like to longpress letters. It features a dedicated top row for Tatar letters (ә, ө, ү, җ, ң, һ) plus ё and ъ, while its 2-4 rows are exactly the same as the standard Russian keyboard – so it can be called `Tatar based on Russian`.

Bashkir letters Ҡ and Ғ are additionally available via longpress on К and Г.

Versions sorting for iPhone:
* tat-3-rows.yaml
* tat-3-rows-rus.yaml
* tat-4-rows.yaml

For iPad there are 2 versions: the national one (tat-3-rows, also reused by tat-4-rows) and the Russian-based one (tat-3-rows-rus), because there is enough space to put all Tatar letters in both.

## Tatar macOS

There are two macOS variants:
* tat-macos.yaml (Apple-style) – standard Russian ЙЦУКЕН layout; Tatar letters are accessible via `Option` (aka `ALT`).
* tat-macos-pc.yaml (PC-style) – the national Tatar layout known from Windows PCs; the displaced Russian letters (Ц, Щ, Ж, Ё, Ъ, Ь) are accessible via `Option`.

## Tatar keyNames

System buttons are localized into Tatar in `keynames-tat.yaml` using common system button labels, shared by all layout variants.
