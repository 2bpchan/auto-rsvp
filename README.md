# _rvsp_ - The Better Way to Read

<div align="center">

![RSVP Speed Reading](https://img.shields.io/badge/Speed%20Reading-RSVP-red?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![Version](https://img.shields.io/badge/Version-1.0.0-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

**Experience reading at the speed of thought with advanced RSVP technology**

[Live Demo](https://eeman1113.github.io/_rvsp_/) • [Documentation](#features) • [Report Bug](#contributing) • [Request Feature](#contributing)

</div>

---

## Table of Contents

- [About](#about)
- [Key Features](#key-features)
- [Demo](#demo)
- [How RSVP Works](#how-rsvp-works)
- [Getting Started](#getting-started)
- [Usage Guide](#usage-guide)
- [Loading Text via URL](#loading-text-via-url)
- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Technology Stack](#technology-stack)
- [Browser Compatibility](#browser-compatibility)
- [Performance](#performance)
- [Contributing](#contributing)
- [Author](#author)
- [License](#license)
- [Acknowledgments](#acknowledgments)
- [Roadmap](#roadmap)

---

## About

**_rvsp_** is a cutting-edge web-based speed reading application that leverages **Rapid Serial Visual Presentation (RSVP)** technology to help users read faster, comprehend better, and eliminate eye strain. Built with modern web technologies, _rvsp_ offers a minimalist, distraction-free reading experience that can boost your reading speed by up to 3x.

Unlike traditional reading where your eyes move across lines of text, _rvsp_ presents words one at a time at your desired speed, eliminating the need for eye movement and reducing cognitive load. This scientifically-proven technique is used by speed readers worldwide to process information more efficiently.

### Why Choose _rvsp_?

- **Read 3x Faster** - Increase reading speed from 200-300 WPM to 600-1000+ WPM
- **Improved Focus** - Single-word display eliminates distractions
- **Reduced Eye Strain** - No eye movement means less fatigue
- **Better Retention** - Optimal Recognition Point (ORP) algorithm maximizes comprehension
- **Beautiful Interface** - Sleek, modern dark mode design
- **Built-in Library** - Save and organize your reading materials
- **Progress Tracking** - Resume exactly where you left off
- **100% Free** - No subscriptions, no ads, no tracking

---

## Key Features

### Core Reading Features
- **Advanced RSVP Engine** - Scientifically optimized word presentation
- **Optimal Recognition Point (ORP)** - Intelligent character-level focus highlighting
- **Adjustable Reading Speed** - 100-1000 WPM with 10 WPM increments
- **Adaptive Pacing** - Automatic delay adjustments for punctuation, long words, and words containing non-letter characters (hyphens, slashes, digits) — the slowdown percentage is configurable in Settings
- **Smart Word Fitting** - Long hyphenated words and file paths shrink to fit on screen instead of getting clipped, without moving the focus letter
- **Real-time Speed Control** - Adjust WPM on the fly without interrupting reading

### Content Management
- **Personal Library System** - Save unlimited articles, books, and notes
- **Smart Bookmarking** - Save your position in any document
- **Progress Tracking** - Visual progress bars show completion percentage
- **Quick Resume** - Pick up exactly where you left off
- **Title Management** - Organize content with custom titles
- **Load via URL** - Populate the reader directly from a link (see [Loading Text via URL](#loading-text-via-url))

### User Experience
- **Minimal Dark Interface** - Eye-friendly design for extended reading sessions
- **Responsive Design** - Optimized for desktop, tablet, and mobile devices
- **Focus Guides** - Visual alignment aids for centered fixation
- **Smooth Animations** - Polished transitions and micro-interactions
- **Zero Distractions** - Fullscreen reading mode
- **Themes & Fonts** - 10 built-in color themes and 4 font choices
- **Word Size** - Adjustable text size (50-200%) in Settings

### Power User Tools
- **Comprehensive Keyboard Shortcuts** - Complete keyboard navigation
- **Seekable Progress Bar** - Jump to any position with a click
- **Quick Skip Controls** - Jump forward/backward by 10 words, or one word at a time
- **Speed Presets** - Quickly adjust reading speed with +/- controls
- **Demo Content** - Built-in example text to test the app

### Technical Features
- **Pure Client-Side** - No server required, 100% privacy
- **LocalStorage Integration** - Persistent data without databases
- **Lightweight** - Fast loading, minimal dependencies

---

## Demo

**Try it now:** [eeman1113.github.io/_rvsp_/](https://eeman1113.github.io/_rvsp_/)

### Quick Start Demo
1. Click "Load Demo" to try sample text
2. Adjust speed to your comfort level (start at 250-300 WPM)
3. Click "Start Reading" or press `Space`
4. Watch words appear one at a time in the center
5. Gradually increase speed as you get comfortable

---

## How RSVP Works

### The Science Behind Speed Reading

**Rapid Serial Visual Presentation (RSVP)** is a scientific approach to reading that eliminates the two main bottlenecks in traditional reading:

1. **Eye Movement (Saccades)** - In normal reading, your eyes jump from word to word. Each jump takes 200-250ms, accounting for up to 90% of reading time. RSVP eliminates this by presenting words in one location.

2. **Regression** - Readers often re-read words or phrases. RSVP's controlled pacing prevents regression while maintaining comprehension.

### The Optimal Recognition Point (ORP)

_rvsp_ implements an intelligent ORP algorithm that highlights the optimal character in each word:

```
Normal word:    "reading"
With ORP:       "rea[d]ing"
                     ↑
              Focus point
```

This allows your brain to process words more efficiently, as research shows we recognize words faster when our gaze is fixed slightly left of center.

### Reading Speed Guidelines

| Speed (WPM) | Proficiency Level | Best For |
|-------------|------------------|----------|
| 100-200 | Beginner | Learning the technique |
| 200-300 | Casual Reader | Articles, emails |
| 300-450 | Intermediate | Books, long-form content |
| 450-600 | Advanced | Technical documents |
| 600-800 | Expert | News, familiar topics |
| 800-1000+ | Power User | Skimming, reviews |

---

## Getting Started

### Online Version (Recommended)

Simply visit **[eeman1113.github.io/_rvsp_/](https://eeman1113.github.io/_rvsp_/)** in any modern web browser. No installation required!

### Local Installation

1. **Clone the repository**
```bash
git clone https://github.com/eeman1113/_rvsp_.git
cd _rvsp_
```

2. **Open in browser**
```bash
# Simply open the index.html file
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

3. **Or use a local server**
```bash
# Python 3
python -m http.server 8000

# Node.js (with http-server)
npx http-server

# PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

### Requirements

- Modern web browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- JavaScript enabled
- ~500KB of disk space for caching
- LocalStorage support for library features

---

## Usage Guide

### Basic Reading Workflow

1. **Add Content**
   - Paste any text into the input area
   - Add an optional title for organization
   - Click "Start Reading" or save to library

2. **Control Playback**
   - `Space` or click screen to play/pause
   - Use speed controls to adjust WPM
   - Seek forward/backward with arrow buttons

3. **Save Progress**
   - Click "Save to Library" to store content
   - Use the bookmark button to save position
   - Resume anytime from your library

### Advanced Tips

**Finding Your Optimal Speed**
1. Start at 250 WPM for comfort
2. Read for 2-3 minutes
3. If comfortable, increase by 50 WPM
4. Find the sweet spot between speed and comprehension
5. Different content types may need different speeds

**Maximizing Comprehension**
- Take breaks every 15-20 minutes
- Use lower speeds for complex or technical content
- Let punctuation pauses guide your rhythm
- Re-read important sections at slower speeds
- Practice regularly to build skill

**Library Organization**
- Use descriptive titles for easy identification
- Review progress bars to track completion
- Delete finished items to keep library clean

---

## Loading Text via URL

_rvsp_ can be pre-loaded with content directly from a link, which is useful for bookmarklets, share links, or feeding it text from another tool.

### Format

```
https://your-site/index.html#text=<URL-encoded text>&title=<URL-encoded title (optional)>
```

- **`text`** (required) - The content to load, URL-encoded (e.g. `encodeURIComponent(...)` in JavaScript).
- **`title`** (optional) - A title for the content, also URL-encoded.

The hash fragment (`#`) is used rather than a query string (`?`) because fragments are never sent to the server, so they aren't subject to the request-line length limits (commonly ~8KB) most web servers enforce on query strings. This lets you pass in very long text. A `?text=...&title=...` query string is also supported as a fallback.

### Example

```js
const url = `https://your-site/index.html#text=${encodeURIComponent(myText)}&title=${encodeURIComponent(myTitle)}`;
```

When the page loads, it reads these parameters, fills in the text and title fields, and then removes them from the address bar so the (potentially large) parameter doesn't linger in the URL or browser history.

---

## Keyboard Shortcuts

Master these shortcuts for a seamless reading experience:

| Shortcut | Action |
|----------|--------|
| `Space` | Play / Pause |
| `↑` | Increase speed (+10 WPM) |
| `↓` | Decrease speed (-10 WPM) |
| `←` | Skip backward 10 words |
| `→` | Skip forward 10 words |
| `<` | Previous word |
| `>` | Next word |
| `B` | Save bookmark |
| `Esc` | Exit reader mode |

> **Tip:** Use keyboard shortcuts for distraction-free reading without touching the mouse!

---

## Technology Stack

_rvsp_ is built with modern, performant web technologies:

### Frontend
- **HTML5** - Semantic markup with rich metadata
- **CSS3** - Custom properties, animations, and responsive design
- **Vanilla JavaScript (ES6+)** - Pure JS, no framework overhead
- **Tailwind CSS** - Utility-first styling via CDN
- **Lucide Icons** - Beautiful, consistent iconography

### Typography
- **Inter** - Clean, readable UI font
- **JetBrains Mono** - Monospace font for code-like elements
- **Merriweather** - Serif option for longer-form reading

### Browser APIs
- **LocalStorage API** - Persistent data storage
- **DOM Manipulation** - Efficient rendering
- **CustomEvent API** - Event-driven architecture

### Design Principles
- **Mobile-First** - Responsive design from the ground up
- **Performance-First** - Optimized rendering and minimal reflows
- **Accessibility** - Semantic HTML and keyboard navigation

### Performance Optimizations
- **Zero Dependencies** - All libraries loaded from CDN
- **Lazy Icon Loading** - Icons created on demand
- **Efficient Timers** - Optimized word presentation timing
- **CSS-based Animations** - Hardware-accelerated transforms

---

## Browser Compatibility

| Browser | Minimum Version | Status |
|---------|----------------|--------|
| Chrome | 90+ | Fully Supported |
| Firefox | 88+ | Fully Supported |
| Safari | 14+ | Fully Supported |
| Edge | 90+ | Fully Supported |
| Opera | 76+ | Fully Supported |
| Samsung Internet | 14+ | Supported |

**Mobile Browsers:** Fully responsive and optimized for iOS Safari and Chrome Android.

---

## Performance

- **Load Time:** <500ms on 3G connection
- **First Contentful Paint:** <200ms
- **Time to Interactive:** <500ms
- **Bundle Size:** ~40KB (uncompressed HTML)
- **Memory Usage:** <5MB typical
- **Rendering:** 60 FPS smooth animations

---

## Contributing

Contributions are welcome! Here's how you can help improve _rvsp_:

### Ways to Contribute
- Report bugs and issues
- Suggest new features
- Improve documentation
- Enhance UI/UX design
- Write tests
- Optimize performance

### Development Setup

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Make your changes
4. Test thoroughly in multiple browsers
5. Commit your changes (`git commit -m 'Add AmazingFeature'`)
6. Push to the branch (`git push origin feature/AmazingFeature`)
7. Open a Pull Request

### Coding Standards
- Use ES6+ JavaScript features
- Follow existing code style and formatting
- Comment complex logic
- Test on Chrome, Firefox, and Safari
- Ensure mobile responsiveness

### Feature Requests
Have an idea? [Open an issue](https://github.com/eeman1113/_rvsp_/issues) with the label `enhancement` and describe:
- The problem you're trying to solve
- Your proposed solution
- Any alternative solutions considered
- Additional context or screenshots

---

## Author

**Eeman Majumder**

- GitHub: [@eeman1113](https://github.com/eeman1113)
- Website: [eeman1113.github.io/_rvsp_/](https://eeman1113.github.io/_rvsp_/)

---

## License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

### MIT License Summary
- Commercial use
- Modification
- Distribution
- Private use
- No liability
- No warranty

---

## Acknowledgments

- **RSVP Research** - Based on cognitive science research in rapid reading
- **Tailwind CSS** - For the excellent utility-first CSS framework
- **Lucide Icons** - For beautiful, consistent icons
- **Google Fonts** - For Inter, JetBrains Mono, and Merriweather typefaces

---

## Roadmap

A short list of possible future improvements:

- [ ] Export/import library as a JSON backup
- [ ] Reading stats (words read, time spent, WPM history)
- [ ] Font size control
- [ ] PWA support (manifest + service worker)
