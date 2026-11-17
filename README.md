# PhysicsLab: Forces, Laws of Motion & Mechanical Equilibrium

An interactive, dependency-free physics website, ready for GitHub Pages.

## What's inside
- **Learn**: Newton's laws, friction, inclines, equilibrium (ΣF = 0, Στ = 0) and a problem-solving recipe.
- **Simulations** (canvas, live free-body diagrams):
  1. Newton's 2nd Law with static/kinetic friction
  2. Inclined plane (components, sliding threshold tanθ > μ)
  3. Hanging sign on two cables (find T₁, T₂)
  4. Seesaw / torque balance (rotational equilibrium)
- **Pre-test**: 10 randomized problems per attempt ("Find F, N, T, a…"), auto-checked within 2%, with step-by-step solutions and a saved best score.

## Deploy on GitHub Pages
1. Create a repository and add `index.html` and `README.md` to the root of the `main` branch.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then Save.
4. After a minute your site is live at `https://<username>.github.io/<repo>/`.

## Customize
- Add a new pre-test problem: append a generator to the `gens` array in `index.html` (return `text`, `parts` with answers, `sol`, `hint`).
- Add a simulation: create an object like `newton` (with `controls`, `calc`, `readout`, `draw`) and add it to the `sims` array.
