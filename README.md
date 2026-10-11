# Mohaned AI Creative — v11 Mobile Deck

Architecture:
- `index.html`: desktop deck; immediately routes phones to `mobile.html`.
- `mobile.html`: one-slide virtual presentation with inline low-quality placeholders, progressive sharpening, swipe navigation, full-screen button, and lightweight slide-entry animation.
- Mobile does not render all 25 slides at once and does not use IntersectionObserver for deck navigation.
- Only the active slide requests full assets; the next slide is warmed after first paint.
