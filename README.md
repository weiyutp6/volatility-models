# Volatility Models

Three notebooks on volatility and option pricing.

| Notebook | Content |
|---|---|
| `GARCH.ipynb` | GARCH expressed as a small neural network (two hidden layers) trained on the Gaussian log-likelihood, with a tenor-matched 20-day volatility forecast and a GARCH(1,1) baseline from the `arch` package. |
| `MCSim.ipynb` | GARCH(1,1) Monte Carlo of an unleveraged position against a daily-rebalanced 3x leveraged one, with Sharpe, Sortino, Calmar and maximum drawdown. |
| `option_price.ipynb` | Black-Scholes pricing, put-call parity, and a Greeks-based price estimate from an option chain pasted as text. The quotes in the notebook are a made-up example. |

Price files are not included. The GARCH notebook reads Investing.com-style CSVs with `Date` and `Price` columns.

```bash
pip install numpy pandas torch scikit-learn arch mpmath matplotlib
```

For research and education only. Not investment advice.
