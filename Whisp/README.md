# Calm for Whisp

The same Calm Paper and Calm Ink palette,
for [Whisp](https://github.com/tanaybhomia/Whisp), the GNOME scratchpad modelled on Antinote.

Whisp has no theme files of its own.
It's a libadwaita app, so the palette arrives as a GTK stylesheet instead.
One file holds both themes: light follows Calm Paper, dark follows Calm Ink,
and Whisp's own system / light / dark switch chooses between them.

## Install

For the Flathub build, put the file inside Whisp's sandbox,
so it styles Whisp and nothing else:

```bash
mkdir -p ~/.var/app/io.github.tanaybhomia.Whisp/config/gtk-4.0
cp Whisp/gtk.css ~/.var/app/io.github.tanaybhomia.Whisp/config/gtk-4.0/gtk.css
```

Restart Whisp.
For the calmest page, pick the Blank paper in Preferences.

To undo, delete that `gtk.css`.

## In honesty

Whisp colours some markdown itself, in code rather than CSS:
headings, links, list keywords and the search highlight.
Those keep Whisp's own colours.
The page, the ink, the header and the accent follow the calm palette.
