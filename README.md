# slide-puzzle

A minimalist brain-training slide puzzle that runs in your browser, on phones and computers.

**Play it here:** 
```
https://madheshiyaraj562-cmyk.github.io/slide-puzzle/
```

<h1 style="color: #FF0000;">OR</h1>

Scan the QR


<img width="735" height="735" alt="my_qr" src="https://github.com/user-attachments/assets/96cd9c87-1428-4f43-9281-9e6b4c769a66" />

## Why i made this

I wanted a simple game that trains my brain to think ahead and to stay calm under pressure. A normal slide puzzle makes you plan your moves. Adding a timer, a move limit and harder difficulty levels makes you do it while the clock is running. Blind mode goes one step further: the numbers disappear and you have to solve the puzzle from memory.

I also made it as a coding project, to practise Python and JavaScript. It started as a pygame game in Python and I turned it into a single web page so anyone can play it on any device with just a link.

## Features

- **timer on/off:** choose 1, 3, 5 or 10 minutes, or type your own
- **difficulty:** easy, hard and god (more scrambling, shorter time, move limits)
- **board size:** 3x3, 4x4, 5x5 or 6x6
- **move counter and score:** fewer moves and more time left give a higher score
- **blind mode:** numbers show for 3 seconds, then fade out. You get 3 peeks, and each peek costs 50 points
- **best scores:** saved in your browser for each difficulty, board size and blind setting
- **minimal design:** dark flat theme, one accent colour, JetBrains Mono font
- **works on mobile:** tap a tile to slide it

## How to play

Slide the tiles into the empty space until the numbers are in order, 1 to the last number, with the blank space at the bottom right.

| action | keyboard | touch |
|---|---|---|
| slide a tile | arrow keys or WASD | tap a tile |
| restart the same puzzle | R | restart button |
| new puzzle | N | new button |
| peek (blind mode) | Space | peek button |
| back to menu | Esc | menu button |

## How the score works

```
base      = (scramble x 2 - moves) x 10
time bonus = seconds left x 5          (only if the timer is on)
score     = (base + time bonus) x difficulty x board size x blind bonus - peek penalty
```

Harder difficulty, bigger boards and blind mode all multiply your score.

## Run it on your computer

1. Download `index.html`.
2. Double-click it to open it in your browser. No installation needed.

## Change the game

Open `index.html` and look for the `CONFIG` block at the top of the script. You can change the scramble length, move limits, blind-mode timing, number of peeks and score values there.

## How it is built

A single file with HTML, CSS and vanilla JavaScript, with no frameworks or libraries. Every puzzle is scrambled using only legal moves, so it can always be solved.

## Credits

Based on the Slide Puzzle game by Al Sweigart, from [inventwithpython.com/pygame](http://inventwithpython.com/pygame), released under a Simplified BSD license. Font: [JetBrains Mono](https://www.jetbrains.com/lp/mono/).

#### *Part Of Project Masterpiece*
Made by [Raj Madheshiya](https://github.com/madheshiyaraj562-cmyk).

MIT License
