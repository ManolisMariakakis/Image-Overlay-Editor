# 🎶 Lyric Editor for Scanned Sheet Music (Image Overlay Editor)

A simple web-based image overlay and text editing tool built with [Fabric.js](http://fabricjs.com/) version 5.2.4. This editor allows you to load a background image, add and style text overlays, erase parts of the image, crop areas, undo/redo changes, and export your work as PNG or JSON.

> 🎶 **This tool is especially created for adding lyrics to scanned or image-based musical scores (partitures) where lyrics in other languages have been erased.** You can use it to easily overlay new text on PNG sheet music images.


## ✨ Features

- **Upload Background Image** (`.png` only)
- **Add Textbox** with customizable:
  - Font family
  - Font size
  - Bold toggle
- **Erase Tool** with adjustable brush size
- **Crop Mode**: Select and duplicate a portion of the background as a new object
- **Undo / Redo** support
- **Export** your canvas as PNG or JSON
- **Import** canvas state from JSON
- **Context Menu** on textboxes (right-click):
  - Delete
  - Duplicate
  - Bring to front
  - Send to back
- **Keyboard Support** for moving textboxes with arrow keys

## 🧰 Tech Stack

- HTML / CSS / JavaScript
- [Fabric.js 5.2.4](https://cdnjs.com/libraries/fabric.js/5.2.4)

## 🗂️ Folder Structure

```
ImageOverlayEditor/
│
├── index.html         # Main application
├── a4_1.png           # Default background image (partiture page 1 without lyrics)
├── a4_2.png           # Background image (partiture page 2 without lyrics)
├── a4_1.json          # Lyrics of partiture a4_1.png
├── a4_1.json          # Lyrics of partiture a4_2.png
└── README.md          # You are here
```

## 🚀 Getting Started

1. **Clone or download** the project.
2. Open `index.html` in a browser.

That's it! No build steps or dependencies required.

## 📦 Functionality Overview

### Toolbar

- **Left:**
  - Upload background image
  - Load saved JSON
- **Center:**
  - Add textbox
  - Change font and size
  - Bold toggle
  - Delete selected
  - Selection mode
  - Eraser mode with brush size
  - Crop mode
- **Right:**
  - Undo / Redo
  - Export as PNG
  - Save as JSON

### Context Menu (Right-click on textbox)

- Delete
- Duplicate
- Bring to front
- Send to back

## 📸 Exporting

- **PNG Export**: Saves the canvas as a PNG image.
- **JSON Export**: Saves the current canvas state, including objects and properties, for later reuse.

## 📥 Importing

- Upload a previously saved `.json` file to restore your session.

## 🖱️ Cropping Instructions

1. Click **Crop Mode**.
2. Click and drag to select an area.
3. The area is:
   - Erased from the background
   - Added as a separate image object on top

## 🔒 Notes

- All images are loaded with `crossOrigin: 'anonymous'` to support canvas export.
- Only `.png` images are currently supported for background upload.

## 📝 License

MIT — free to use, modify, and distribute.
