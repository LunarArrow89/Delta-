# Delta

Delta is a small programming language playground for learning to code and making simple canvas programs. The editor itself is a coding tool, not a game. Press **Run in window** to open your program in a separate window.

## Hello world

```delta
let name = "world"
print("Hello, " + name)
```

## Draw a scene

```delta
screen(640, 400)
background("#182033")
square[\n    name(Player)\n    location(60, 80)\n    size(70)\n    color("#9c8cff")\n]\nmovesquare("Player", 3.5)
circle(220, 120, 35, "#72e0b1")
text("Made with Delta!", 60, 230, "#ffffff", 28)
```

## Language basics

- `print("text")` writes output in the program window
- `let score = 10` creates a variable
- `score = score + 1` changes an existing variable
- Values: numbers, quoted strings, `true`, `false`, and `null`
- Math: `+`, `-`, `*`, `/`, `%`
- Comparisons: `==`, `!=`, `<`, `>`, `<=`, `>=`
- Logic: `and`, `or`, `not`, `&&`, `||`, `!`
- Decisions: `if condition { ... } else { ... }`
- Comments start with `//`

## Drawing commands

- `screen(width, height)` sets the canvas size
- `background(color)` fills the canvas
- `square[ name(Name) location(x, y) size(value) color(color) ]` creates and draws a named square without moving it\n- `movesquare("Name", speed)` adds keyboard movement to an already-created square without drawing another one
- `rect(x, y, width, height, color)` draws a rectangle
- `circle(x, y, radius, color)` draws a circle
- `text(message, x, y, color, size)` draws text
- `clear()` clears the canvas

Your current code autosaves in this browser. Use **Save** to store named projects, and use the saved-project menu to reopen them. Saved projects stay in the same browser on the same device. Browser pop-ups must be allowed for the Run in window button.
