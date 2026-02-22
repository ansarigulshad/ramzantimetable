# 🌙 Ramzan 2026 — Sehri & Iftar Timings

A beautifully designed, interactive Ramzan timing card for major Indian cities. Built as a single-file static web app — no backend, no dependencies to install, ready to host on GitHub Pages.

![Ramzan 2026](https://img.shields.io/badge/Ramzan-2026%20%7C%201447%20AH-C9A84C?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0id2hpdGUiIGQ9Ik0yMSAxMi4yOEE5IDkgMCAxIDEgMTEuNzIgM2E3IDcgMCAxIDAgOS4yOCA5LjI4eiIvPjwvc3ZnPg==)
![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-181717?style=for-the-badge&logo=github)

---

## ✨ Features

- 🕌 **Live countdown** to Sehri & Iftar (updates every second)
- 🗓️ **Full 30-Roza schedule** — click any city to expand its complete timetable
- 🌆 **6 Indian cities** — Pune, Mumbai, Delhi, Hyderabad, Solapur, Bangalore
- 🌙 **Today's Roza** automatically highlighted
- ⭐ Animated starry night background & crescent moon
- 📱 Fully **responsive** — works on mobile, tablet, desktop
- ⚡ **Zero dependencies** — pure HTML, CSS, JavaScript (Google Fonts via CDN only)

---

## 📁 Project Structure

```
ramzan-2026/
├── index.html       ← The entire app (single file)
└── README.md        ← This file
```

That's it. The whole app lives in one HTML file.

---

## 🚀 Hosting on GitHub Pages

### Step 1 — Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click **"New"** (green button, top left)
3. Name your repo — e.g. `ramzan-2026`
4. Set visibility to **Public**
5. Click **"Create repository"**

---

### Step 2 — Upload the Files

**Option A — via GitHub website (easiest)**

1. Inside your new repo, click **"Add file" → "Upload files"**
2. Drag and drop both `index.html` and `README.md`
3. Scroll down, write a commit message like `Initial upload`
4. Click **"Commit changes"**

**Option B — via Git CLI**

```bash
git clone https://github.com/YOUR_USERNAME/ramzan-2026.git
cd ramzan-2026

# Copy your index.html and README.md into this folder, then:
git add .
git commit -m "Initial upload"
git push origin main
```

---

### Step 3 — Enable GitHub Pages

1. In your repo, go to **Settings** (top navigation)
2. Scroll down to **"Pages"** in the left sidebar
3. Under **"Source"**, select:
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Wait ~60 seconds, then your site will be live at:

```
https://YOUR_USERNAME.github.io/ramzan-2026/
```

> GitHub will show a blue banner at the top of the Pages settings with your live URL once it's ready.

---

## 🌆 Cities Covered

| City | Timezone Note |
|------|--------------|
| Pune | Base city (IST UTC+5:30) |
| Mumbai | ~16 min later sehri than Pune |
| Delhi | Earlier sehri, earlier iftar |
| Hyderabad | ~2 min earlier than Pune |
| Solapur | ~4 min earlier than Pune |
| Bangalore | Earliest iftar of the group |

---

## 📅 Schedule Details

- **Ramzan Start:** 19 February 2026 (1st Roza)
- **Ramzan End:** 20 March 2026 (30th Roza)
- **Hijri Year:** 1447 AH
- Timings are approximate — always verify with your local mosque

---

## 🛠️ Customisation

Want to add your city or tweak timings? Open `index.html` and find the `cities` array in the `<script>` section:

```javascript
const cities = [
  { key:'pune', name:'Pune', isPune:true, sch:puneSchedule },
  { key:'mumbai', name:'Mumbai', isPune:false, sch:mumbaiSchedule },
  // Add your city here ↓
  { key:'nagpur', name:'Nagpur', isPune:false, sch:nagpurSchedule },
];
```

Then define a 30-entry schedule array for your city (each entry: `[sehri_hour, sehri_min, iftar_hour, iftar_min]`).

---

## 🤲 Disclaimer

Timings displayed are calculated approximations for general guidance. Please confirm exact Sehri and Iftar times with your **local mosque** or Islamic authority.

---

## 👤 Author

Designed & developed by **Gulshad**

---

*رمضان المبارك — Ramzan Mubarak* 🌙
