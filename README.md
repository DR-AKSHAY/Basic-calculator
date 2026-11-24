# ⚡ Basic Calculator ⚡

A sleek, modern calculator built with **HTML, CSS and vanilla JavaScript**. It features a glassmorphism design, an animated gradient background, calculation history, and full keyboard support.

---

## ✨ Features

- **Basic operations:** addition, subtraction, multiplication, division and percentage
- **Clear (C) and Delete (⌫)** buttons
- **Calculation history:** stores your last 20 calculations and saves them in the browser (`localStorage`), so they remain after a refresh
- **Click a history item** to reuse its result
- **Keyboard support:** type numbers and operators directly
- **Error handling:** invalid expressions or division by zero show `Error` with a shake animation
- **Animations:** animated gradient background, floating card, glowing shadow, button ripple, pulsing `=` button, display pulse on result, and a welcome fade-in
- **Responsive layout:** works on desktop and mobile screens

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| HTML5 | Structure |
| CSS3 | Styling, gradients, glassmorphism, animations |
| JavaScript (ES6) | Logic, history, keyboard events |
| [Font Awesome](https://fontawesome.com/) | Delete icon |
| [Google Fonts – Poppins](https://fonts.google.com/specimen/Poppins) | Typography |

---

## 📁 Project Structure

```
basic-calculator/
│
├── index.html     # Page layout and buttons
├── style.css      # Styling and animations
├── script.js      # Calculator logic
└── README.md      # Project documentation
```

---

## 🚀 Getting Started

No installation or build step is needed.

1. **Download or clone** the project:
   ```bash
   git clone https://github.com/your-username/basic-calculator.git
   ```
2. **Open the folder:**
   ```bash
   cd basic-calculator
   ```
3. **Open `index.html`** in any modern browser (double-click it, or use the VS Code *Live Server* extension).

> An internet connection is needed on first load for Google Fonts and Font Awesome.

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `0` – `9` | Enter digits |
| `+` `-` `*` `/` `%` | Operators |
| `.` | Decimal point |
| `Enter` | Calculate result |
| `Backspace` | Delete last character |
| `Delete` / `Esc` | Clear display |

---

## 🧮 How It Works

1. Each button click (or key press) appends a value to an `expression` string.
2. Pressing `=` evaluates the expression and shows the result.
3. Valid calculations are saved to the history list (most recent first, max 20) and stored in `localStorage` under the key `sakHistory`.
4. If the result is not a finite number (e.g. `5/0`), the calculator shows **Error** and resets.

---

## ⚠️ Known Limitations & Ideas for Improvement

- **`eval()` is used** to compute results. This is fine for a personal learning project where input only comes from the calculator's own buttons, but a safer approach is to write a small expression parser (or use a library such as [math.js](https://mathjs.org/)).
- **`%` behaves as modulo** (e.g. `10%3 = 1`), not as a percentage of a number.
- **Floating-point precision:** results like `0.1 + 0.2` show `0.30000000000000004`. Rounding the output would fix this.
- **No input validation:** operators can be entered back-to-back (e.g. `5++3`).
- **Missing styles:** the `.background span` bubbles and the `.rgb-border` element in the HTML have no colors/positions defined yet, and the `borderMove` keyframes are unused. Adding them would complete the intended glowing-border and floating-orb effects.
- **Possible additions:** dark/light theme toggle, scientific mode, a "Clear history" button, and sound effects.

---

## 📸 Preview

*Add a screenshot or GIF of your calculator here:*

```
![Calculator Preview](screenshot.png)
```

---

## 🤝 Contributing

Suggestions and improvements are welcome. Fork the repo, make your changes, and open a pull request.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👤 Author

Made with ❤️ by **avinash tripathi**
GitHub: [@DR-AKSHAY](https://github.com/your-username)
