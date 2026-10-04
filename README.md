# Kushan & Ishara — Paged paper invitation (static, Vercel-ready)
Files: `index.html`, `og.png`, and **your `music.mp3`** (same folder). No build step, nothing stored.

**Flow:** paper doors with a seal medallion → tap to open → six full screens: names · invitation & families · date & time · location & directions · countdown · thank-you. A "Scroll down" button, swipe, mouse wheel or arrow keys move between screens.

- **Music:** save your track as `music.mp3` next to `index.html` (`W.musicUrl`; loudness `W.musicVolume`). Starts when the doors open, loops. Use only a track you own or have licensed. The ♪ button appears only if the file exists.
- **Auto-play:** after opening, screens advance by themselves every `W.pageSeconds` (7). Any manual move pauses it; the ▶ button resumes.
- **Personal links:** `https://YOUR-DOMAIN.com/?to=Thushan` → "For Thushan" on the cover and "Thank you, Thushan" at the end.
- **Before launch:** check the map (built from `W.venue.mapQuery`; paste verified links into `mapsUrl`/`directionsUrl` if needed), replace `YOUR-DOMAIN.com` in the `og:` tags, optionally set `W.whatsapp`.
- **Deploy:** push the folder to GitHub → Vercel (Framework: Other, no build command), or `npx vercel --prod`.
