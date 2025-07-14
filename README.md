# 🎰 Roulette Strategy Simulation

This project simulates and analyzes commonly used betting strategies in **European Roulette**, using a Jupyter Notebook and Monte Carlo methods. The goal is to understand the mathematics behind each strategy and their long-term impact on bankroll and risk.

📄 **Report:** [Roulette Strategy Summary.pdf](./Roulette%20Strategy%20Summary.pdf)

---

## 🧠 Strategies Covered

- **Flat Betting**  
  - Bet the same amount each round.
  - Low variance, but guaranteed long-term loss due to house edge.
  - EV ≈ –0.028 units per spin.

- **Martingale Strategy**  
  - Double the bet after every loss, reset after a win.
  - Recovers all previous losses +1 unit if win happens.
  - Extremely risky due to exponential bet growth.  
  - Ruin is likely on long losing streaks.

- **Anti-Martingale (Reverse Martingale)**  
  - Double the bet after a win, reset after a loss.
  - Capitalizes on winning streaks.
  - Safer than Martingale, works well with a win cap / exit strategy.
  - Still negative EV but with better risk control.

- **Kelly Criterion**  
  - Uses probability theory to calculate optimal bet fraction:
    - `f = (bp - q) / b`
    - For roulette, EV is negative ⇒ `f < 0` ⇒ don't bet.
  - Kelly advises not betting at all in a negative EV game.

---

## 📊 Insights from the Report

- No betting system can beat the house edge in the long run.
- Martingale leads to large losses quickly.
- Anti-Martingale + profit targets performs best short-term.
- Kelly mathematically confirms that roulette is unwinnable over time.

---

## 📁 Project Structure

```text
roulette-simulation/
├── Roulette.ipynb                # Jupyter Notebook with strategy simulations
└── Roulette Strategy Summary.pdf # Detailed written analysis, graphs, and formulas
```

---

## 🚀 How to Run

1. **Install Jupyter** (if not installed):
   ```bash
   pip install notebook
   ```

2. **Start the notebook**:
   ```bash
   jupyter notebook Roulette.ipynb
   ```

3. **Run cells step-by-step** to simulate:
   - Flat betting
   - Martingale & Anti-Martingale
   - Kelly Criterion
   - Probability of ruin
   - Monte Carlo bankroll projections

4. **Outputs:**
   - Graphs: bankroll curves, ruin probability
   - ROI comparisons
   - Confidence intervals

---

## 📷 Visuals (from the PDF)

- 📈 Bankroll over 100 spins for Anti-Martingale
- 🎯 Ruin probability over time
- 📊 Histogram of bankroll outcomes
- 🔄 Comparison of different strategies’ volatility

---

## 🧑‍💻 Author

Made by **Adityavardhan Iyengar**  
📘 Read the full analysis in the attached [`Roulette Strategy Summary.pdf`](./Roulette%20Strategy%20Summary.pdf)

---

## 📄 License

MIT License – you are free to use, modify, and distribute this for personal or academic use.
