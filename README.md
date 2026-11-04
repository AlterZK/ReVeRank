# ReVeRank ♡ — Red Velvet Edition (v1.3)

An unofficial, standalone Red Velvet ranking web app. Separate from VERSUS Studio; it uses its own local browser storage.

## Launch

1. Extract the ZIP to a folder.
2. Double-click `index.html` to open it in a modern desktop browser.
3. Pick a Red Velvet album or collection; its songs load **immediately**. Edit the ranking title or list if you like, then click **Start comparing**.

The album collections, rankings, local progress, and poster exports work without a server. Internet access is needed for online Apple/iTunes 30-second previews, matched album covers, and optional fonts.

## Ranking methods

- **⚡ Speed Round (fastest, approximate):** Three adaptive Swiss-style rounds, with Elo-based ratings calculated after your choices. For 142 songs, there are **213 comparisons**. All songs receive a numbered rank at the end, but neighboring placements, especially in the middle of the ranking, are **estimates**. They are *not guaranteed to be the true order*, even assuming consistent preferences.
- **✦ Smart Merge Sort (accurate, recommended):** Uses transitivity (A > B and B > C implies A > C). Generates a complete consistent ordering with at most **881 comparisons** for 142 songs.
- **♡ Exhaustive:** Checks each unique pair; 10,011 comparisons for 142 songs.

All three modes support saved progress, undo, ranking titles, CSV/JSON exports, and image exports. **Old ranking projects still open in their original modes.** Rankings stay hidden until completion. You can use the left/right arrow keys to vote.

## Music player

Only the **online audio preview** button remains under each song's card. It plays short previews where the Apple/iTunes catalog offers them. Local audio uploads, folder selection, and local-file playback have been removed.

## Poster exporter

Finish a ranking, then use **Export picture** in the top results toolbar. In the dialog, the **Download picture** action is visible in the header without needing to scroll.

Choose PNG or JPEG, a customizable poster title, optional covers, and Portrait / Square / 16:9 Widescreen. The poster highlights the top three and can show Top 10, 20, 50, 100, a custom count, or **all ranked items**. If the chosen list is long, the canvas grows in height to fit it.

**14 poster themes:** Midnight Violet, Sunset Glow, Ocean Blue, Minimal Black, Spring Waltz, Cosmic Dream, The Red Pop, Velvet Noir, Sweet Cream, Midnight Peek, Porcelain Lace, Royal Sparkle, Birthday Confetti, Summer Magic. Some themes evoke Red Velvet eras through original abstract, floral, starry, candy, or lace motifs; they do **not** copy official album art.

The preview and download render locally via Canvas. When third-party cover art cannot be safely loaded into an export, the artwork uses a placeholder instead of making the preview fail. Actual album-cover images can still appear in comparisons.

## Collections

- Full curated Red Velvet group discography (~150 non-duplicate tracks)
- Red Velvet title tracks
- Korean & Japanese albums, EPs, reissues, and selected remixes
- Irene & Seulgi sub-unit releases
- Irene, Seulgi, Wendy, Joy, Yeri solo collections and selected releases
- Curated Red / Velvet style playlists and B-sides

Presets are curated, not guaranteed to be a definitive exhaustive discography. You can add and remove songs before starting. Switching collections replaces the *current unsaved draft* only, not your saved rankings.

## Backups

**Milestone popups have been removed.** The comparison counter and progress bar remain visible, and progress still saves automatically after each choice.

**Export backup** on the home screen saves the full in-progress project data. **Import backup** restores it after confirmation, replacing browser-local rankings. Because localStorage is bound to your browser and file path, keep a backup when moving the app to another folder or changing browsers.

## Disclaimer

Fan-made, unofficial tool; not affiliated with Red Velvet, SM Entertainment, Apple, or Wikimedia. This app bundles no recorded music or official cover images.
