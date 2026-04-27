# PDF Toolkit

A lightweight, browser-based PDF utility tool — no server, no installs, no file uploads. Everything runs locally in your browser.

---

## Features

| Tool | Description |
|------|-------------|
| **Remove pages** | Load a PDF, select pages to delete, download the trimmed result |
| **Images → PDF** | Combine multiple images (JPG, PNG, WebP) into a single PDF |
| **PDF → Images** | Split a PDF and export every page as a high-resolution PNG |

---

## Demo

> Open `pdf-toolkit.html` directly in any modern browser — no setup required.

If hosted on GitHub Pages:

```
https://<your-username>.github.io/<your-repo>/pdf-toolkit.html
```

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
```

### 2. Open in browser

```bash
# Option A — just open the file
open pdf-toolkit.html

# Option B — serve locally (avoids any browser file:// restrictions)
npx serve .
# or
python3 -m http.server 8080
```

Then visit `http://localhost:8080/pdf-toolkit.html`.

---

## Usage

### Remove pages

1. Click or drag a PDF into the drop zone.
2. Click the page chips to mark pages for removal (they turn red).
3. Click **Remove pages & download** — the trimmed PDF downloads automatically.

### Combine images into PDF

1. Click or drag one or more images (JPG, PNG, WebP) into the drop zone.
2. Use the **↑ / ↓** arrows to reorder pages, or **✕** to remove an image.
3. Click **+ Add more images** to append more files.
4. Click **Combine into PDF & download**.

### Split PDF into images

1. Click or drag a PDF into the drop zone.
2. Page thumbnails render as a preview.
3. Click **Download all pages as PNG** — each page saves as `page-001.png`, `page-002.png`, etc.

---

## Tech Stack

| Library | Version | Purpose |
|---------|---------|---------|
| [pdf-lib](https://pdf-lib.js.org/) | 1.17.1 | Create, edit, and merge PDFs |
| [PDF.js](https://mozilla.github.io/pdf.js/) | 3.11.174 | Render PDF pages to canvas |

Both libraries are loaded from [cdnjs](https://cdnjs.com/) — no npm install needed.

---

## File Structure

```
.
├── pdf-toolkit.html   # The entire app (single file)
└── README.md
```

---

## Browser Support

| Browser | Supported |
|---------|-----------|
| Chrome 90+ | ✅ |
| Firefox 90+ | ✅ |
| Edge 90+ | ✅ |
| Safari 15+ | ✅ |
| Mobile browsers | ✅ |

---

## Privacy

All file processing happens **entirely in your browser**. No files or data are ever sent to a server.

---

## Deploy to GitHub Pages

1. Push `pdf-toolkit.html` and `README.md` to your repository.
2. Go to **Settings → Pages**.
3. Set the source to your main branch and root folder.
4. Your tool will be live at:

```
https://<your-username>.github.io/<your-repo>/pdf-toolkit.html
```

---

## License

MIT — free to use, modify, and distribute.
