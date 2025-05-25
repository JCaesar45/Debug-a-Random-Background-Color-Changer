````markdown
# 🎨 Random Background Color Changer

This is a simple JavaScript web app that changes the background color of the page to a random dark color from a predefined list every time a button is clicked.

---

## 📌 Features

- Randomly changes the background to one of 10 dark-themed hex colors.
- Displays the current background hex code on the screen.
- Clean UI with styled button.
- Responsive and mobile-friendly.

---

## 🛠️ Tech Stack

- **HTML5**
- **CSS3**
- **JavaScript (ES6)**

---

## 🧠 How It Works

1. A list of dark color hex codes is stored in an array.
2. On button click:
   - A random index is generated.
   - The page background is updated to the color at that index.
   - The hex code is displayed to the user.

---

## 🧪 Key Code Highlights

```js
const darkColorsArr = [
  "#2C3E50", "#34495E", "#2C2C2C",
  "#616A6B", "#4A235A", "#2F4F4F",
  "#0E4B5A", "#36454F", "#2C3E50", "#800020"
];

function getRandomIndex() {
  return Math.floor(Math.random() * darkColorsArr.length);
}

function changeBackgroundColor() {
  const color = darkColorsArr[getRandomIndex()];
  document.querySelector("body").style.backgroundColor = color;
  document.querySelector("#bg-hex-code").innerText = color;
}

document.querySelector("#btn").addEventListener("click", changeBackgroundColor);
```

---

## 🧩 Setup Instructions

1. **Clone the repo**

   ```bash
   git clone https://github.com/your-username/random-bg-color-changer.git
   cd random-bg-color-changer
   ```

2. **Open in Browser**
   Simply open `index.html` in your favorite browser.

---

## 📁 File Structure

```
/random-bg-color-changer
│
├── index.html         # Main HTML file
├── styles.css         # CSS styles
└── script.js          # JavaScript logic
```

---

## 📸 Screenshot

![App Preview](screenshot.png)
*A simple and clean UI with a functional color changer button.*

---

## 🚀 Future Enhancements

* Add option to copy hex code to clipboard.
* Add light/dark toggle themes.
* Allow user to input custom colors.
* Animate background transitions.

---

## 👨‍💻 Author

**Jordan Leturgez**
[The Ballin' J-Money World](#)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

```
