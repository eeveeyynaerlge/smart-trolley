# Smart Trolley functional prototype

A standalone, retailer-neutral interactive web prototype for a smart shopping trolley. It is a front-end demonstration only: no real payment, camera, scale, account, email, or location services are connected.

## Open it

Open `smart-trolley-concept.html` in a modern browser. No installation, internet connection, server, or build process is required.

For a local web server (useful when testing browser permissions), serve the `outputs` folder with any static-file server and open the page in Chromium, Edge, or Chrome.

## What is interactive

- Light and dark modes, with dark-accent blue button borders.
- Live basket quantities, item totals, savings, and receipt total.
- Simulated camera scan that adds an item.
- Per-item camera, barcode, and scale detection details.
- Apple camera/scale mismatch that must be resolved before payment.
- Route-mode selection and progress through store stops.
- Offer application that adds an item, adjusts savings, and changes the selected route.
- Shared-basket demonstration, including a second shopper adding bananas.
- Session-only parking-space saving and a route back to the car.
- Low-battery demonstration; **Reset demo** restores normal charge (84%).
- Simulated payment, receipt copy/email actions, basket verification, exit pass, and exit-gate scan.
- New-session reset.

## Suggested demo flow

1. Open **Basket** and select **Simulate camera scan** or amend quantities.
2. Resolve the apple mismatch by confirming three apples.
3. Open **Offers** and add the pasta-sauce offer.
4. Optionally connect a shopper from **Home** and advance the route from **Route**.
5. Open **Pay & receipt** and complete the demo payment.
6. Open **Exit**, then simulate the exit-gate scan.
7. Use **Find my car** or start a new demo shop.

## Raspberry Pi 5 kiosk option

A Raspberry Pi 5 can run this prototype comfortably. For a physical trolley demo, use Raspberry Pi OS 64-bit and launch Chromium in kiosk mode against the local HTML file or a local static server. A 7–10 inch capacitive touchscreen works well for the interface.

For hardware integration, connect cameras by CSI/USB and use a dedicated microcontroller or load-cell/ADC board for basket-weight sensing. Send sensor results to the Pi over USB or serial. Use an active cooler, reliable 5 V / 5 A power provision, and proper battery-management hardware. Real payment handling, anti-theft checks, and computer vision would need secure backend services and hardware-specific integration beyond this prototype.

## Data and privacy note

The page stores only small demo preferences in the browser's local storage, such as theme, basket quantities, selected route, parking space, and shared-basket state. No data leaves the browser.

# NOTICE:
this website was made with AI

