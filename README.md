# Fall 2025 NSO Mentor Map

This project is a web-based interactive map and schedule tool designed for mentors participating in BYU’s Fall 2025 New Student Orientation (NSO). It helps mentors:

- View their assigned meeting locations on a campus map
- Check room assignments by supervisor group
- Access a schedule tailored to mentor responsibilities

---

## 📁 Project Structure

- `index.html` — Main interactive map page with all 160+ mentor meeting spots
- `spot.html` — Detail page showing the description and image for each spot
- `rooms.html` — Room assignments organized by mentor supervisor groups
- `schedule.html` — NSO schedule formatted specifically for mentors
- `css/styles.css` — Custom styling, including color-coded map spots
- `js/main.js` — Hover preview and spot interaction logic
- `images/spot-#.jpeg` — Images of each meeting spot

---

## 🎨 Color Group Assignments

Mentor groups are color-coded by supervisor:

| Color   | Number of Spots | Group Name (if any) |
|---------|------------------|---------------------|
| 🔴 Red (was pink) | 27               | Anjilee's Supervisor Group  |
| 🟡 Yellow         | 26               | Danja's Supervisor Group  |
| 🟢 Green          | 27               | New Supervisor Group  |
| 🔵 Blue           | 36               | Debi's Supervisor Group  |
| ⚫ Black          | 16               | Becky's Supervisor Group  |
| 🟣 Purple         | 26               | Sam's Supervisor Group  |
| 🟠 Orange         | 26               | Sandi's Supervisor Group  |

> Map spots are grouped visually for clarity without renumbering the files.

---

## ✅ To Do

- [ ] Add 12 more orange and purple spots (total of 26 each)
- [ ] Update spot descriptions for new spots
- [ ] Add legend to map for color group reference
- [ ] Optional: Add filtering by group on the map

---

## 📸 How to Add a New Spot

1. Add a new image to `images/spot-XYZ.jpeg`
2. Insert a new `<a class="map-spot">` entry in `index.html` with:
   - `id="spot-XYZ"`
   - `href="spot.html?id=XYZ"`
   - Inline `left` and `top` style for positioning
   - `data-group="orange"` or whatever group
3. Add a new `<div class="image-preview" id="preview-XYZ">` below with a matching `<img>`
4. Add description in `spot.html` JavaScript under `spotData[XYZ]`

---

## 👤 Contact

Built and maintained by Micah Russell and the BYU First-Year Experience Team.