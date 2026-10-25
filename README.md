# RiskForge

RiskForge is a standalone, browser-based trading risk dashboard. It is intentionally distinct from Trade Lens: Trade Lens is about trade context and review; RiskForge focuses on pre-trade risk sizing, loss-streak scenarios, process discipline, and randomized equity-path experiments.

## Features

- Position sizing from account balance, risk percentage, entry, stop, target, and a user-defined contract multiplier.
- Risk/reward, planned cash risk, planned reward, and break-even win-rate estimate.
- Drawdown scenarios for consecutive losses, including recovery return required.
- 13-trade batch tracker with result and rule-following fields, saved in local browser storage.
- 50-trade Monte Carlo path simulation with estimated expectancy, final equity, and maximum peak drawdown.
- Responsive layout for desktop and mobile; no server or API key required.

## Run locally

Open `index.html` in a modern browser. The app is static and can also be hosted on GitHub Pages.

## Important limitations

- This is an educational calculator, not investment advice or a broker-connected trading terminal.
- Contract multipliers and lot sizing differ by broker and instrument. Verify contract size, tick value, lot increment, account currency, fees, and slippage before using any result.
- Monte Carlo uses randomized independent outcomes based on user-entered assumptions. It is not a forecast and does not model changing market regimes.
- Trade tracker data is stored in the current browser's local storage and does not sync between devices.

## License

MIT
