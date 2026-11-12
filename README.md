# ScannerQRC — Browser QR Code Generator

A lightweight browser project that converts a website URL into a downloadable QR code. Despite the repository's historical name, the implemented app is a **QR generator**, not a camera-based QR scanner.

![QR code generator screenshot](img/screen.png)

## How it works

1. Enter a valid web URL.
2. Choose a QR image size between 100×100 and 700×700 pixels.
3. Select **Generate QR Code** to render a QR code in the browser.
4. Use the available download action to save the generated image.

## Tech stack

- HTML, vanilla JavaScript and CSS
- Tailwind CSS through a CDN
- QRCode.js for client-side QR rendering
- Poppins via Google Fonts

## Run locally

Clone the repository and open `index.html` in a browser. A local static server is recommended for consistent asset handling:

```bash
python -m http.server 5500
```

Visit `http://localhost:5500`. Internet connectivity is required to load the CDN-hosted dependencies unless you vendor them locally.

## Repository map

- `index.html` — form, markup and visual layout
- `js/script.js` — QR generation and interaction logic
- `img/` — starter illustration and screenshot

## Scope

This is a small, educational client-side utility. It has no login, account storage or backend QR history. Only generate QR codes for destinations you trust and check the destination before sharing.

Maintained as a portfolio project by [JohnBarsisa](https://github.com/JohnBarsisa).
