# Rashmi — Portfolio Website

## Folder Structure

```
rashmi-portfolio/
├── index.html        ← the website (do not edit unless changing design)
├── data.json         ← all content lives here (edit this to update)
├── README.md         ← this file
└── images/
    ├── Photo_1.jpg
    ├── Photo_2.jpg
    └── ... all painting images here
```

---

## How to Add a New Painting

**Step 1 — Add the image**
Copy the new painting's photo into the `images/` folder.
Name it clearly: `Photo_12.jpg` or something descriptive like `Woman_at_Window.jpg`

**Step 2 — Open data.json**
Find the `"paintings"` array and add a new entry at the end, before the closing `]`

Copy this template and fill in the details:
```json
{
  "id": "P12",
  "file": "images/Photo_12.jpg",
  "title": "Title of Painting",
  "year": "2025",
  "dims": "24 x 36 inches",
  "medium": "Acrylic on canvas",
  "story": "The story behind this piece — who commissioned it, where it was shown, what inspired it.",
  "status": "Available",
  "series": "",
  "featured": false
}
```

**Status options:** `Available` / `Sold` / `Commissioned` / `Not for sale`

**Step 3 — Update the stats**
In `data.json`, find `"stats"` near the top and update the numbers:
```json
"stats": {
  "works": 14,
  "exhibitions": 2,
  "sold": 11
}
```

**Step 4 — Upload to GitHub**
- Go to your GitHub repository
- Drag the new image into the `images/` folder
- Upload the updated `data.json`
- Live in 60 seconds

---

## How to Add a Business Channel / Collaboration

When Rashmi's work is placed in a café, yoga studio, or any partner space,
add it to the `"channels"` array in `data.json`:

```json
{
  "name": "DYU Art Cafe",
  "type": "Café",
  "model": "Consignment · 70/30 split",
  "status": "Active",
  "since": "June 2025"
}
```

The Collaborations section on the website will appear automatically once
the first channel entry is added.

---

## How to Change the Featured Hero Image

In `data.json`, find the painting you want to feature and set `"featured": true`
Make sure all others have `"featured": false`

---

## How to Update the About Text

In `data.json`, find the `"bio"` array under `"artist"`.
Each item in the array is one paragraph. Edit, add, or remove paragraphs freely.

---

## Hosting on GitHub Pages

1. Go to github.com → your repository
2. Settings → Pages → Source: Deploy from branch → main → / (root)
3. Your site is live at: `https://YOUR-USERNAME.github.io/rashmi-portfolio`

To connect a custom domain (e.g. rashmiart.in):
- Buy domain from GoDaddy / Namecheap / Google Domains (~₹800/year)
- In GitHub Pages settings, enter your custom domain
- Follow DNS instructions — live within 24 hours

---

## Getting Help from Claude

Bring to Claude:
- New painting images (upload in chat)
- Any changes you want to the design or structure
- New channel partnerships to add

Claude will produce updated files ready to drag and drop into GitHub.
