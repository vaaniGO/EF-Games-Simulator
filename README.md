# EF Games Simulator

An interactive playground for two game-based proof techniques in finite model theory:

- **Ehrenfeucht–Fraïssé games** for first-order logic (a fixed number of rounds)
- **Pebble games** for fixed-point logic, FO(LFP) (a fixed number of pebble pairs)

Write a sentence φ, draw or pick two graphs A and B, and play Spoiler and Duplicator. The rules are enforced automatically: after every round the map f(xᵢ) = yᵢ must preserve adjacency and equality (a partial isomorphism), and the winner is shown as soon as the game is decided.

## Features

- Sentence input with symbols (`∃ ∀ ∧ ∨ ¬ → ↔ = ≠`) or plain words (`exists`, `forall`, `and`, `or`, `not`), plus fixed points written as `[lfp R(x,y) : … ](u,v)`
- Live truth values: A ⊨ φ / A ⊭ φ for each graph
- The number of rounds (EF) is the sentence's quantifier depth; the number of pebble pairs is its number of variables
- Draw your own graphs, or use a cycle of length n, a complete graph on n vertices, or a disconnected graph
- Hints, undo, and a computer player for either side
- An optional perfect-play oracle that solves the game exactly for small graphs (up to 10 vertices each)

## Deploying with GitHub Pages

The whole app is a single static file, `index.html`, so there is no build step.

1. On GitHub, open the repository and go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
3. Choose the **main** branch and the **/ (root)** folder, then click **Save**.

After a minute or so the site is live at:

https://vaanigo.github.io/EF-Games-Simulator/

## Running locally

Open `index.html` in a browser. To serve it the same way GitHub Pages does:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Credits

The overview of EF games on the page is adapted from the [Cornell Math Explorers' Club lesson on Ehrenfeucht–Fraïssé games](https://pi.math.cornell.edu/~mec/Summer2009/Raluca/lesson1.html).
