# 🧠 Ultimate Memory Game

A modern, highly customizable, and interactive memory matching game built completely from scratch using **vanilla HTML, CSS, and JavaScript**. No external libraries, no image files, and no audio files required!

## ✨ Features

- **3 Card Themes**: Choose between Emojis (🍎), Letters (A), or Numbers (1).
- **3 Difficulty Levels**: 
  - Easy (4x4 grid - 8 pairs)
  - Medium (6x4 grid - 12 pairs)
  - Hard (6x6 grid - 18 pairs)
- **Live Game Stats**: Tracks your current **Time** and **Moves** in real-time.
- **Sound Effects**: Procedurally generated sound effects for flipping, matching, and winning using the native **Web Audio API** (no `.mp3` files needed!).
- **Sleek UI/UX**: Features smooth 3D card-flipping animations, responsive grid layouts, and a modern color palette.
- **Fully Responsive**: Works perfectly on both desktop browsers and mobile devices.

## 🚀 How to Run

Because this project uses pure vanilla web technologies, there are no build steps, package managers, or servers required.

1. Clone or download this repository.
2. Locate the `index.html` file on your computer.
3. Double-click `index.html` to open it in your default web browser.
4. Enjoy the game!

## 🎮 How to Play

1. Use the dropdown menus at the top to select your preferred **Card Type** (Emojis, Letters, or Numbers) and **Difficulty Level**.
2. Click on any card to reveal its symbol. The timer will start on your first click.
3. Click on a second card to try and find its match.
4. If they match, they will turn green and stay face-up.
5. If they don't match, they will flip back over after 1 second. Try to remember their positions!
6. Find all the pairs as fast as you can with the fewest amount of moves.
7. When you match all pairs, a Win Screen will display your final Time and Move count.

## 🛠️ Technologies Used

- **HTML5**: Game structure and semantics.
- **CSS3**: Grid layout, Flexbox, gradients, and 3D transform animations (`perspective`, `rotateY`, `backface-visibility`).
- **JavaScript (ES6)**: Game logic, DOM manipulation, Fisher-Yates shuffle algorithm, and interval timers.
- **Web Audio API**: Synthetic sound generation (`AudioContext`, `OscillatorNode`, `GainNode`).

## 🔧 Customization

Want to add your own symbols? It's incredibly easy! 
Open `index.html` in a text editor, find the `dataSets` object in the JavaScript, and add your own array of items:

```javascript
const dataSets = {
    emojis: ['🍎','🍌','🍇','🍓','🍒','🍍','🥝','🍉','🍑','🥥','🍋','🍈','🍏','🍐','🍊','🥭','🫐','🍅'],
    letters: ['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R'],
    numbers: ['1','2','3','4','5','6','7','8','9','10','11','12','13','14','15','16','17','18'],
    // Add your own custom set here! Must have at least 18 items for "Hard" mode.
    animals: ['🐶','🐱','🐭','🐹','🐰','🦊','🐻','🐼','🐨','🐯','🦁','🐮','🐷','🐸','🐵','🐔','🐧','🐦']
};
```
(Don't forget to add a new <option> tag in the HTML <select> dropdown if you add a new set!)
