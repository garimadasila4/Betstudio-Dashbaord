# Betstudio Dashboard

A dark-themed backoffice dashboard built with HTML, CSS, and JavaScript.

## How to Run

### Option 1: Simple File Open (Quickest)
1. Navigate to the `public` folder
2. Double-click `index.html` to open it in your default browser
3. Or right-click and select "Open with" → choose your preferred browser

### Option 2: Using Python HTTP Server (Recommended)
If you have Python installed:

```bash
# Navigate to the public directory
cd public

# Python 3
python3 -m http.server 8000

# Or Python 2
python -m SimpleHTTPServer 8000
```

Then open your browser and go to: `http://localhost:8000`

### Option 3: Using Node.js http-server
If you have Node.js installed:

```bash
# Install http-server globally (one-time)
npm install -g http-server

# Navigate to the public directory
cd public

# Start the server
http-server -p 8000
```

Then open your browser and go to: `http://localhost:8000`

### Option 4: Using VS Code Live Server
1. Install the "Live Server" extension in VS Code
2. Right-click on `index.html` in the file explorer
3. Select "Open with Live Server"
4. The page will automatically open in your browser

### Option 5: Using PHP Built-in Server
If you have PHP installed:

```bash
# Navigate to the public directory
cd public

# Start the server
php -S localhost:8000
```

Then open your browser and go to: `http://localhost:8000`

## Features

- Dark theme dashboard
- Responsive sidebar navigation
- Interactive charts (GGR and NGR)
- Statistics cards with KPIs
- Revenue breakdown tables
- Filter and date picker functionality

## Browser Compatibility

Works best in modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)

## Dependencies

All dependencies are loaded via CDN:
- Tailwind CSS (via CDN)
- Chart.js (via CDN)
- Google Fonts (Inter)

No build process or npm install required!

