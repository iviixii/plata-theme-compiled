<img src=".gitlab/logo_thumb_small.png" alt="Logo" align="left" width="85" height="85"/>

### Plata-theme

This is just a precompiled Gtk+ Plata theme based on Material Design Refresh.

All credit goes to tista500 amazing work!

You can find the repo at the following gitlab:
https://gitlab.com/tista500/plata-theme

----------------------------------------------

Typography
----------

Plata strongly depends on Material Design resources, especially its **fonts**.

 1. [**Roboto**](https://fonts.google.com/specimen/Roboto)
   - Very famous as the default truetype font in Android (English ver.).
   - Multilingual support is not good.
   - Weight used in Plata: 300, 400, 500, 700

| |Primary|Fallback|
|:-----|:-----:|:-----:|
|Gnome-Shell|**Roboto**|Sans-serif|
|Cinnamon   |**Roboto**|Sans-serif|

Plata is designed with nominal **13px (or 14px)** Roboto Regular font.
In Gnome, "window-scaling-factor = 1.0" means `-gtk-dpi = 96`, it also means:
  ```
  13 [px] x 72 [pt/inch] / 96 [px/inch] = 9.75 [pt]
  14 [px] x 72 [pt/inch] / 96 [px/inch] = 10.5 [pt]
  ```
That's the reason why `13.33px = 10pt` is used for rem/px conversion in Gtk+ 3.2x/4.0 theming.

> **Note:**
>
> NotoSans CJK (ChineseJapaneseKorean) opentype fonts are actually **0.1em taller than Roboto fonts**, so if 10pt Roboto was suitable on your LCDs, set 9pt for NotoSans CJK families.

**Verify the fonts are rendered correctly via font-viewer tools like Gnome-Font-Viewer.**

Required Components
-------------------
Plata supports Gtk+ 2.24.x, 3.20.x, 3.22.x and 3.24.x.

 ```
 * Gtk+-3.0             >= 3.20.0
 * Gtk+-2.0             >= 2.24.30
 * gtk2-engines-pixbuf  >= 2.24.30
 * gtk2-engines-murrine >= 0.98.1
 ```

Supported Desktop Environments
------------------------------

 ```
 * GNOME-Shell     >= 3.20.0
 * GNOME-Flashback >= 3.20
 * Budgie-Desktop  >= 10.4
 * Cinnamon        >= 3.2.0
 * XFce4           >= 4.12.2
 * LXDE            >= 0.99.1 (Gtk+ 2.x only)
 ```

Unsupported Gtk+ Based Desktop(s)
-------------------------------
 * Pantheon
 * Unity7
 * Gnome-Shell customed by Canonical ( = Ubuntu session)
 * Mate

 > **Note:**
 >
 >   * Plata does NOT support elementaryOS.

Installation from this Repository
---------------------------------
 * git clone https://github.com/madgrid/plata-theme-compiled.git
 * cd plata-theme-compiled
 * cp -r Plata-Noir-Compact ~/.themes (or any other theme variant)

Additional Installation from Package(s)
----------------------------
 * Arch (AUR): [**plata-theme**](https://aur.archlinux.org/packages/plata-theme)
 * OpenSUSE: [**Official repository**](https://software.opensuse.org/package/plata-theme)
 * Solus: Official repository
 * Flatpak: Official flathub repository (current package branch = **3.22**)
 * My Personal Package Archives (PPA): [**plata-theme**](https://launchpad.net/~tista/+archive/ubuntu/plata-theme)


Extra Browser Support
---------------------
To try our color samples for FirefoxColor test pilot, check these URLs:

  1. [**Plata**](https://color.firefox.com/?theme=XQAAAAL8AAAAAAAAAABBKYhm849SCia2CaaEGccwS-xNKliFvd9NUAF6ENY3kBjKL2oHo45W2-O_o0hH8v9jyb1gPLS8xyg320t5BtQBRbshC37eqwUpEtrNzUXzzCCGCEnPVujOpTgJBqePqVNh4q1nxYUIdLIFaoaGFtpU8UGWTHdYK89VREGS2_uycyNkLyT_fUsp3rt8085FMcIrk2zP6zlQ8nXHifYExWUlXde95kD4F3H_cvgAAA)

  2. [**Plata-Lumine**](https://color.firefox.com/?theme=XQAAAAL8AAAAAAAAAABBKYhm849SCia2CaaEGccwS-xNKliFvd9NUAF6ENY3kBjKL2oHo45W2-O_o0hH8v9jyb1gPLS8xyg3NbO0xf8CWW1IQ-VFBeST-c2ya550Jq-AJT3qXk84PCZgv4Q1Ip6G8KMxah3hVdR8-Zr9ze0kGqgOtR7bn1Nps1cYGNzQQkA8ajSLlQnjaMNzy_Cgfm6TGsTtSGCZPEHAaGevqPSrPV7L_8f2AAA)

  3. [**Plata-Noir**](https://color.firefox.com/?theme=XQAAAAL8AAAAAAAAAABBKYhm849SCia2CaaEGccwS-xNKlhR4U3ii01izoNSwV8EzxA9i34l-h9kNzmmbht5egIz1VwqGu4asy3bC0Iu-fSfcIJAVAwKwUYrdnMCFPHjDRh3WIEk3D10l1b0yhJ2JJ4iidXrDdOeHtPXECgT4mWPRinIv4rInTDn_LmydH4PXIv_OPeKQZiffADmQZvxlSWtpsLQfUznQX8sEtOtxfBaEVM7_-LnUAA)

 > **Note:**
 >
 >   * We no longer support "Normal" UI layout in Chrome(ium). Use "Refresh" instead.
 >
 >   * Vivaldi can make custom themes via settings like these:
 >     ```
 >     Background: #F8F8F8 (#1D1D1D)
 >     Foreground: #111111 (#F5F5F5)
 >     Highlight:  #3F51B5
 >     Accent:     #E7E7E7 (#080808)
 >     Accent Color from Active Page: [ ]
 >     Apply Accent Color to Window:  [*]
 >     Transparent Tabs:              [*]
 >     Corner Rounding:               2px
 >     ```

All credit goes to @tista500
Gitlab: https://gitlab.com/tista500/plata-theme.git
--------------
 Nana-4, the developer of Materia (formerly Flat-Plat)

 Sam Hewitt, the developer of Paper-icon theme
