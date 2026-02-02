# Dev Dashboard ⚡

A beautiful, dark-themed developer dashboard built as a single HTML file.

![Dashboard Preview](https://img.shields.io/badge/status-active-brightgreen)

## Features

- 🕐 **Live Clock & Date** - Always know what time it is
- 👋 **Smart Greeting** - Changes based on time of day
- 💻 **System Stats** - CPU, RAM, Disk, Uptime (simulated)
- 🌤️ **Weather** - Real weather data from wttr.in
- 📊 **Git Activity** - Recent commits at a glance
- ✅ **Todo List** - Persistent task tracking with localStorage
- 🔗 **Quick Links** - Fast access to your tools
- 💡 **Dev Quotes** - Random programming wisdom

## Usage

Just open `index.html` in your browser!

Or serve it locally:
```bash
# Python
python -m http.server 3000

# Node.js
npx serve .

# Or just double-click index.html
```

## Customization

### Quick Links
Edit the `links-grid` section in index.html to add your own links:
```html
<a href="YOUR_URL" class="quick-link" target="_blank">
  <span class="link-icon">📦</span>
  <span class="link-text">Your Link</span>
</a>
```

### Weather Location
Change the location in the `fetchWeather()` function:
```javascript
const response = await fetch('https://wttr.in/YOUR_CITY?format=j1');
```

### System Stats
For real system stats, you'd need a backend API. The current implementation simulates values.

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge).

## License

MIT - Do whatever you want with it!

---

Built with ❤️ by Turbo
