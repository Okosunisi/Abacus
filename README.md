# ABACUS

A scientific calculator, styled like a physical instrument — phosphor-green LCD display, graphite body, single-file HTML/CSS/JS with no dependencies or build step.

## Features

- **Core operations**: addition, subtraction, multiplication, division, parentheses
- **Scientific functions**: sin, cos, tan (and inverses), ln, log, √, x², xʸ, n!, 1/x, %
- **Constants**: π, e
- **Angle modes**: RAD / DEG toggle
- **Memory**: MC (clear), MR (recall), M+ (add), M− (subtract)
- **Keyboard support**: type numbers and operators directly, `Enter` for `=`, `Backspace` to delete, `Esc` to clear
- **Responsive**: works down to mobile widths, with visible keyboard focus states

## Usage

Just open `index.html` in any modern browser — no installation, no build step, no dependencies.

```bash
# clone the repo, then:
open index.html      # macOS
start index.html      # Windows
xdg-open index.html   # Linux
```

## How it works

Expressions are parsed with a small tokenizer and converted to Reverse Polish Notation via the shunting-yard algorithm, then evaluated — no `eval()` involved. This keeps operator precedence, unary minus, functions, and factorials all correct without relying on JavaScript's own expression parser.

## Tech

Plain HTML, CSS, and vanilla JavaScript. One file, no frameworks, no build tools.

## License

MIT
