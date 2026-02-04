# 2M Motors LLC

A luxury used car dealership website. Static HTML/CSS/JS with dynamic vehicle inventory from a single data source.

## Features

- Dynamic vehicle inventory loaded from `vehicles-data.js`
- Responsive slider/carousel on home page
- Individual vehicle detail pages
- Mobile-friendly design
- No server or build tools required

## Files

- `index.html` — Home page with featured inventory slider
- `vehicle.html` — Vehicle detail page (loads data via URL query `?id=...`)
- `vehicles-data.js` — Single source of truth for all vehicle data
- `style.css` — Responsive styles

## Adding Vehicles

Edit `vehicles-data.js` and add new entries to the `window.VEHICLES` object:

```javascript
"vehicle-id": {
    "title": "Year Make Model",
    "price": "$XX,XXX",
    "mileage": "XX,XXX miles",
    "engine": "Engine specs",
    "transmission": "Type",
    "drivetrain": "Type",
    "exterior": "Color",
    "interior": "Material",
    "images": ["URL1", "URL2", "URL3"],
    "features": ["Feature 1", "Feature 2"],
    "description": "Vehicle description."
}
```

Then update `index.html` inventory links to include the new ID:

```html
<a href="vehicle.html?id=vehicle-id" class="btn-small">View Details</a>
```

## Viewing Locally

Open `index.html` directly in your browser via `file://` — no server required.

## Contact

2M Motors LLC  
5532 NW Beaver Dr  
Johnston, IA 50131  
(515) 770-7883  
Hours: Mon–Sat: 9 AM – 6 PM
