# AI Tools Spring 2026

## Assignment #20: Simple Game

### ChatGPT prompt

> Create a prompt for creating a single file snake game in HTML5/JS/CSS. Free-angle turning (left/right arrows and A/D), faster turn when a modifier (shift or space) is pressed. Smooth nice graphics (something dark + teal/purple), snake scales and segments visible, some details in the head. Particle effects on collisions, head explodes. Eating a food pellet shows a small bulge at it's location as the body passes the point until the tail is reached. Max three food visible at the same time, food vanishes if not eaten. Subtle short-ish tail trail. Some different food types with different outcomes; regular adds length, speeder adds length and speed (+1) instantly, slower adds length and slows (-1) down instantly, splitter reduces length (tail shrinks nicely). Eaten food type is shown briefly. Speed increases (+1) at certain intervals. Logical scoring (integer score!), and 5 best scores saved to localStorage. Claude Sonnet optimized prompt.

## Output

Here’s a **Claude Sonnet-optimized prompt** you can directly paste into Claude (or another coding model). It’s structured to maximize implementation quality, completeness, and visual polish.

---

## Prompt — HTML5 Free-Angle Snake Game (Single File)

You are an expert senior game developer and creative frontend engineer.

Create a **complete, production-quality snake game implemented as a SINGLE self-contained HTML file** (HTML + CSS + JavaScript together). No external libraries or CDNs. Everything must run by simply opening the file in a browser.

### Core Requirements

Build a **modern smooth snake game** with **free-angle turning** rather than grid movement.

---

## Gameplay

### Movement

* Snake moves continuously forward.
* Turning is **free-angle rotation**, not grid based.
* Controls:

  * LEFT ARROW or `A` → turn left.
  * RIGHT ARROW or `D` → turn right.
* Holding a modifier:

  * `Shift` OR `Space`
  * increases turning speed (tighter turning radius).

Movement and rotation must feel smooth and responsive.

---

## Visual Style

Create polished visuals:

* Dark theme background.
* Accent colors:

  * teal
  * purple.
* Smooth animation at ~60fps using `requestAnimationFrame`.

Snake:

* Visible body segments.
* Scales or subtle texture.
* Slight shading or gradient along body.
* A recognizable head:

  * small eyes or head detail.
  * slightly different shape from body.

Tail:

* Short, subtle fading trail behind the tail.

---

## Food System

### General

* Maximum **3 food pellets visible simultaneously**.
* Food disappears after some time if not eaten.
* Spawn new food automatically when needed.

### Food Types

Include visually distinct food types:

1. **Regular**

   * Adds length.

2. **Speeder**

   * Adds length.
   * Instantly increases speed by +1.

3. **Slower**

   * Adds length.
   * Instantly decreases speed by −1.

4. **Splitter**

   * Reduces snake length.
   * Tail shrinks smoothly rather than snapping.

Each food type must:

* Have unique colors or glow.
* Show a brief floating label when eaten (example: “+Speed”, “Slow”, etc.).

---

## Eating Effects

When food is eaten:

* Show a small visible **bulge traveling through the snake body** at the eaten location.
* Bulge moves naturally along body segments.
* Bulge disappears when it reaches the tail.

---

## Speed System

* Speed increases automatically by +1 at certain score or time intervals.
* Speed must remain controllable and fair.

---

## Collision

Snake dies when:

* Head collides with itself.
* Head collides with boundary (or define your own logical boundary).

Death effects:

* Head explodes into particles.
* Use particles matching teal/purple theme.
* Smooth animated particle dispersion.

---

## Graphics & Effects

Include:

* Subtle glow effects.
* Smooth interpolation of movement.
* Minor motion polish.

Particles:

* On death explosion.
* Optional small spark when eating food.

---

## Score System

* Logical integer score.
* Score increases from:

  * eating food.
  * possibly survival time.

Display:

* Current score clearly visible.

---

## High Scores

Save locally:

* Top 5 best scores.
* Use `localStorage`.

Requirements:

* Automatically update list after death.
* Display best scores on screen.
* Sorted highest → lowest.

---

## Technical Requirements

* Single `.html` file only.
* No frameworks.
* No external dependencies.
* No images required — use Canvas rendering.
* Use HTML5 Canvas.
* Smooth delta-time animation.
* Organized readable code.

Structure clearly:

* Game loop.
* Rendering.
* Physics/update.
* Input handling.
* Effects system.

---

## Polish

Focus heavily on:

* Smooth feel.
* Clean visuals.
* Good performance.
* Readable code.

Avoid:

* Grid snapping.
* Janky rotation.
* Instant body resizing.

---

## Deliverable

Output ONLY:

* The complete single HTML file.
* No explanations.

---

If you want, I can also give you a **“Claude Sonnet ultra-max quality version”** (even stronger prompt engineering that tends to produce *serprisingly high-end results*) or a **GPT-5.2 optimized version** — just ask 👍.
