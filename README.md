# Book Store

A responsive, single-page website for an independent bookstore in Nairobi. The site presents curated fiction, non-fiction, bookseller recommendations, upcoming events, and a contact form for book enquiries.

## Features

- Responsive layout for desktop, tablet, and mobile screens
- Sticky navigation with smooth scrolling to each section
- Hero section with bookstore introduction and featured imagery
- Curated collections for:
  - Fiction
  - Non-fiction
  - Staff picks
- Upcoming events section
- Contact form for availability, pricing, delivery, and recommendations
- Accessible labels, alternative text, keyboard focus styles, and semantic HTML
- Local image assets with Google Fonts loaded from the stylesheet

## Project structure

```text
Bookstore/
├── index.html              # Main page markup and content
├── Styles.css              # Responsive layout, typography, and theme styles
├── Images/
│   ├── Hero_Image.avif     # Hero image
│   ├── fiction/            # Fiction book covers
│   ├── nonfiction/         # Non-fiction book covers
│   ├── staffpick/           # Bookseller recommendation covers
│   └── events/              # Event artwork
└── README.md
```

## Run locally

This is a static website and does not require a build step or package installation.

### Option 1: Open the file directly

Open `index.html` in a modern web browser.

### Option 2: Use a local server

Serving the project locally is recommended for more realistic browser testing:

```bash
python -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000).

## Editing the site

- Update page text, book titles, prices, event details, and contact information in `index.html`.
- Add or replace images in the relevant `Images/` subdirectory, then update the corresponding `src` and `alt` attributes.
- Adjust colors, spacing, typography, responsive breakpoints, and component styles in `Styles.css`.
- Keep image paths relative to `index.html` so the page works when opened directly or served locally.

## Contact form

The form currently uses a `mailto:` action and opens the visitor's default email client:

```text
hello@bookstore.example
```

For production use, replace the form action with a server-side form handler or a trusted form service. The displayed address, phone number, opening hours, and social links are sample bookstore details and should be updated before launch.

## Browser testing checklist

Before publishing, verify:

1. Navigation links scroll to the intended sections.
2. All local images load and have meaningful alternative text.
3. The contact form validates required fields and opens the intended mail client or production form endpoint.
4. The layout remains usable at mobile, tablet, and desktop widths.
5. Keyboard users can reach navigation links, cards, form controls, and footer links.
6. External font loading has an acceptable fallback when offline.

## License

No license has been specified for this project. Add a license before distributing the code or website publicly.
