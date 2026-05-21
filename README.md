⏱️ Simple Vanilla JavaScript Stopwatch

A lightweight, modern web-based stopwatch application built with clean, single-file HTML5, CSS3, and native Vanilla JavaScript. 

✨ Features

* **Minimalist UI:** Features a sleek, modern card layout centered on a vibrant linear gradient background.
* **Full Control System:** Smoothly start, pause, and reset your time.
* **Lap Recording:** Capture current display timestamps instantly and compile them into a clean, scrollable list.
* **Smooth Animations:** Interactive button hover states with crisp micro-scaling transforms.
* **No Dependencies:** Built entirely with native web technologies—no frameworks, libraries, or setups required.

🚀 How to Run

1. Save the code into a file named `index.html`.
2. Double-click the `index.html` file to open it instantly in any modern web browser.

🛠️ How It Works

### Time Tracking Logic
The application uses sequential state counters for human-readable time tracking. When the stopwatch runs, an active `setInterval` loops every 1000 milliseconds to increment the time metrics sequentially:

* **Seconds Counter:** Cascades into a minute marker upon hitting 60 seconds.
* **Minutes Counter:** Cascades into an hour marker upon hitting 60 minutes.

### Formatting Engine
To maintain a consistent digital clock aesthetic (`00:00:00`), the app passes raw counter numbers through an inline string padder before rendering to the DOM:

```javascript
let h = hours < 10 ? "0" + hours : hours;
let m = minutes < 10 ? "0" + minutes : minutes;
let s = seconds < 10 ? "0" + seconds : seconds;

📂 File Layout

└── index.html       # Combines structural HTML, styling rules, and core logic.
