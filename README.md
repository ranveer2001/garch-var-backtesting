## Key Results

### Backtesting Performance
- Kupiec Test Statistic: **2.13**
- Christoffersen Test Statistic: **0.79**

Interpretation:
- Both tests suggest that VaR violations are broadly consistent with model assumptions (no strong evidence of misspecification at typical critical levels).

---

### Risk Estimates (99% Confidence Level)

| Metric | Value |
|------|------|
| Portfolio VaR | -2.61% |
| Portfolio Expected Shortfall (ES) | -2.94% |
| EWMA VaR | -2.40% |
| EWMA ES | -2.78% |

---

### Stress Testing (COVID-like Shock Scenario)

| Metric | Value |
|------|------|
| Stress VaR | -4.18% |
| Stress ES | -4.79% |

---

### Final Risk Summary
- Portfolio VaR (99%): **-2.61%**
- Portfolio ES (99%): **-2.94%**
- Stress VaR: **-4.18%**
- Stress ES: **-4.79%**

---

### Key Insight
- EWMA model produces lower (less conservative) VaR than full portfolio historical estimation.
- Stress scenario significantly increases tail risk, with losses ~1.6× higher than normal VaR.
- ES consistently exceeds VaR, confirming heavier tail loss behavior.

## Visual Results

### 1. EWMA Portfolio Risk Distribution
![EWMA Distribution](results/EWMA%20Portfolio%20Risk%20Distribution.png)

Shows the distribution of portfolio returns under EWMA volatility modeling.

---

### 2. GARCH VaR Backtest (Student-t)
![GARCH VaR Backtest](results/GARCH%20VaR%20Backtest%20(Student-t).png)

Demonstrates VaR violations under heavy-tailed Student-t assumptions.

---

### 3. Monte Carlo Return Distribution
![Monte Carlo](results/Portfolio%20Monte%20Carlo%20Return%20Distribution.png)

Simulated return distribution capturing tail risk under stochastic scenarios.