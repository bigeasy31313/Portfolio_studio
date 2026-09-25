# ARBX

## ARBX: sportsbook arbitrage terminal

`arbitrage/index.html` is a self-contained app (no build step; open it in a browser):

- **Scanner**: finds arbitrage (2-way, 3-way, spreads, totals), middles, and +EV bets priced against a sharp no-vig line.
- **Stake optimizer**: equal-profit stakes, a risk-free bias slider, anchor-a-leg for max-bet limits, and round-number stakes chosen by best worst-case ROI.
- **DEMO** mode runs a simulated 14-book market. **LIVE** mode pulls real odds from [The Odds API](https://the-odds-api.com). Add your key under Settings; it is stored only in your browser.
- **Books**: track what's in each sportsbook account. The scanner shows how much of each arb you can fund, the optimizer caps legs at book balances, logging or settling a bet debits and credits the right books, and a rebalance plan tells you where to withdraw and deposit. ARBX never holds or moves money; you fund each book and place bets yourself.
- **Recommended moves**: a ranked list of what to do next. It covers the best arb you can fund right now (and which leg to place first), which book to top up based on profit you missed, low balances, rebalancing, bets waiting to be settled, top +EV and middle spots, and warnings about account limits.
- Also includes a calculator, odds converter, no-vig tool, bet ledger with equity curve and CSV export, and a guide.
