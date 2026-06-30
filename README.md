# Personal Portfolio Website

This is Minh Pham's personal portfolio website featuring projects and professional information.

## Website Structure

```
/
├── index.html           # Main landing page
├── styles.css           # Global styles
├── Resume.pdf           # Resume
├── images/              # Project screenshots and cover art
└── pkg/                 # Tetris WASM game files
```

## Sections

- **About** — short personal introduction
- **Projects**
  - **Tetris** — featured, playable in the browser (Rust + wgpu, compiled to WebAssembly)
  - **Mazegame** — competitive code-vs-code maze game (Zig + C++, sockets, matchmaking)
  - **Spicy Adventures** — action roguelike (Godot, HTML5)
  - **Roads Royale** — two-player turn-based strategy game
  - **snag** — campus fashion marketplace app
- **Student Plan** — embedded PDF
- **Calendar** — embedded Google Calendar
- **Contact** — links to GitHub, LeetCode, and LinkedIn

To add a new project, copy a `.project-card` block in the "More projects" grid in
`index.html` and drop its cover image in `images/`.

## Development

To test your changes locally:
1. Open `index.html` in a web browser
2. For the Tetris game to work, you may need to run a local server:
   ```bash
   python -m http.server 8000
   # or
   npx http-server
   ```

## Notes

- The site is responsive and mobile-friendly
- Navigation is consistent across the page
