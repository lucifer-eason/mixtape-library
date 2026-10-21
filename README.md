# Under an Indifferent Sun

A fully English, responsive, buildless mixtape library for Albert Camus’s *The Stranger*. Contains a record sleeve, five individual track pages, and final liner notes. Track order follows the supplied list.

## Open locally

Open `index.html` to read the booklet. For reliable official player behavior, serve the folder with a static web server or publish through GitHub Pages (HTTPS). The original music links remain available if embeds are unavailable.

## Publish on GitHub Pages

1. Create a repository named `mixtape-library` on GitHub. Use a public repository if your account does not support Pages for private repositories.
2. Upload `index.html`, `style.css`, `app.js`, `content.js`, and `.nojekyll` into its root, not inside another folder.
3. In Settings → Pages, choose **Deploy from a branch**, then **main** and **/ (root)**, and Save.
4. Wait for GitHub to finish deploying. The Pages panel displays your site URL.
5. To update the site, edit `content.js` on GitHub and commit. Pages republishes the changes.

No installation, build, API keys, or backend required. Hash routes work on GitHub Pages without rewrite rules.

## Personalize the writing

All editorial text is in `content.js`. Each song includes `title`, `artist`, `theme`, `lyrics`, `quote`, `cite`, `page`, `heading`, `paragraphs`, and `cue`. Final notes and the oral presentation draft are also there. Keep quotation marks and commas valid when editing JavaScript. The final page can download a fresh editable copy.

The supplied 318 / 312 / 308 numbers were not used as durations or page numbers because their meaning was not specified. The unavailable pasted image was not used.

### Before handing in

- Treat the analyses as drafts: revise into your own voice and connect them to your own listening and reading.
- Quotations and printed pages currently use Matthew Ward, Vintage International, 1989: 3, 3, 103, 78, 122. Check every excerpt and page in your assigned book; translation and pagination vary.
- The reference copy is linked on the website. Quotation excerpts are intentionally short; expand from your own book if your teacher needs more context.
- Full copyrighted song lyrics are not distributed. Replace lyric placeholders with permitted text, or leave them as listening notes. Dramamine is marked instrumental; Fake Heartfelt Words has an explicit title-based interpretation because lyrics were not verified.
- The last track addresses suicide; its interpretation distinguishes that from Meursault’s imposed death sentence. The booklet discusses the unnamed murder victim and does not excuse Meursault’s violence.

## Music behavior

The record and play button load the official YouTube or Spotify player on demand. Rotation follows playback events, stops when paused/buffering/ended, and is disabled for reduced-motion preferences. Changing pages destroys the previous player to avoid overlapping audio. Full-track playback, previews, ads, login, and availability are controlled by the music platforms. Playback can require an additional click inside their player because of browser restrictions. No audio files are bundled or downloaded. External fonts use Google Fonts with local serif/sans-serif fallbacks.

## Present in class

Choose Presentation mode to show a concise speaking prompt on each track page. Left/right arrow keys move between tracks. The final page has a condensed speaking draft and a copy button.

## Files

- `index.html`: page shell
- `content.js`: editable booklet and music links
- `app.js`: page navigation and official-player controls
- `style.css`: layout, palette, record illustration, responsive and print styles
- `.nojekyll`: static GitHub Pages compatibility

## Album artwork

The five images supplied by the user are bundled beside `index.html`. Each track’s `cover` field in `content.js` selects the centre label artwork. Artwork rotates with the vinyl and is displayed using a circular CSS crop; source images are preserved. Keep the five artwork files beside `index.html`.

## Cloudflare Pages

This repository is a buildless static site. Connect the `main` branch in Cloudflare Pages, select framework **None**, leave the build command empty, and set the build output directory to `/`. Editing files in GitHub triggers deployment through the connected Pages project.
