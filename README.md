# Credits Generator

A web-based tool to create beautiful scrolling credits for your productions. Perfect for theater shows, school plays, livestreams, and video productions!

**Live Demo:** [https://whyisjake.github.io/credits/](https://whyisjake.github.io/credits/)

## Features

- 🎬 **Two Scrolling Styles**
  - Classic Vertical Scroll - Traditional upward scrolling credits
  - Star Wars Crawl - Iconic 3D perspective effect with animated starfield

- 🎨 **Full Customization**
  - Custom background colors
  - Custom title colors
  - Custom text colors
  - Adjustable scroll speed
  - Production title

- ➕ **Dynamic Content**
  - Add unlimited cast members
  - Add unlimited crew members
  - Add acknowledgements and special thanks
  - Easy add/remove interface

- 💾 **Save & Load**
  - Save your progress locally
  - Load saved credits anytime
  - No account needed (uses browser localStorage)

- 📺 **OBS Ready**
  - Perfect for streaming
  - Works as Browser Source
  - Auto-restarts when scene becomes active
  - Manual restart with 'R' key

## Usage

### Online (Recommended)

1. Visit [https://whyisjake.github.io/credits/](https://whyisjake.github.io/credits/)
2. Fill in your production details
3. Choose your style (Classic or Star Wars)
4. Customize colors and speed
5. Add cast and crew members
6. Click "Generate Credits"

### Local Installation

1. Clone or download this repository
2. Open `index.html` in your web browser
3. No build process or dependencies required!

## Using with OBS

### Method 1: Use the Live URL (Requires Internet)

1. In OBS, add a new **Browser Source**
2. Uncheck "Local file"
3. Set URL to: `https://whyisjake.github.io/credits/player.html`
4. Set Width: 1920, Height: 1080 (or your stream resolution)
5. Check "Refresh browser when scene becomes active"
6. Click OK

**Note:** Generate your credits first from the main page, then the player will load them from localStorage.

### Method 2: Use Local Files (No Internet Required)

1. Download or clone this repository
2. In OBS, add a new **Browser Source**
3. Check "Local file"
4. Browse to `player.html` in your downloaded folder
5. Set Width: 1920, Height: 1080
6. Check "Refresh browser when scene becomes active"
7. Click OK

### Controls

- Press **R** to restart credits
- Credits auto-restart when animation completes
- Credits auto-restart when switching back to the scene (if "Refresh browser when scene becomes active" is enabled)

## Customization Options

### Credits Style
- **Classic Scroll** - Traditional vertical scrolling, good for formal productions
- **Star Wars Crawl** - 3D perspective with starfield background, great for sci-fi or fun productions

### Colors
- **Background Color** - Main background (not used in Star Wars style, which uses starfield)
- **Title Color** - Color for section headers (Cast, Crew, etc.)
- **Text Color** - Color for names and roles

### Speed
- Adjustable from 30-600 seconds
- Recommended: 240 seconds (4 minutes)
- Higher number = slower scroll

## Tips

- **Classic Scroll**: Works great for traditional theater productions with standard black background
- **Star Wars Crawl**: Requires larger font sizes due to perspective - these are automatically applied
- **Speed**: Test your timing - allow about 3-4 seconds per cast/crew entry
- **Colors**: High contrast works best (white text on black, or maroon titles on black)
- **Save Often**: Use "Save Progress" regularly to avoid losing your work
- **Preview**: Generate and test before your production to ensure timing is right

## Browser Compatibility

Works in all modern browsers:
- Chrome/Edge (Recommended for OBS)
- Firefox
- Safari
- Opera

## Technical Details

- Pure HTML, CSS, and JavaScript
- No frameworks or dependencies
- Uses CSS animations and 3D transforms
- Canvas-based starfield for Star Wars style
- localStorage for data persistence
- Responsive design

## Project Structure

```
.
├── index.html          # Main credits generator interface
├── player.html         # Credits player/display
├── credits.html        # Original single-file version
└── README.md          # This file
```

## Credits

Created for theater productions, livestreams, and video projects.

Originally built for a school production of Romeo and Juliet.

## License

Free to use for any purpose. No attribution required, but appreciated!

---

**Need help?** Open an issue on GitHub or visit the live demo for examples.
