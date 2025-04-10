# Static HTML Implementation

This directory contains a framework-free, static HTML implementation of the UI components with JavaScript data loading. This version is ideal for quickly integrating the dashboard into existing projects or for developers who prefer vanilla JavaScript.

## Features

- **Pure HTML, CSS, and JavaScript**: No framework dependencies
- **Tailwind CSS**: Fully styled with responsive design

## Structure

- `dashboard.html` - The main dashboard UI

## Getting Started

### Quick Start

The easiest way to run the static implementation:

1. Make sure the `sample-data` directory (at the repository root) contains the JSON files
2. Start a local web server in this directory
3. Access the implementation in your browser

### Local Development Options

#### Option 1: Python HTTP Server

```bash
cd static-html
python -m http.server 5000
```

Then open [http://localhost:5000](http://localhost:5000) in your browser.

#### Option 2: Node.js HTTP Server

```bash
cd static-html
npx http-server -p 5000
```

Then open [http://localhost:5000](http://localhost:5000) in your browser.

#### Option 3: Docker (Recommended)

From the repository root:

```bash
docker-compose up static-html
```

Then open [http://localhost:5000](http://localhost:5000) in your browser.

## Customizing the Implementation

### Modifying the UI

The HTML structure in `dashboard.html` uses Tailwind CSS classes for styling. You can modify the appearance by changing these classes or adding your own CSS.

```html
<!-- Example of customizing a card -->
<div class="bg-white rounded-lg shadow p-6 border-l-4 border-blue-500">
  <!-- Card content -->
</div>
```
## Browser Compatibility

This implementation is compatible with all modern browsers (Chrome, Firefox, Safari, Edge). For older browsers, you may need to add polyfills for features like `async/await` and `fetch`.
