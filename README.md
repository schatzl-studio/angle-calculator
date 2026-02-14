# SCHATZL Winkelrechner

A minimal, single-file right-triangle calculator built for workshop and woodworking use.  
Enter any two known values (sides or angles) and all remaining values are computed instantly.

---

## Features

- **Any two inputs** — enter any combination of two sides (a, b, c) or angles (α, β) to solve the triangle
- **Live validation** — clear German-language error messages for impossible inputs (e.g. hypotenuse shorter than a leg, angles not summing to 90°)
- **Interactive SVG diagram** — labeled triangle visualization with mirror and rotate controls
- **Color-coded fields** — green for user input, blue for calculated results
- **Zero dependencies** — single `.html` file, no build step, no framework
- **PWA-ready** — works as a standalone app on iOS (Add to Home Screen)
- **Responsive** — adapts to mobile and desktop

## Usage

Open `angle-calculator.html` directly in any modern browser — no server required.

1. Enter any two values in the **Seiten** (sides) or **Winkel** (angles) columns
2. The remaining three values appear automatically after a short debounce
3. Use **↔ Spiegeln** and **⟳ Rotieren** to reorient the diagram
4. Press **Neu** to clear all fields and start over

### Input reference

| Field | Meaning        | Unit | Range          |
|-------|----------------|------|----------------|
| a     | Gegenkathete   | mm   | > 0, ≤ 99 999  |
| b     | Ankathete      | mm   | > 0, ≤ 99 999  |
| c     | Hypotenuse     | mm   | > 0, ≤ 99 999  |
| α     | Angle at A     | °    | 0.01 – 89.99   |
| β     | Angle at B     | °    | 0.01 – 89.99   |

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

- **a** (Gegenkathete) is opposite α — the horizontal leg C–B
- **b** (Ankathete) is opposite β — the vertical leg C–A
- **c** (Hypotenuse) is the diagonal A–B

## Browser support

Any evergreen browser (Chrome, Firefox, Safari, Edge). No polyfills needed.

## License

Copyright © 2025 SCHATZL Fine Furniture. All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

This software is provided "as is" without warranty of any kind. In no event shall the copyright holder be liable for any claim, damages or other liability arising from the use of this software.

---

*SCHATZL Fine Furniture — [schatzl.studio](https://schatzl.studio)*
