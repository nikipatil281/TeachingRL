# ☕ TeachingRL — Learn Reinforcement Learning Through a Coffee Shop

> **Live Demo:** [teaching-rl.vercel.app](https://teaching-rl.vercel.app)

---

## What is this?

**TeachingRL** is an interactive, browser-based simulation designed to teach the core concepts of **Reinforcement Learning (RL)** through a fun and tangible metaphor — running your own coffee shop.

Instead of reading theory, you *experience* it. You set the price of coffee each day, watch the market react, face competitors, unpredictable weather, and local events — and slowly build the intuition behind why RL agents learn the way they do.

---

## How it works

The app is structured into two phases:

### Phase 1 — Training Mode (Tutorial)
A guided 7-day trading week where you run your coffee shop solo. Each day introduces a new RL concept through actual gameplay:

| Day | Concept Introduced |
|-----|--------------------|
| 1   | State, Agent & Action |
| 2   | Environment |
| 3   | Sequential Learning |
| 4   | Reward |
| 5   | Exploration |
| 6   | Penalty |
| 7   | Exploration vs Exploitation |

At the end of the week, you get a **Weekly Report** with a pricing policy summary showing how your decisions compared across different market conditions.

### Phase 2 — Main Simulation (28 Days)
Now you play alongside two AI agents — an **ML Agent** (pattern-based predictor) and an **RL Agent** (Q-learning) — experiencing the same market conditions you do. At the end of each week, you review a performance report comparing your profit, sales, and pricing policy against the agents.

You can also customise the simulation by toggling which market variables are active (Weather, Local Events, Competitor).

---

## Key Concepts Demonstrated

- **State / Action / Reward** — the core RL loop, made tangible
- **Exploration vs Exploitation** — when to try new prices vs. rely on what worked
- **Sequential Decision Making** — how today's inventory affects tomorrow's options
- **Penalties** — sell-out (emergency restock) and overstock (disposal fee) consequences
- **Policy Review** — compare your pricing strategy against the RL agent's optimal range

---

## Tech Stack

- **React** (Vite)
- **Framer Motion** — animations & transitions
- **Tailwind CSS** — styling
- **Lucide React** — icons
- **Custom RL Engine** — Q-learning agent implemented in vanilla JS (`src/logic/RLAgent.js`)
- **Deployed on Vercel**

---

## Running Locally

```bash
# Install dependencies
npm install

# Start dev server
npm run dev
```

---

## Project Structure

```
src/
├── components/        # All UI components (Tutorial, Dashboard, Modals, etc.)
├── logic/             # Market engine, RL agent, ML predictor
└── App.jsx            # Phase routing & global state
```

---

*Built as an educational tool to make Reinforcement Learning approachable and intuitive — no maths degree required.*
