# Acid for rofi

Two flavours: **Acetic** (`#000000`), vibrant, and **Citric** (`#1c1b19`), muted.

Part of [Acid](https://github.com/acid-theme/acid), a very dark colourscheme in two
flavours. The main README lists the other ports.

## Preview

| Acetic | Citric |
| --- | --- |
| ![Acid Acetic](previews/acetic.png) | ![Acid Citric](previews/citric.png) |

## Install

```sh
curl -fsSLo ~/.config/rofi/acid-acetic.rasi \
  https://raw.githubusercontent.com/acid-theme/rofi/main/acid-acetic.rasi
```

The theme is the role names only. Import it and map them onto rofi's widgets:

```rasi
@import "acid-acetic"

* {
    background-color: @base;
    text-color:       @text;
    border-color:     @surface2;
}

inputbar {
    background-color: @mantle;
    text-color:       @text;
}

element selected.normal {
    background-color: @surface1;
    text-color:       @text;
}

element.active {
    text-color: @aqua;
}
```

rofi accepts a name it does not know without complaint, so a misspelled role
leaves that widget on rofi's own default rather than failing.

## Files

- `acid-acetic.rasi`
- `acid-citric.rasi`

## Generated

Acid 0.1.0, rendered by acidify from
[`ports/rofi/acid.rasi.tera`](https://github.com/acid-theme/acid/blob/main/ports/rofi/acid.rasi.tera).
Edits to these files are overwritten on the next release. Report issues on
[acid-theme/acid](https://github.com/acid-theme/acid/issues).

## Licence

MIT.
