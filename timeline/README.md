# Timeline Leaf Design Project

A beautiful, scrollable timeline webpage with a nature-inspired branch and leaf design.

## Project Structure

```
timeline/
├── index.html          # Main HTML file
├── data/
│   └── timeline.json   # Timeline data (events, descriptions, colors, image names)
└── images/
    └── (add your images here)
```

## Features

✨ **Responsive Design** - Works on desktop, tablet, and mobile
🍃 **Animated Leaves** - Each event has a swaying leaf marker
🌳 **Branch Visualization** - Central timeline branch with alternating event cards
🎨 **Color Customization** - Each event has its own color in the JSON
📸 **Image Integration** - Each event can display an associated image

## Getting Started

### 1. Add Images
Place your images in the `images/` folder:
```
timeline/images/
├── event1.jpg
├── event2.jpg
├── event3.jpg
├── event4.jpg
└── event5.jpg
```

### 2. Update Timeline Data
Edit `data/timeline.json` to add more events:

```json
{
  "timeline": [
    {
      "id": 1,
      "year": "2020",
      "title": "Event Title",
      "description": "Event description...",
      "image": "event1.jpg",
      "color": "#FF6B6B"
    }
  ]
}
```

**Fields:**
- `id` - Unique identifier
- `year` - Year or date
- `title` - Event title
- `description` - Event description
- `image` - Image filename (must exist in images/ folder)
- `color` - Hex color code for the leaf and accent

### 3. View the Timeline
Open `index.html` in your browser or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (with http-server)
http-server
```

Then navigate to: `http://localhost:8000/timeline/`

## Customization

### Color Palette
Modify the background gradient in `index.html`:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Branch Color
Change the timeline branch color:
```css
background: linear-gradient(180deg, #2ecc71 0%, #27ae60 100%);
```

### Typography
Adjust fonts and sizes in the CSS section

## Browser Support
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

---

**Ready to add your events!** Update the JSON and add images to get started. 🌿
