# 📸 Screenshots & Visual Guide

Visual overview of the Global Free IPTV application interface and features.

---

## 🖥️ Desktop View

### Main Interface
```
┌─────────────────────────────────────────────────────────────────────┐
│ 📺 Global Free IPTV          🔧 Low Bandwidth Mode [Toggle]         │
├─────────────┬───────────────────────────────────────────────────────┤
│             │ ⚠️ LEGAL DISCLAIMER                                   │
│ 🌐 All      │ This application provides access to publicly          │
│   Channels  │ available free-to-air streams...                      │
│             ├───────────────────────────────────────────────────────┤
│ 🇵🇰 Pakistan │ ▶️ Now Playing: Select a channel to start watching   │
│             │                                                        │
│ 🇮🇳 India    │ ┌──────────────────────────────────────────────────┐ │
│             │ │                                                    │ │
│ 📰 News     │ │         Select a channel to start streaming        │ │
│             │ │              🎬 (Play Icon)                        │ │
│ 🎬 Entertain│ │                                                    │ │
│             │ └──────────────────────────────────────────────────┘ │
│ ⚽ Sports   │                                                        │
│             ├───────────────────────────────────────────────────────┤
│ 🌍 Global   │ 📺 All Channels                                       │
│             │                                                        │
│             │ ┌──────┐  ┌──────┐  ┌──────┐  ┌──────┐              │
│             │ │ GEO  │  │ ARY  │  │ PTV  │  │ BBC  │              │
│             │ │ News │  │ News │  │ News │  │ News │              │
│             │ │ 🇵🇰   │  │ 🇵🇰   │  │ 🇵🇰   │  │ 🌍   │              │
│             │ └──────┘  └──────┘  └──────┘  └──────┘              │
│             │                                                        │
│             │ ┌──────┐  ┌──────┐  ┌──────┐  ┌──────┐              │
│             │ │NDTV  │  │India │  │ Al   │  │NASA │              │
│             │ │24x7  │  │Today │  │Jazeera│ │ TV  │              │
│             │ │ 🇮🇳   │  │ 🇮🇳   │  │ 🌍   │  │ 🌍   │              │
│             │ └──────┘  └──────┘  └──────┘  └──────┘              │
└─────────────┴───────────────────────────────────────────────────────┘
│ © 2026 Global Free IPTV • Open-source • Optimized for 2G/3G        │
└─────────────────────────────────────────────────────────────────────┘
```

---

## 📱 Mobile View

### Portrait Mode
```
┌──────────────────────────┐
│ ☰  📺 Global Free IPTV   │
│            🔧 [Toggle]   │
├──────────────────────────┤
│ ⚠️ Legal Disclaimer      │
│ This app provides...     │
├──────────────────────────┤
│ ▶️ Select a channel      │
│                          │
│ ┌──────────────────────┐ │
│ │                      │ │
│ │   🎬                 │ │
│ │   Choose channel     │ │
│ │                      │ │
│ └──────────────────────┘ │
├──────────────────────────┤
│ 📺 All Channels          │
│                          │
│ ┌─────┐ ┌─────┐         │
│ │ GEO │ │ ARY │         │
│ │News │ │News │         │
│ │ 🇵🇰  │ │ 🇵🇰  │         │
│ └─────┘ └─────┘         │
│                          │
│ ┌─────┐ ┌─────┐         │
│ │ BBC │ │Al J │         │
│ │News │ │azeer│         │
│ │ 🌍  │ │ 🌍  │         │
│ └─────┘ └─────┘         │
└──────────────────────────┘
```

### Sidebar (Opened)
```
┌──────────────────────────┐
│ 📺 Global Free IPTV      │
├──────────────────────────┤
│ 🌐 All Channels          │
│ 🇵🇰 Pakistan             │
│ 🇮🇳 India                │
│ 📰 News                  │
│ 🎬 Entertainment         │
│ ⚽ Sports                │
│ 🌍 Global                │
└──────────────────────────┘
```

---

## 🎨 Color Scheme

### Dark Theme (Default)
```
Primary Background:   #1a1a2e ████████
Secondary Background: #16213e ████████
Accent Color:         #0f3460 ████████
Highlight Color:      #e94560 ████████
Text Color:           #ffffff ████████
Text Secondary:       #a0a0a0 ████████
```

---

## 🎬 Player States

### 1. Initial State (No Channel Selected)
```
┌────────────────────────────────────────┐
│ ▶️ Select a channel to start watching  │
│                                        │
│        ┌──────────────────┐            │
│        │                  │            │
│        │       🎬         │            │
│        │   (Play Icon)    │            │
│        │                  │            │
│        │  Choose a channel│            │
│        │  from below to   │            │
│        │  start streaming │            │
│        │                  │            │
│        └──────────────────┘            │
└────────────────────────────────────────┘
```

### 2. Loading State
```
┌────────────────────────────────────────┐
│ ▶️ Now Playing: Geo News               │
│                                        │
│        ┌──────────────────┐            │
│        │                  │            │
│        │    ⏳ Loading    │            │
│        │       ○○○        │            │
│        │   (Spinner)      │            │
│        │                  │            │
│        └──────────────────┘            │
│                                        │
│ 🔄 Connecting...                       │
└────────────────────────────────────────┘
```

### 3. Playing State
```
┌────────────────────────────────────────┐
│ ▶️ Now Playing: Al Jazeera English     │
│                                        │
│  ┌────────────────────────────────┐    │
│  │ [LIVE VIDEO STREAM]            │    │
│  │                                │    │
│  │  ▶️ ⏸️  ⏮️ ⏭️  🔊  ⚙️  ⛶      │    │
│  │  00:00 ━━━━━━━━━━━━━━━━ LIVE  │    │
│  └────────────────────────────────┘    │
└────────────────────────────────────────┘
```

### 4. Error State
```
┌────────────────────────────────────────┐
│ ▶️ Now Playing: PTV News               │
│                                        │
│        ┌──────────────────┐            │
│        │                  │            │
│        │       ⚠️         │            │
│        │  Connection Lost │            │
│        │                  │            │
│        │  Retrying (2/5)  │            │
│        │                  │            │
│        └──────────────────┘            │
│                                        │
│ 🔄 Network error. Retrying...          │
└────────────────────────────────────────┘
```

### 5. Low Bandwidth Mode
```
┌────────────────────────────────────────┐
│ ▶️ Now Playing: NDTV 24x7              │
│ 📶 Low Bandwidth Mode Active           │
│                                        │
│  ┌────────────────────────────────┐    │
│  │ [LIVE VIDEO STREAM]            │    │
│  │ (Lower Quality)                │    │
│  │                                │    │
│  │  ▶️ ⏸️  ⏮️ ⏭️  🔊  ⚙️  ⛶      │    │
│  └────────────────────────────────┘    │
│                                        │
│ 📊 Reduced quality for better playback │
└────────────────────────────────────────┘
```

---

## 🎯 Channel Card States

### Default State
```
┌───────────────┐
│   [LOGO]      │
│               │
│  Channel Name │
│   CATEGORY    │
└───────────────┘
```

### Hover State (Desktop)
```
┌───────────────┐ ← Elevated shadow
│   [LOGO]      │ ← Border highlight
│               │
│  Channel Name │
│   CATEGORY    │
└───────────────┘
```

### Active/Playing State
```
┌───────────────┐ ← Red border
│   [LOGO]      │
│     ▶️        │ ← Playing indicator
│  Channel Name │
│   CATEGORY    │
└───────────────┘
```

---

## 📊 Network Status Badge

### Normal Mode
```
┌──────────────────┐
│ 📶 Normal Mode   │
└──────────────────┘
  (Bottom-right corner)
```

### Low Bandwidth Mode
```
┌──────────────────┐
│ 📶 Low Bandwidth │
└──────────────────┘
  (Bottom-right, orange)
```

---

## 🎨 UI Elements

### Buttons

**Category Button (Inactive)**
```
┌──────────────────┐
│ 🌐 All Channels  │
└──────────────────┘
```

**Category Button (Active)**
```
┌──────────────────┐
│▐🌐 All Channels  │ ← Red border on left
└──────────────────┘
```

**Toggle Switch**
```
OFF: ◯────  │  ON: ────◉
```

---

## 📱 Responsive Breakpoints

### Desktop (1200px+)
- Sidebar visible
- 4 channel cards per row
- Large player

### Tablet (768px - 1199px)
- Sidebar visible
- 3 channel cards per row
- Medium player

### Mobile (< 768px)
- Sidebar hidden (hamburger menu)
- 2 channel cards per row
- Responsive player

---

## 🎬 Video Player Controls

```
┌────────────────────────────────────────┐
│                                        │
│         [VIDEO CONTENT AREA]           │
│                                        │
├────────────────────────────────────────┤
│ ▶️ ⏸️  ⏮️ ⏭️  🔊 ────○  ⚙️  ⛶       │
│ 00:00 ━━━━━━━━━━━━━━━━━━━━━━ LIVE   │
└────────────────────────────────────────┘

Legend:
▶️ Play      🔊 Volume     ⚙️ Settings
⏸️ Pause     ────○ Volume  ⛶ Fullscreen
⏮️ Previous   Slider
⏭️ Next
```

---

## 🎨 Animation States

### Loading Spinner
```
Frame 1: ○○○
Frame 2: ●○○
Frame 3: ○●○
Frame 4: ○○●
(Rotates continuously)
```

### Hover Effect
```
Normal:    [Card]
           
Hover:     [Card]  ← Moves up 5px
          (Shadow increases)
```

---

## 📐 Layout Grid

### Desktop Channel Grid
```
┌────┬────┬────┬────┐
│CH 1│CH 2│CH 3│CH 4│
├────┼────┼────┼────┤
│CH 5│CH 6│CH 7│CH 8│
├────┼────┼────┼────┤
│CH 9│CH10│CH11│CH12│
└────┴────┴────┴────┘
```

### Mobile Channel Grid
```
┌────┬────┐
│CH 1│CH 2│
├────┼────┤
│CH 3│CH 4│
├────┼────┤
│CH 5│CH 6│
└────┴────┘
```

---

## 🎯 Key Features Visualization

### Category Filtering
```
All → Pakistan → India → News → Entertainment → Sports → Global
 ✓      ○         ○       ○          ○           ○        ○

[Displays only selected category channels]
```

### Low Bandwidth Toggle
```
Normal Mode:        Low Bandwidth Mode:
- Full quality      - Reduced quality
- High buffer       - Low buffer
- 5 Mbps+          - 128 Kbps+
```

---

## 📊 User Flow Diagram

```
1. Open App
    ↓
2. View Disclaimer
    ↓
3. Browse Categories ──→ Filter Channels
    ↓                        ↓
4. Select Channel    ←──────┘
    ↓
5. Player Loads
    ↓
6. Stream Plays → [If Error] → Retry Logic
    ↓                              ↓
7. Watch TV                    Try Again
    ↓                              ↓
8. Switch Channel? ──Yes──→ Back to Step 4
         ↓
        No
         ↓
    Continue Watching
```

---

## 🎨 Accessibility Features

### Visual Indicators
- ✅ High contrast colors
- ✅ Clear focus states
- ✅ Icon + text labels
- ✅ Loading spinners
- ✅ Error messages

### Keyboard Navigation
- Tab: Navigate elements
- Space: Play/Pause
- Arrow keys: Volume/seek
- F: Fullscreen
- Esc: Exit fullscreen

---

## 📷 Taking Screenshots

### For Contributors

**To add actual screenshots:**

1. Take screenshots on different devices:
   - Desktop (Chrome, 1920x1080)
   - Tablet (iPad, 1024x768)
   - Mobile (iPhone, 375x667)

2. Name files:
   - `desktop-home.png`
   - `desktop-playing.png`
   - `mobile-home.png`
   - `mobile-playing.png`
   - `tablet-view.png`

3. Add to `/screenshots` folder

4. Update this document with real images:
   ```markdown
   ![Desktop View](screenshots/desktop-home.png)
   ```

---

## 🎨 Branding Guidelines

### Logo Usage
- Icon: 📺 (TV emoji)
- Name: "Global Free IPTV"
- Colors: See color scheme above

### Typography
- Font: Segoe UI (system font)
- Headings: Bold
- Body: Regular

---

**Note**: This is a text-based mockup. Actual screenshots will be added as the project grows. Contributors are welcome to add real screenshots!

---

**For actual screenshots, visit the live demo or run locally!**
