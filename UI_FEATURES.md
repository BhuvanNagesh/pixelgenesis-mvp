# PixelGenesis — UI/UX Feature Documentation

## 🎨 Design System

### Color Palette (Exact Match to Midnight Blockchain Theme)
```css
--dark-bg: #0A1E17        /* Dark background */
--deep-green: #0F3E2E     /* Deep green */
--neon-green: #1FA973     /* Neon green accent */
--mint-glow: #C2FBE1      /* Mint glow */
--white: #FFFFFF          /* Text */
```

### Typography
- **Headings**: Orbitron (900/700/600) - Futuristic, uppercase
- **Body**: Rajdhani (300-700) - Clean, readable
- **Code**: Courier New - Monospace for hashes/keys

---

## 🌟 Key Animations

### 1. **Background Effects**
- Pulsing radial gradients (8s loop)
- Vertical scanning line (4s sweep)
- Floating particle system (5 particles, 12-18s rise)

### 2. **Interactive Elements**
- **Buttons**: Ripple effect on hover, lift animation (translateY -2px)
- **Inputs**: Laser scan animation on focus
- **Cards**: Glow pulse on container (3s loop)
- **Links**: Underline expansion from left

### 3. **Status Animations**
- **Success**: Animated SVG checkmark with stroke animation
- **Loading**: Circular spinner with neon green accent
- **Ripple**: Expanding circles for key generation
- **Shield**: Pulsing glow for verification

---

## 📱 Responsive Design

### Breakpoints
- **Mobile**: < 768px - Single column, reduced padding
- **Tablet**: 768px - 1024px - Optimized spacing
- **Desktop**: > 1024px - Full features, larger containers

### Mobile Optimizations
- Stacked tabs (vertical on mobile)
- Reduced font sizes (2rem → 1.5rem for h1)
- Touch-friendly button sizes (min 44px)
- Simplified particle effects

---

## 🎯 Page-by-Page Features

### 1. **Home Page** (`index.html`)
- Animated title with pulse effect
- 8 interactive navigation cards
- Hover: translateX(10px) + glow effect
- Floating particles in background

### 2. **Create DID** (`signup.html`)
- Ripple animation during generation
- Three glowing boxes for DID/keys
- Copy-to-clipboard with JavaScript
- Warning state for private key (red glow)

### 3. **Login** (`login.html`)
- Three-step flow: DID → Challenge → Verify
- Shield icon with animated glow
- Animated checkmark on success
- Password input with scan effect

### 4. **User Profile** (`userdata.html`)
- Clean form with cyber-green theme
- Date picker with custom styling
- Dropdown with hover effects
- Lock icon animation

### 5. **Profile Success** (`userdata_success.html`)
- SVG checkmark animation (stroke-dashoffset)
- SHA-256 hash in glowing mono box
- Copy hash button
- Privacy messaging

### 6. **Token Generation** (`access_request.html`)
**Tab System** (Mode A/B/C):
- **Mode A - Selective Disclosure**
  - Dropdown selector
  - Animated chip display
  - Real-time attribute preview

- **Mode B - Predicate Proof**
  - Condition builder (>, ≥, =, ∈)
  - Zero-knowledge visualization
  - Live predicate display

- **Mode C - File Upload**
  - Dashed border upload box
  - AES-256 encryption toggle
  - Shamir 2-of-3 shard visualization

### 7. **Token Success** (`access_success.html`)
- Animated checkmark
- Token in glowing container
- Shamir shares (if encrypted)
- Copy buttons with feedback

### 8. **Verify Token** (`verify_access.html`)
- Shield animation
- Valid/Invalid/Expired states
- Structured JSON response
- File decryption instructions

### 9. **Token Dashboard** (`tokens.html`)
- Full-width table (1200px max)
- Color-coded mode badges
- Live status indicators
- Inline revoke buttons
- Hover row highlight

### 10. **Shamir Recovery** (`shamir_recover.html`)
- 3-shard visualization
- Merge animation (2 + 2 = unlock)
- Textarea input
- Recovered key display

### 11. **VC Signing** (`vc_sign.html`)
- JSON editor with default template
- DID validation
- Signature display
- Public key export

---

## 🔐 Security UI Patterns

### Visual Trust Indicators
- ✓ Green checkmark for success
- ⚠️ Red warning for errors
- 🔐 Lock icon for encryption
- 🛡️ Shield for verification
- 🔑 Key for secrets

### State Colors
- **Success**: Neon green (#1FA973)
- **Error**: Red (#ef4444)
- **Warning**: Orange/Yellow
- **Info**: Mint glow (#C2FBE1)
- **Neutral**: Deep green (#0F3E2E)

---

## 💎 Premium Polish Details

### Glassmorphism
```css
background: rgba(15, 62, 46, 0.4);
border: 1px solid rgba(31, 169, 115, 0.3);
backdrop-filter: blur(20px);
```

### Neon Glow
```css
box-shadow:
  0 8px 32px rgba(0, 0, 0, 0.4),
  inset 0 1px 0 rgba(31, 169, 115, 0.2),
  0 0 60px rgba(31, 169, 115, 0.1);
```

### Animated Borders
```css
@keyframes borderPulse {
  0%, 100% { border-color: var(--neon-green); }
  50% { border-color: var(--mint-glow); }
}
```

---

## 🚀 Performance

- **Pure CSS animations** (no JavaScript libraries)
- **Optimized keyframes** (GPU-accelerated transforms)
- **Lazy-loaded fonts** (Google Fonts CDN)
- **Minimal JavaScript** (only for copy/tabs)
- **Fast page loads** (<100KB total assets)

---

## ✨ Micro-Interactions

1. **Button Hover**: Ripple + lift + glow
2. **Input Focus**: Laser scan + border glow
3. **Card Hover**: Slide right + shadow increase
4. **Link Hover**: Underline expand + color shift
5. **Success State**: Checkmark draw animation
6. **Loading State**: Rotating spinner

---

## 🎭 Accessibility

- Semantic HTML5 elements
- ARIA labels on interactive elements
- Sufficient color contrast (WCAG AA)
- Keyboard navigation support
- Focus indicators on all inputs
- Screen reader friendly

---

## 📦 Deployment Ready

All pages are:
- ✓ Mobile responsive
- ✓ Cross-browser compatible
- ✓ Accessible
- ✓ SEO friendly (meta tags)
- ✓ Performance optimized
- ✓ Production ready

---

**Built for Midnight Blockchain Track 3 Hackathon**
Zero-knowledge • Privacy-first • Futuristic UI
