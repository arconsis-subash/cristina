# Cristina & Subash — Our Timeline

A beautiful, scrollable timeline webpage with a nature-inspired branch and leaf design. Based on the original romantic timeline design with pink color scheme.

## Features

✨ **Responsive Design** - Works on desktop, tablet, and mobile
💕 **Romantic Pink Theme** - Inspired by the original Cristina & Subash timeline
🌳 **Branch Visualization** - Central timeline branch with alternating event cards
📸 **Image Integration** - Each event displays its associated photo
🎨 **Color-Customizable** - Each event has its own color
💾 **Browser Storage** - Events persist using localStorage
📱 **Hover Effects** - Cards lift up when you hover over them
🔍 **Modal View** - Click photos to view them larger

## Project Structure

```
timeline/
├── index.html          # Main HTML file
├── data/timeline.json  # Timeline data (NOT used in current version)
└── images/
    └── (add your images here)
```

## Getting Started

### 1. Add Images
Place your images in the `images/` folder:
```
timeline/images/
├── event1.jpg
├── event2.jpg
├── event3.jpg
├── event4.jpg
├── event5.jpg
└── event6.jpg
```

### 2. Edit Events in JavaScript
Open `index.html` and modify the `initialEvents` array in the script section:

```javascript
const initialEvents = [
    {
        date: '2024-11-20', 
        title: 'Event Title', 
        text: 'Event description...',
        photo: null, // Will use placeholder until you add image path
        color: '#ffb6c1'
    }
];
```

**Fields:**
- `date` - ISO format date (YYYY-MM-DD)
- `title` - Event title
- `text` - Event description/message
- `photo` - Path to image or null for placeholder
- `color` - Hex color code for placeholder SVG

### 3. View the Timeline
Open `index.html` in your browser or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (with http-server)
http-server
```

Then navigate to: `http://localhost:8000/timeline/`

## Features in Detail

### Events
- Automatically sorted by date
- Alternate left/right layout on desktop
- Stack vertically on mobile
- Click on any photo to view it in a modal

### localStorage
- All events are saved to browser storage
- Events persist even after closing the browser
- Use the browser console to access: `localStorage.getItem('cristina_timeline_events')`

### Color Scheme
The default pink romantic theme uses these CSS variables:
```css
--bg: #fff5f8;
--accent: #ff6b9f;
--muted: #6b6b6b;
--branch: linear-gradient(180deg, #ff9bbf, #ff6b9f);
```

Modify the `:root` section in the `<style>` tag to customize colors.

## Browser Support
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

## Tips
- Add real photos by replacing `photo: null` with `photo: './images/your-image.jpg'`
- Colors are used for placeholder SVG backgrounds
- Edit dates to sort events chronologically
- Use descriptive titles and messages for better storytelling

---

**Based on the original timeline.html** — Enhanced with cleaner styling and localStorage support. 💕
