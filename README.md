# 🎯 Screener Scalping

> IHSG Intraday Stock Screener — Real-time top gainer scanner with persistent history tracking for scalping strategies.

![Version](https://img.shields.io/badge/version-3.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)

---

## ✨ Features

### 📊 Real-Time Scanning
- Paste data from **CIAJENG Bot** / Telegram directly
- Auto-sync timestamp (`HH:mm`) with live clock
- Manual lock mode for precise time entry

### 🏛️ Three-Table Dashboard
| Table | Description |
|-------|-------------|
| **Current Scan** | Latest paste data with `FirstSeen` timestamp |
| **Persistent** | Stocks that keep appearing across scans — with flashing count badge |
| **Dropped Out** | Stocks that vanished from the latest scan |

### 🆕 New Stock Detection
- Green-highlighted rows for first-time appearances
- Dedicated "🆕 Baru" filter

### ⚡ Flashing Count Badge
- `1x` → slow pulse | `5x+` → rapid flash
- Visual intensity increases with persistence count

### 🎨 Dual Theme
- **Night** (dark terminal aesthetic)
- **Light** (clean daytime mode)

### 🔍 Smart Filtering
- Filter by symbols: ⭐ * + $ #
- Filter by score: 5 ideal / ≥4
- Filter by change: positive only
- Filter by new stocks

### 🔄 Multi-Sort
- Click column headers to add sort priority (max 4)
- Click chips to reverse direction
- Remove sorts individually

---

## 🚀 Quick Start

1. **Open** `screener_scalping_v3.html` in any modern browser
2. **Paste** data from CIAJENG Bot into the textarea
3. **Press Enter** or click **▶ PROSES DATA**
4. **Watch** the dashboard populate across 3 tables

### Sample Data Format
```
🍬 Top gainer IHSG (proc18)
Ticker Current    %  valM vv1 chg
  MIDI    322     2%   10   5  -4⭐
  OMED    250     2%    6   1  -1    #
  BANK    505     2%    1   3  -2 *
  ...
```

### Symbol Legend
| Symbol | Meaning |
|--------|---------|
| ⭐ | Frekuensi / Bintang spike |
| * | Daily open = low (1 week) |
| + | Weekly open = low (2 weeks) |
| $ | Kamehameha hourly signal |
| # | Kamehameha 15min signal |

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Enter` (in textarea) | Process data |
| `Enter` (in time input) | Process data |
| Click 🔓/🔒 | Toggle auto/manual time |

---

## 📁 File Structure

```
.
├── screener_scalping_v3.html    # Main application (single file)
├── .gitignore                   # Git ignore rules
└── README.md                    # This file
```

> **Zero dependencies.** Pure HTML/CSS/JS. No build step required.

---

## 🧠 Scoring System

| Criteria | Points |
|----------|--------|
| ⭐ Bintang | +1.5 |
| * Daily Low | +0.5 |
| + Weekly Low | +0.5 |
| $ Kamehameha H | +0.5 |
| # Kamehameha 15 | +0.5 |
| Chg Positive | +0.5 |
| Chg ≥ 5 | +0.5 |

**Max Score: 5** (ideal setup for scalping entry)

---

## 🌙 Theme Switching

Click the colored dots in the header:
- 🔵 Night (default)
- 🟣 Light

Preference saved to `localStorage`.

---

## ⚠️ Notes

- **Session-based history**: Data persists during browser session. Refreshing clears history (by design for daily use).
- **No server required**: Runs entirely client-side.
- **Browser support**: Chrome, Firefox, Safari, Edge (latest versions).

---

## 📝 Changelog

### v3.0 — Intraday History
- Added 3-table dashboard (Current / Persistent / Dropped)
- Flashing count badges for persistence tracking
- New stock detection with green highlight
- Auto/manual timestamp with lock toggle

### v2.x — Top Gainer Parser
- Support for 🍬 Top Gainer IHSG format
- Separate symbol columns (⭐ * + $ #)

### v1.x — SUPERKETAT
- Original MA-based stock screener

---

## 📜 License

MIT License — feel free to use, modify, and share.

---

Built with 💚 for the Indonesian trading community.
