Mohaned AI Portfolio — Mobile v10 Performance

Key performance changes:
- Mobile fast path skips the expensive full-deck animation/lightbox measurement pass.
- Offscreen slides use CSS content-visibility so mobile browsers can skip layout/paint work.
- Dedicated smaller mobile image files (m-img-XX.webp) are selected only on mobile; desktop still receives full-quality images.
- Videos remain preload=none on mobile and do not download video data until playback.
- Only viewport-near slides are warmed; media is no longer broadly prefetched on phones.
- _headers is included for Netlify browser caching; GitHub Pages safely ignores it.

For GitHub Pages: upload every file in this folder to the repository root.
For Netlify: drag this whole folder into Netlify Drop.
