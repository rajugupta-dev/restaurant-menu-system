# 🍽️ SpiceNest — Restaurant Digital Menu

A beautiful, fully interactive digital menu system for restaurants. Customers scan a QR code to view the menu. The owner can add, edit, and delete items — all in a single HTML file, no backend needed.

---

## ✨ Features

### For Customers
- Browse menu by category (Beverages, Snacks, Healthy, Chinese, etc.)
- See item name, description, price, and veg badge
- Clean, mobile-friendly design

### For Owner
- Password-free admin panel (click "Owner Login")
- Add new items with name, price, category, emoji, and description
- Edit any existing item
- Delete items instantly
- Auto-generated QR code pointing to your live menu URL

---

## 📋 Menu Items (Pre-loaded)

| Item | Category | Price |
|------|----------|-------|
| ☕ Cold Coffee | Beverages | ₹99 |
| 🍹 Mojito | Beverages | ₹101 |
| 🌯 Veg Wraps | Snacks | ₹99 |
| 🥪 Sandwich | Snacks | ₹119 |
| 🥗 Quinoa Salad | Healthy | ₹149 |
| 🍓 Fruit Bowl | Healthy | ₹89 |
| 🥤 Green Smoothie | Healthy | ₹109 |
| 🍚 Veg Fried Rice | Chinese | ₹139 |
| 🍜 Hakka Noodles | Chinese | ₹129 |
| 🥢 Manchurian | Chinese | ₹159 |

---

## 🚀 How to Host (Free)

### Option 1 — Netlify Drop (Fastest, 30 seconds)

1. Rename the file to `index.html`
2. Go to [netlify.com/drop](https://netlify.com/drop)
3. Drag and drop the file
4. Get a live URL instantly — e.g. `https://spicenest.netlify.app`

### Option 2 — GitHub Pages

1. Create a new repo on GitHub (e.g. `spicenest-menu`)
2. Upload `index.html` to the repo
3. Go to **Settings → Pages → Source → main → Save**
4. Live at: `https://yourusername.github.io/spicenest-menu`

---

## 📱 QR Code Setup

1. Host the file using any method above
2. Open your live URL in a browser
3. Click **"Owner Login"** — the QR code auto-generates
4. Right-click the QR → **Save image**
5. Print and place on every table!

> The QR always points to the live URL of wherever the file is hosted.

---

## ✏️ How to Customize

Open `index.html` in any text editor (Notepad, VS Code, etc.)

**Change restaurant name:**
```html
<div class="brand">SpiceNest <small>RESTAURANT</small></div>
```
Replace `SpiceNest` with your restaurant name.

**Change brand color** (default is red `#c0392b`):
```css
--accent: #c0392b;
```
Replace with any hex color. E.g. `#1a6b3a` for green, `#1a4fa0` for blue.

**Add or edit menu items directly in code:**
```js
let items = [
  {id:1, name:'Cold Coffee', price:99, cat:'Beverages', emoji:'☕', desc:'...'},
  ...
];
```

**Add a new category** — in the `<select id="new-cat">` dropdown, add:
```html
<option value="Desserts">Desserts</option>
```

---

## 📁 File Structure

```
index.html       ← Everything is in this single file
README.md        ← This file
```

No framework. No backend. No database. Just one HTML file.

---

## 🛠️ Tech Used

- Pure HTML, CSS, JavaScript
- [QRCode.js](https://github.com/davidshimjs/qrcodejs) — for QR generation
- Google Fonts — Playfair Display + DM Sans

---

<p align="center">Made with ❤️ for SpiceNest Restaurant</p>
