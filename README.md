# Nudge 🧠💳
*An empathetic behavioral fintech platform bridging mental health telemetry with automated banking interventions.*

> **Hack for Humanity Submission**
> 📺 [Watch the 3-Minute Video Presentation](YOUR_VIDEO_LINK_HERE)  
> 📊 [View the Master Pitch Deck & Wireframes](YOUR_SLIDE_DECK_LINK_HERE)

---

## 🚀 Overview
Traditional budgeting apps treat finances purely as numbers, punishing users with red alerts when they stress-spend. **Nudge** takes a human-centric approach. By combining subjective mental health telemetry (1–10 stress, anxiety, and energy scales) with real-time banking data, Nudge automatically executes protective financial interventions—such as cooling-off savings sweeps and micro-debt payoffs—while delivering compassionate guidance.

---

## 👥 The 5 Behavioral Archetypes
Nudge tailors its strategy based on the user's primary behavioral profile, diagnosed during onboarding:
1. **The Impulse Stress-Shopper**: High stress triggers retail therapy. *(Strategy: Cooling-off balance sweeps & intercept prompts)*
2. **The Debt Avoider**: Anxiety causes active account avoidance. *(Strategy: Snowball payoff method for quick psychological wins)*
3. **The Executive Dysfunction Planner**: Severe cognitive load leads to missed bills. *(Strategy: Automated bill sweeps & zero-friction UI defaults)*
4. **The Exhausted Convenience Spender**: High fatigue drives heavy delivery usage. *(Strategy: Convenience tax calculation & micro-savings offsets)*
5. **The Quantified-Self Optimizer**: Data-driven biohacker. *(Strategy: Avalanche debt optimization & dual-axis correlation charts)*

---

## ⚙️ Technical Architecture & Pipeline
The project is structured around a modular Python backend notebook (`nudge_pipeline.ipynb`) that handles local persistence, decision logic, and data analysis:

* **Persistence Layer**: Dual SQLite databases (`nudge_telemetry.db` and `nudge_actions.db`) for lightweight, zero-config local archival of user check-ins and executed financial actions.
* **Data Fusion Engine**: Pandas processes synthetic banking transactions and cross-references them against a computed **Cognitive Load Index (0–100)** derived from daily mental telemetry.
* **Mock Open Banking API**: Simulates secure financial routing endpoints (e.g., Plaid/Finicity) to execute balance sweeps and micro-payoffs automatically.
* **Dashboard Aggregator**: Compiles multi-modal success metrics (mental health trends vs. financial execution totals) into a centralized executive view.

---

## 📂 Repository Structure
```text
/
├── README.md                  # Project overview and documentation
├── nudge_pipeline.ipynb       # End-to-end Python backend notebook
└── docs/
    └── data_dictionary.md     # SQLite schemas and data models
