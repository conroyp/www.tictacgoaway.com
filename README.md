# TicTacGoAway

**Tic-Tac-Toe, Evolved.**

A fresh twist on the classic game where pieces don't stay forever. Each player can only have 3 pieces on the board at once - place your 4th, and your oldest vanishes. No more draws, no more stalemates.

Play at: [tictacgoaway.com](https://www.tictacgoaway.com)

## Features

- **The Twist**: First in, first out - your oldest piece disappears when you place your 4th
- **Two Modes**: Play against a friend (2 Player) or challenge the bot (vs Computer)
- **Three Difficulty Levels**: Easy, Medium, and Hard AI opponents
- **Stats Tracking**: Win/loss record and win streaks saved locally
- **Sound Effects**: Synthesized audio feedback (Web Audio API)
- **Confetti Celebration**: Victory animations
- **Fully Responsive**: Works on desktop and mobile
- **Lightweight**: Single HTML file, no build step required

## How to Play

1. Get three in a row - horizontal, vertical, or diagonal
2. You can only have **3 pieces** on the board at once
3. Place your 4th piece and your oldest one vanishes
4. Watch for the **pulsing piece** - that's the one about to go
5. Think ahead and force tough choices on your opponent

## Deployment

A single self-contained `index.html` (inlined CSS + JavaScript), plus `favicon.png` and `og-image.png`. No build process, no dependencies, no server-side code.

Hosted on **Cloudflare Pages**, connected to this GitHub repo — **every push to `main` auto-deploys**. The site is fully static, so the Pages project uses **build command: none** and **output directory: `/`** (repo root). Custom domain: **tictacgoaway.com**. (Migrated from S3 static hosting.)

## Tech Stack

- HTML5
- CSS (Tailwind CSS v3.4, purged and inlined)
- Vanilla JavaScript
- Web Audio API for sound effects
- Canvas API for confetti animation
- Google Fonts (Outfit)

## Development

To regenerate the Tailwind CSS (if modifying styles):

```bash
npm install tailwindcss@3 --save-dev
npx tailwindcss -i input.css -o output.css --minify
```

Then inline the output into the `<style>` tag in `index.html`.

## License

Released under the [MIT License](LICENSE) — free to use.

## Author

[conroyp](https://www.conroyp.com)

---

**More games:**
- [Kids Sudoku](https://www.kidssudoku.com)
- [JDCaptcha](https://www.jdcaptcha.com)
