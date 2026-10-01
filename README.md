# JSON Visualizer

A lightweight tool for Product Managers and Engineers that turns a raw API JSON payload into a visual front-end mockup.

## The problem

Product Managers spend a lot of time reading raw API docs, JSON payloads and webhooks. Working out how that data becomes the end-user experience often takes a sync meeting with engineering, which slows down product decisions.

## What it does

Paste a payload (or open/drop a `.json` file) and immediately see how it would look to a user:

- **Detects the payload shape**: webhook events become a notification plus a detail page; paginated list responses become a list page with result count, filter chips and page controls; single records become a detail page.
- **Picks a UI component for each field**: status pills with good/warning/error colors, formatted prices (including amounts stored in cents), readable dates, avatars and thumbnails, tables or cards for lists, trend charts for number series, address blocks and more.
- **Hides what users shouldn't see**: record IDs and system fields are tucked into a "Developer fields" section.
- **Hover to trace**: hover any part of the mockup to see which JSON field it came from.
- **Field map**: every field with an example value, type, how it's shown, and whether it's on screen, hidden or empty. Copy it as a Markdown table for a PRD or ticket.
- Desktop/mobile preview, Auto/Cards/Table list layouts, light and dark themes.

Field detection is rule-based (field names and value formats), so unusual fields may be guessed wrong. The Field map shows every guess.

## Run it

It's a single static file with no build step. Open `index.html` in a browser, or use the GitHub Pages link for this repo.
