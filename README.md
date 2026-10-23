# adygabze-online-audio

Audio files for [Adygabze Online](https://adygabze-online.ru), served by GitHub Pages so that LearningApps games and the Android app can play them from a direct link:

```
https://abedshowgan.github.io/adygabze-online-audio/<folder>/<file>.mp3
```

## Conventions

- **Lowercase ASCII only, hyphens instead of spaces**, for folders and filenames. Cyrillic or spaced names get percent-encoded into long, fragile URLs.
- **Folders by purpose**: `words/`, `stories/`, `exercises/`. `test/` holds test files only.
- **Audio only.** The app's content manifest lives elsewhere; it changes often, the audio rarely, and both would share this site's 1 GB limit.
- **Never rename or delete a published file.** LearningApps games link to these URLs; a renamed file breaks every game that uses it. Add a new file instead.
- Format: MP3, mono, 44.1 kHz, 64–96 kbps for speech.

## Layout

```
index.html                 overview page with players
test/test-tones-6s.mp3     test file: low tone 0–2 s, middle 2–4 s, high 4–6 s
.nojekyll                  serve files as-is (no Jekyll processing)
```

## Limits (GitHub Pages)

1 GB per site, about 100 GB/month bandwidth (soft limit), 100 MB per file. A few hundred short clips use a few MB.
