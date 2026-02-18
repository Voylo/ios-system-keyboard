# Avar (ava) native iOS/macOS keyboards

## Avar iOS

There is 1 default layout: ava-4-rows.

The 4-row layout places all Avar letters directly on the primary layer without letter replacement.

Long-press is used for stress marks and secondary symbols.

Versions sorting for iPhone:
* ava-4-rows.yaml

For iPad keyboard versions there is only 1 version, because there is enough space to place all Avar letters.

## Avar macOS

All 33 Avar letters (including ӏ) are placed directly on the primary layer using standard ANSI geometry.

No letter replacement is used.

Stress marks are available via dead keys.

The Option (ALT) layer contains extended system symbols, similar to other macOS Cyrillic layouts.


## Avar keyNames

Key names are translated into Avar using natural interface phrasing.

### Stress marks

Stress marks (combining acute accent U+0301) are optional and used primarily for educational and disambiguation purposes.

They should be ignored during:
 • autocorrection
 • search
 • tokenization
 • frequency analysis

#### Recommended preprocessing:

Unicode NFD normalization followed by removal of combining marks.
