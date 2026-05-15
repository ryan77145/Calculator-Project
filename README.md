# JavaScript Calculator

A fully functional calculator built from scratch with HTML, CSS, and vanilla JavaScript. Features a custom UI with a retro-styled design, animated cursor display, and real-time expression evaluation.

Live: [ryanshill.com/projects](https://www.ryanshill.com/projects)

---

## Features

- Full arithmetic support: addition, subtraction, multiplication, and division
- Decimal input support
- Animated blinking cursor on the display screen
- Clear button resets the display
- Hover states on all buttons for interactive feedback
- Retro aesthetic using the Orbitron font, a burlywood/black/silver color palette, and inset box shadows

---

## How It Works

**Display**
The screen element holds a live string of the current input. The blinking `|` cursor is the default state, animated via a CSS `@keyframes` flash loop.

**Input**
All number and operator buttons share the `.button` class. A single `getInput()` function loops over every button and attaches a click listener that appends that button's inner text to the display string.

**Evaluation**
When `=` is clicked, the current display string is passed to `eval()` after stripping the leading cursor character. The result replaces the display content.

**Clear**
The Clear button resets the display back to `|`, restoring the cursor and wiping the current expression.

---

## File Structure

```
/
├── index.html       # Calculator markup and button layout
├── styles.css       # UI styling, grid layout, animations
└── calculator.js    # Input handling, evaluation, clear logic
```

---

## Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Semantic structure, button layout |
| CSS3 | Grid layout, custom styling, `@keyframes` animation |
| JavaScript (ES6) | DOM manipulation, event listeners, `eval()` for expression parsing |

No frameworks. No libraries. Vanilla everything.

---

## About

Built by **Ryan Shill** as a JavaScript practice project.  
Portfolio: [ryanshill.com](https://www.ryanshill.com)
