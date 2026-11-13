<div align="center">

# `slide puzzle`

**a minimalist brain-training puzzle. beat the clock. trust your memory.**

[![play now](https://img.shields.io/badge/▶_play_now-7ee787?style=for-the-badge&labelColor=111111&color=111111&logoColor=white)](https://madheshiyaraj562-cmyk.github.io/slide-puzzle/)

![html](https://img.shields.io/badge/HTML-111111?style=flat-square&logo=html5&logoColor=7ee787)
![css](https://img.shields.io/badge/CSS-111111?style=flat-square&logo=css3&logoColor=7ee787)
![javascript](https://img.shields.io/badge/JavaScript-111111?style=flat-square&logo=javascript&logoColor=7ee787)
![mobile friendly](https://img.shields.io/badge/mobile-friendly-111111?style=flat-square&labelColor=111111&color=7ee787)
![no dependencies](https://img.shields.io/badge/dependencies-none-111111?style=flat-square&labelColor=111111&color=7ee787)

**[https://madheshiyaraj562-cmyk.github.io/slide-puzzle/](https://madheshiyaraj562-cmyk.github.io/slide-puzzle/)**

</div>

---

## why i made this

I wanted a simple game that trains my brain to **think ahead** and **stay calm under pressure**.

A normal slide puzzle makes you plan your moves. Add a timer, a move limit and harder levels, and you have to plan while the clock is running. **Blind mode** goes one step further: the numbers disappear and you solve the puzzle from memory.

It is also a coding project. It started as a pygame game in Python, and I turned it into a single web page so anyone can play it on any device with just a link.

---

## the game

```
┌────┬────┬────┬────┐
│  1 │  2 │  3 │  4 │
├────┼────┼────┼────┤
│  5 │  6 │  7 │  8 │
├────┼────┼────┼────┤
│  9 │ 10 │ 11 │ 12 │
├────┼────┼────┼────┤
│ 13 │ 14 │ 15 │    │   ← the goal: numbers in order, blank bottom right
└────┴────┴────┴────┘
```

Slide the tiles into the empty space until they are back in order.

---

## features

| | feature | details |
|---|---|---|
| ⏱ | **timer** | on or off. Pick 1, 3, 5 or 10 minutes, or type your own |
| 🎚 | **difficulty** | `easy`, `hard`, `god`: more scrambling, less time, move limits |
| 📐 | **board size** | 3x3, 4x4, 5x5 or 6x6 |
| 🔢 | **score** | fewer moves and more time left means a higher score |
| 🙈 | **blind mode** | numbers show for 3 seconds, then fade away. 3 peeks, each costs 50 points |
| 🏆 | **best scores** | saved in your browser per difficulty, size and blind setting |
| 📱 | **mobile friendly** | tap a tile to slide it, works on any screen |
| 🎨 | **minimal design** | dark, flat, one accent colour, JetBrains Mono font |

---

## controls

| action | keyboard | touch |
|---|---|---|
| slide a tile | `arrow keys` / `W A S D` | tap a tile |
| restart same puzzle | `R` | **restart** button |
| new puzzle | `N` | **new** button |
| peek (blind mode) | `Space` | **peek** button |
| back to menu | `Esc` | **menu** button |

---

## difficulty levels

| level | scramble moves | default time | move limit | score multiplier |
|---|---|---|---|---|
| easy | 20 | 5 min | none | x1 |
| hard | 80 | 3 min | 3x scramble | x2 |
| god | 200 | 2 min | 2.5x scramble | x5 |

---

## how the score works

```
base       = (scramble × 2 − moves) × 10
time bonus = seconds left × 5                  (only when the timer is on)

score = (base + time bonus) × difficulty × (board size ÷ 9) × blind bonus − peek penalty
```

Harder levels, bigger boards and blind mode (x2) all multiply your score.

---

<details>
<summary><b>run it on your computer</b></summary>

<br>

1. Download `index.html`.
2. Double-click it. It opens in your browser. No installation needed.

</details>

<details>
<summary><b>change the game yourself</b></summary>

<br>

Open `index.html` and find the `CONFIG` block at the top of the script. You can change:

- scramble length and move limits for each difficulty
- blind mode timing and number of peeks
- score multipliers and the peek penalty

Save the file and reload the page to see the change.

</details>

<details>
<summary><b>how it is built</b></summary>

<br>

A single file of HTML, CSS and vanilla JavaScript, with no frameworks and no libraries. Every puzzle is scrambled using only legal moves, so it can always be solved. Best scores use the browser's `localStorage`.

</details>

---

## credits

Based on the **Slide Puzzle** game by Al Sweigart, from [inventwithpython.com/pygame](http://inventwithpython.com/pygame), released under a Simplified BSD license.

Font: [JetBrains Mono](https://www.jetbrains.com/lp/mono/).

<div align="center">

made by [Raj Madheshiya](https://github.com/madheshiyaraj562-cmyk)

</div>
