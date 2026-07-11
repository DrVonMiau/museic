# Museic

A clean, paper-and-ink music player for Linux, built with GTK4 and libadwaita.

Museic scans your music folders into a local library — artists, albums,
tracks, favourites and playlists — and plays them gaplessly, with cover art
pulled from your files' own tags (or MusicBrainz as a fallback). It remembers
your queue, integrates with the desktop's media controls (MPRIS), and stays
out of your way.

## Features

- Library views: Artists, Albums, Tracks, Favourites, Playlists
- Gapless playback with shuffle, repeat and an editable Up Next queue
- Cover art from embedded tags, MusicBrainz/Cover Art Archive, or your own images
- Tag editing: tracks, albums and artist names, written back to the files
- MPRIS: media keys, sound menu and lock-screen controls, with seeking
- Folder watching, desktop notifications, sleep timer, light/dark theme

## Building

Open the project in **GNOME Builder** and press Run — the included Flatpak
manifest (`io.github.drvonmiau.Museic.json`) handles the rest.

Or with flatpak-builder directly:

```sh
flatpak-builder --user --install --force-clean _flatpak io.github.drvonmiau.Museic.json
flatpak run io.github.drvonmiau.Museic
```

## Design

The interface follows a Tempo-inspired mockup: a flat grey desktop, a white
"paper" card holding the library, and a floating player panel. Design assets
live in `design/`.
