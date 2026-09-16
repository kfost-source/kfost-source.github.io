# Windows 98 asset collection

Downloaded 2026-09-15. This folder is independent of the website checkout.

## Ready-to-use files

- `icons/`: 39 PNG files. Most have separate native 16×16 and 32×32 variants.
- `wallpapers/clouds.jpg`: classic Clouds image, 640×480.
- `wallpapers/setup.png`: classic Setup image, 640×480.
- `wallpapers/bubbles.png`: classic Bubbles repeating tile, 64×64.
- `wallpapers/waves.png`: classic Waves repeating tile, 32×32.
- `wallpapers/*.bmp`: the three original bitmap downloads, retained alongside lossless PNG copies.
- `fonts/ms_sans_serif.woff2` and `fonts/ms_sans_serif_bold.woff2`: pixel MS Sans Serif-style regular and bold webfonts from 98.css.
- `fonts/font-face.css`: ready-to-copy webfont declarations.

## Icon mapping

| Purpose | File stem in icons/ |
|---|---|
| Closed / open folder | folder / folder-open |
| Generic document | document |
| Notepad application / text file | notepad / notepad-file |
| Paint | paint |
| Minesweeper | minesweeper |
| Computer / display | my-computer |
| Internet globe | zone-internet |
| Internet Explorer | internet-explorer |
| Generic executable / application window | task |
| Settings / display themes | settings / themes |
| Programs | programs |
| Recycle Bin | recycle-bin |
| Run / Help / Shut Down | run / help / shutdown |

These stems have `-16x16.png` and `-32x32.png` variants. Extras: `start-logo.png` (23×18), `windows-32x32.png`, and `start-menu-side-98.png` (21×30 source artwork).

Render icons at native size or integer multiples with `image-rendering: pixelated`. Tile Bubbles and Waves at native size with `background-repeat: repeat`.

## Sources and reuse information

**Icons and Clouds:** [1j01/98](https://github.com/1j01/98), revision `5245105214cee90ab984fc15bece6c92db15ca7d`. The repository [README](https://github.com/1j01/98/blob/master/README.md#license) says the project is not yet licensed and is source-available/shared source, not open source. No separate permissive license for these Windows graphics was established.

**Setup, Bubbles, Waves:** [azayrahmad/win98-web](https://github.com/azayrahmad/win98-web), revision `e7ddf164cf982d160b4fe52ea073fbe04f6c9372`, `src/assets/img/wallpapers/default/`. Its code license is MIT, but its README and [credits](https://github.com/azayrahmad/win98-web/blob/main/CREDITS.md) explicitly attribute original Windows artwork, icons, cursors, and media rights to Microsoft Corporation. That code license should not be represented as a permissive license for the original Microsoft assets.

**Fonts:** [jdan/98.css](https://github.com/jdan/98.css/tree/main/fonts/converted), downloaded from `main`. The repository uses the [MIT license](https://github.com/jdan/98.css/blob/main/LICENSE), copyright 2020 Jordan Scales. Keep the supplied `source/98-css-LICENSE.txt` when redistributing these font files.

`asset-manifest.json` records every download URL, byte count, SHA-256 hash, and image dimensions. Original repository notices are retained under `source/`.

## Verification

All downloaded PNG, JPEG, and BMP images decoded successfully. PNG wallpaper copies preserve exactly the original RGBA pixels. Both webfonts have valid WOFF2 signatures and matching declared/actual file lengths. Clouds, Paint, and the generic application icon were visually inspected; wallpaper PNGs were inspected after conversion.
