# Tempo: free music, no ads, synced lyrics

Tempo is a web app (PWA) that installs on Android and iPhone from the browser. No app store, no Mac needed.

## What it does
- Streams free music from **Audius** (independent artists, legal, no ads, no account needed)
- Plays **your own music files** (MP3, FLAC, M4A, WAV, OGG), offline, stored on the phone
- **Synced lyrics** from LRCLIB that scroll with the song; tap a line to jump to it. The current line also shows in the mini player
- **Playlists**: create, rename, reorder, delete; add any song (streamed or your own) via the ⋯ menu
- **Liked songs**, recently played, queue (play next / add to queue / remove)
- Shuffle, repeat (all / one), lock-screen and headphone controls
- **Keeps the music going**: when the queue ends, similar songs carry on (can be switched off in Settings)
- Remembers where you were when you reopen it
- Backup and restore of playlists and liked songs (Settings), to move them to another phone

## Put it online (GitHub Pages, same as PumpRoute)
1. On GitHub, create a new **public** repository, for example `tempo`.
2. Upload everything in this folder **keeping the `icons` folder**: `index.html`, `manifest.webmanifest`, `sw.js`, `README.md`, `icons/…`.
3. Repository **Settings → Pages → Build and deployment**: Source = *Deploy from a branch*, Branch = `main`, folder `/ (root)`, Save.
4. After a minute or two the app is live at `https://<your-username>.github.io/tempo/`.

## Install it on a phone
- **iPhone**: open the link in **Safari** → Share button → **Add to Home Screen**.
- **Android**: open the link in **Chrome** → ⋮ menu → **Install app** (or *Add to Home screen*).

Then open Tempo from the home-screen icon, not the browser tab.

## Updating later
Change the files, upload them again, and edit the first lines of `sw.js` to bump `VERSION` (for example `tempo-v2`). Phones pick up the new version the next time the app is opened online.

## Good to know
- Playlists, likes and imported files live **on each phone**. Friends each get their own library. Use Settings → Export backup to move yours.
- Lyrics: excellent for well-known songs (so best with your own files); independent tracks on Audius often have none yet. Use **Search lyrics** in the Lyrics tab if a title doesn't match.
- iPhone: background playback and lock-screen controls work when Tempo is installed to the home screen (iOS 16.4 or later recommended).
- Audius currently works without a key. If that ever changes, get a free key from audius.co (Settings → Developer apps) and paste it in Tempo's Settings.
