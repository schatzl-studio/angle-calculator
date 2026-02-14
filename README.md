# Angle Calculator

A handy minimal, single-file right-triangle calculator built for workshop and woodworking use.  
Enter any two known values (sides or angles) and all remaining values are computed instantly.

---

## Features

- **Any two inputs** — enter any combination of two sides (a, b, c) or angles (α, β) to solve the triangle
- **Bilingual** — full German/English interface, toggled via a DE · EN switch in the header; default is German
- **Live validation** — clear error messages for impossible inputs (e.g. hypotenuse shorter than a leg, angles not summing to 90°)
- **Interactive SVG diagram** — labeled triangle visualization with mirror and rotate controls
- **Color-coded fields** — green for user input, blue for calculated results
- **Zero dependencies** — single `.html` file, no build step, no framework
- **PWA-ready** — works as a standalone app on iOS (Add to Home Screen)
- **Responsive** — adapts to mobile and desktop

## Usage

Open `angles.html` directly in any modern browser — no server required.

1. Enter any two values in the **Seiten / Sides** and **Winkel / Angles** columns
2. The remaining three values appear automatically after a short debounce
3. Use **↔ Spiegeln / Mirror** and **⟳ Rotieren / Rotate** to reorient the diagram
4. Press **Neu / Reset** to clear all fields and start over
5. Toggle the **DE · EN** switch in the top-right corner to change language

### Input reference

| Field | DE           | EN         | Unit | Range         |
|-------|--------------|------------|------|---------------|
| a     | Gegenkathete | Opposite   | mm   | > 0, ≤ 99 999 |
| b     | Ankathete    | Adjacent   | mm   | > 0, ≤ 99 999 |
| c     | Hypotenuse   | Hypotenuse | mm   | > 0, ≤ 99 999 |
| α     | Winkel α     | Angle α    | °    | 0.01 – 89.99  |
| β     | Winkel β     | Angle β    | °    | 0.01 – 89.99  |

The right angle γ = 90° is always fixed at vertex C.

## Triangle convention

```
C ──── B
│    /
│   /    C = 90°  (right angle)
│  /     α at A   (bottom-left)
│ /      β at B   (top-right)
│/
A
```

- **a** (Gegenkathete / Opposite) is opposite α — the horizontal leg C–B
- **b** (Ankathete / Adjacent) is opposite β — the vertical leg C–A
- **c** (Hypotenuse) is the diagonal A–B

## Browser support

Any evergreen browser (Chrome, Firefox, Safari, Edge) with JavaScript.

## License

MIT License

Copyright (c) 2025 SCHATZL Fine Furniture

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL SCHATZL FINE FURNITURE BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

*SCHATZL Fine Furniture — [schatzl.studio](https://schatzl.studio)*
