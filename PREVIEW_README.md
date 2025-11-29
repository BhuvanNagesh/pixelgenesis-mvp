# PixelGenesis - Static Preview

## 🎨 Preview Setup

This project now includes a **static HTML preview** that showcases the beautiful cyber-green UI without requiring Flask or any backend.

### Files Added:

1. **`preview.html`** - Self-contained static preview with all CSS inline
2. **`index.html`** - Auto-redirects to preview.html

### What's Included in the Preview:

✅ **5 Interactive Sections:**
- 🏠 Home Page - Animated landing with navigation
- 🔐 Create DID - Key generation display
- 🎫 Token Generation - 3-mode tab system (Selective Disclosure, Predicate Proof, File Upload)
- ✓ Success View - Profile saved confirmation
- 🧩 Shamir Recovery - Secret share reconstruction

✅ **Full Cyber-Green Theme:**
- Dark background (#0A1E17)
- Neon green accents (#1FA973)
- Animated particles floating
- Glassmorphism cards
- Glowing borders with pulse animations
- Scanning line effects
- Smooth transitions

✅ **Animations:**
- Background pulse (8s)
- Scanning lines (4s sweep)
- Floating particles
- Button hover effects
- Input focus animations
- Animated SVG checkmark
- Tab switching

### How to View:

**Option 1: Direct File Access**
Simply open `preview.html` in your browser - no server needed!

**Option 2: With npm (if available)**
```bash
npm start
```
This will serve the files on http://localhost:5000

**Option 3: With Python**
```bash
python3 -m http.server 8000
```
Then visit http://localhost:8000/preview.html

### Navigation:

The preview includes a fixed navigation bar at the top:
- Click any nav link to switch between sections
- Click navigation cards on the home page
- Use the buttons within each section

### Original Flask App:

Your original Flask application (`app.py` and all `templates/`) remains **completely untouched** and fully functional for production use.

---

## 🎯 Purpose

This static preview allows:
- Quick UI demonstration without backend setup
- Easy sharing with stakeholders
- Visual testing of the cyber-green theme
- Showcase for hackathon judges
- Portfolio presentation

The preview replicates the exact look and feel of your Flask templates but with static, non-functional forms (no actual data submission).

---

**Built for Midnight Blockchain Track 3 Hackathon**
Zero-knowledge • Privacy-first • Futuristic UI
