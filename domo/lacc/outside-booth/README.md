# Domo Cafe — LA Comic Con outside booth

Ready-to-host static 3D simulation for Jarvis HQ. No build step, account, API keys, backend, or CDN is required. Three.js r128 is bundled locally with its MIT license. Artwork and menu QR textures are embedded in booth.js; original uploads are included in assets for reference.

## Publish

Copy this folder into an appropriate static location in Jarvis HQ, such as `/domo/lacc/outside-booth/`. Keep `index.html`, `styles.css`, `booth.js`, and `vendor/` together. All references are relative, so subdirectory hosting works. Use Jarvis HQ's established deployment and access process. There is no integration with or dependency on the original Railway reference website.

For local review, run `python3 -m http.server 8080` from this folder and open `http://localhost:8080/`. Open the page directly from disk if preferred; an HTTP server is recommended for testing host behavior.

## Included behavior

- Exterior, inside layout, and overhead views
- Drag to orbit, mouse-wheel and button zoom
- Canopy, sidewall, and equipment label toggles
- 10 × 10 foot tent, supplied canopy and half-wall graphics
- Two supplied Domo Cafe flags, modeled at 54.3 inches high, approximate 18.9 inch width from artwork ratio
- Left window ORDER + PAY, right window PICKUP
- Two menu A-frame signs, each with a real QR code for the existing Toast menu
- Separate stanchion lanes, assumed 4 feet wide
- Back cookline: 36 inch griddle plus 27 inch prep table
- Two ice chests, front folding table, handwash station, two chairs, optional fan

QR destination: https://order.toasttab.com/online/domo-cafe-8340-la-palma-avenue

## Assumptions to preserve or explicitly revise

Equipment and tent geometry is schematic. The 36 inch griddle width, 27 inch prep table width, 10 × 10 foot tent, and flag height come from user specifications. Tent eave is assumed 7 feet; peak is assumed 10.3 feet. Flag mounts, table size (6 × 2.5 feet), ice chests (30 × 18 inches), equipment depths, handwash model, two chairs, 24 × 36 inch A-frame panels, and queue footprint are assumptions. The gray background pad is visualization context, not reserved convention floor space. The rear wall is neutral because no rear graphic was supplied. Staff entrance and utility placements are not specified.

Menu signs currently show a heading and QR rather than a priced convention menu. The QR opens the existing cafe menu, not a dedicated LACC menu. Replace these only when Izzy supplies the approved event menu/destination. Keep all Domo logos and character art as supplied; do not redraw, reinterpret, or modify them.

## Validation

JavaScript syntax, local resource paths, embedded image decoding, QR payload generation, and ZIP integrity were checked. Browser/WebGL visual QA was not completed in the authoring environment because a browser executable was unavailable. Before publishing, verify rendering and controls in a real browser at desktop and mobile sizes, inspect artwork orientation, check that flags and lanes fit in each view, and scan both displayed QR codes. Use the Grok instructions for the final deployment checks.

This package is a visual planning model. Physical staff access, venue allocation, equipment clearances, and utility requirements remain to be settled in the booth plan.
