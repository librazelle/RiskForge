# RiskForge

RiskForge is a standalone, responsive trading-risk dashboard. It is deliberately different from Trade Lens: Trade Lens focuses on trade context and review, while RiskForge focuses on pre-trade position sizing, rule guardrails, execution discipline, and risk scenarios.

## Features

- Futures position sizing for MNQ, MES, NQ, ES, MYM, and YM using each contract's point value and tick size.
- Risk budget, estimated stop risk, target reward, risk-to-reward, and break-even win-rate calculation.
- Contract-count guardrail for FundedNext Futures Flex 50K: 3 E-mini or 30 Micro contracts. Mixed positions use the firm's 1:10 equivalence rule; this single-instrument calculator caps the selected contract type accordingly.
- ICT 2022 / IFVG pre-trade checklist.
- 13-trade result tracker with a rule-following flag, a loss pause alert, and a win-streak reminder.
- Consecutive-loss drawdown table and 500-run Monte Carlo simulation for 50-trade paths.
- Local-browser persistence for inputs, checklist, and trade tracker. No account connection, backend, or API key is required.

## Run locally

Open `index.html` in a modern browser. The repository can also be hosted with GitHub Pages.

## Important limitations

- Risk estimates exclude commissions, slippage, gaps, and execution failures. A contract cap is not a drawdown guarantee.
- Verify multiplier, tick size, tick value, and prop-firm rules for your broker and account before trading. Official FundedNext Futures rules: https://helpfutures.fundednext.com/en/articles/17229848-fundednext-futures-flex-fundednext-account-all-rules
- The ICT checklist is a process reminder, not a validated probability model or trade signal.
- Monte Carlo results are randomized illustrations based on user-entered assumptions. Outcomes are assumed independent; real markets have changing regimes and correlated losses. The simulation does not validate the entered win rate.
- Tracker data and settings are stored only in the current browser's local storage and do not sync between devices.

## License

MIT
