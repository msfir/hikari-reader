# 光 Hikari — Light Novel Reader

A clean, private, single-file EPUB reader that runs entirely in your browser. No server, no accounts, no uploads — your books stay on your device.

<img width="2554" height="1342" alt="library_screenshot" src="https://github.com/user-attachments/assets/87b48874-084c-42a8-876b-36d2f89750ec" />
<img width="2558" height="1356" alt="reader_screenshot" src="https://github.com/user-attachments/assets/7c1e0b5c-96d4-432b-a93e-9ebeb01c78d3" />

---

## Features

- 📚 **Library** — drag-and-drop or browse to add `.epub` files
- 📖 **Reader** — comfortable reading with adjustable font, size, line height, and width
- 🌙 **Themes** — Light, Sepia, and Dark modes
- 🔖 **Bookmarks** — bookmark any position or highlighted text passage
- 📑 **Table of Contents** — chapter sidebar with one-click navigation
- 💾 **Persistent storage** — library saved in IndexedDB (handles large books with images); bookmarks and preferences in localStorage
- 📍 **Resume reading** — last position is saved per book automatically
- 📊 **Accurate progress** — global progress weighted by word count, not chapter count

---

## Privacy

All data (books, bookmarks, reading position) is stored **locally in your browser** using IndexedDB and localStorage. Nothing is ever sent to any server. Two people visiting the same GitHub Pages URL each have their own completely separate library.

---

## Dependencies

Hikari is a single self-contained HTML file with two external runtime dependencies loaded from CDNs:

| Library | Purpose |
|---|---|
| [JSZip 3.10](https://stuk.github.io/jszip/) | Unpacking `.epub` files (ZIP format) |
| [Google Fonts](https://fonts.google.com/) | Lora, DM Sans, DM Mono typefaces |

> **Offline use:** If you need the app to work without an internet connection, open the file locally — Google Fonts will fall back to system fonts gracefully. JSZip is required to parse EPUBs; without it books cannot be opened.

---

## License

MIT — do whatever you like with it.
