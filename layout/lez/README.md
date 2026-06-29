# Lezgi keyboard
 
System keyboard layout for the **Lezgi language** (Лезги чӏал · Lezgi · ISO&nbsp;639: `lez` · Cyrillic script) for **iOS, iPadOS and macOS**.
 
The layout is built on top of the standard **Russian** system keyboard. The goal is zero relearning for people already used to the Russian layout: no familiar key is moved from its place.
 
## 📘 Highlights
 
- **Palochka `Ӏ` / `ӏ`** (U+04C0 / U+04CF) takes the position of `щ`. Case is preserved: lowercase `ӏ` on the base layer, uppercase `Ӏ` on Shift.
- **`щ`** (used only in loanwords) is available via **long-press on `ш`** on touch keyboards.
- **`ъ`** is promoted to a dedicated key — it is frequent in Lezgi (гъ, къ, хъ, etc.). On iPhone it is added to the top row; on iPad and macOS it is a normal key, as in Russian.
- System keys (Return, Space, Search, etc.) are **localized into Lezgi** (`keyNames`).
- Fully position-compatible with the Russian layout across all form factors.

## 📱 Existing implementation

In addition to this proposed native system layout, we have already built and published a custom Lezgi keyboard for iOS:

- **GitHub:** https://github.com/LekiTech/LezgiKeyboard-ios
- **App Store:** https://apps.apple.com/us/app/id6444746265

This existing implementation demonstrates practical demand for Lezgi input support on iOS and provides a working reference for the proposed native keyboard layout.

## 🧩 Files
 
```
layout/lez/
 ├── lez-3-rows.yaml      # primary iOS/iPadOS layout (iPhone + iPad-9in + iPad-12in)
 ├── lez-longpress.yaml   # long-press alternates
 └── lez-macos.yaml       # macOS layout (hardware keyboard)
```
 
## ⌨️ Long-press alternates
 
The following Lezgi-specific long-press alternates are defined in `lez-longpress.yaml` and differ from the default Russian layout:
 
- **Letters:** 
  - `ш → щ` 
  - `ц → цӏ`
  - `у → уь`
  - `к → кь къ кӏ`
  - `г → гь гъ`
  - `х → хь хъ`
  - `ч → чӏ`
  - `т → тӏ`
- **Symbols & punctuation:** currencies on `₽`, `№` on `#`, ellipsis on `.`, quote and dash variants, and more.

## 🌍 Compatibility
 
The layouts follow the repository's unified scheme and are compatible with platform layout-generation tools (Apple Keyboard, Unicode CLDR, etc.).
 
## 📝 Notes
 
On **macOS**, the letter `щ` is not present in the Lezgi layout because hardware keyboard layouts do not support touch-style long-press alternates. Users who frequently type Russian loanwords containing `щ` can switch to the Russian layout when needed.

## 👥 Contact
 
Authors: E. Eskendarov, R. Gamidov, A. Magomedov, K. Tadzjibov. 

Prepared for the *Apple Keyboards for All* project.
