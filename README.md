# Long Division — Pastel Rainbow + Sound + Celebration

An interactive long-division practice game (2-digit÷1-digit, 3-digit÷1-digit) with:
- **Traditional long division layout** (hundreds/tens/ones aligned grid)
- **Stepwise inputs** (quotient → partial product → subtraction line → bring-down …)
- **Soft pastel rainbow feedback** for correct inputs, **gray** for wrong inputs
- **Live checking** on every keystroke
- **Fun chiptune-style motifs** on correct answers, **buzz** on wrong answers
- **Confetti + toast** celebrating when all inputs are correct
- **Non-trivial problems** only (avoids times-table-trivial cases)

> Works fully offline. Single-file HTML (no frameworks).

## Demo
- (Optional) GitHub Pages: **[https://YOUR_USER.github.io/YOUR_REPO/](https://math-gamex.github.io/long-division-game)**
- (Optional) Preview GIF  
  ![Preview](assets/preview.gif)

## Features
- SVG underlay lines so they **never overlap** with input boxes:
  - Under divisor/dividend row
  - Mid subtraction lines per step
  - Above final remainder
- **Numbered badges** (very subtle) guide the recommended solving order  
  *(You can fill boxes in any order; numbering is only a guide.)*
- **Web Audio API**:
  - Correct → rotates through 5 short, fun **chip-tune motifs**
  - Wrong → **buzz**
- Accessibility friendly-ish: large hit targets, low visual clutter, pastel colors

## How to Use
1. Open `index.html` in a modern browser (Chrome/Edge/Firefox/Safari).
2. Choose problem type: **2-digit ÷ 1-digit** or **3-digit ÷ 1-digit**.
3. Type digits in the grid boxes.  
   - Correct: pastel rainbow color + short motif 🎶  
   - Wrong: gray + buzz  
4. When every box is correct → **🎉 confetti + toast** automatically.

> Browser note: the first interaction (typing/clicking) enables audio due to browser autoplay policies.

## Local Development
- Just open `index.html`.  
- Or run a local server (optional):
  ```bash
  # Python 3
  python -m http.server 8000
  # then visit http://localhost:8000
