---
layout: page
title: Private Debt Calculator 
summary : Simple debt payoff calculator in Streamlit
date: 2025-08-08
---

[🔗 View the full project on GitHub](https://github.com/kgadgil/financial-planner)

---

### Take Charge of Your Debt — Locally, Instantly, Intelligently

**1. 100 % local, 100 % private**
The Multi-Debt Payoff & What-If Calculator is a pure-Python Streamlit app that runs entirely on your own machine. No cloud back-end, no account sign-ups, no APIs pinging who-knows-where—your balances, interest rates and “what-if” scenarios never leave your laptop. Close the tab, and your data stays offline with you.

**2. Numbers in seconds, not hours**
A clean sidebar lets you paste—or CSV-import—every credit card, loan or line of credit you have. Click **Edit → Save**, and the dashboard instantly shows payoff time, total interest and a live balance curve. Want to see the impact of an extra \$50 a month, or a lower refi rate? Two clicks and the chart redraws. Because the math is vectorised in Pandas and rendered by Streamlit, results feel instantaneous—perfect for those “Can I afford this?” moments.

**3. A quick pulse-check on financial health**
Seeing *all* your debt on one screen—plus how much interest you’re saving by paying more than the minimum—turns vague anxiety into concrete insight. The app’s aggregate metrics act like a blood-pressure cuff for your finances: payoff horizon, interest saved, and monthly-payment load give a clear snapshot of where you stand today and what it will take to get debt-free.

**4. Where this can go next**
Today the app crunches the numbers you feed it. Tomorrow, it could *read* them for you. Hooking an LLM to the back-end would let you:

* Drop in a PDF or email statement and have the model extract balance, APR and minimum-payment fields automatically.
* Ask natural-language questions—“What’s my earliest debt-free date if I add \$100 to the car loan?”—and get answers without touching a slider.
* Spot anomalies (“Your Visa rate just jumped by 2 %; want to simulate a balance transfer?”).

With your core payoff engine already rock-solid and test-covered, layering AI on top becomes the logical next sprint.

---

**Ready to try it?**

```bash
git clone <repo>    # or copy the single file
pip install streamlit pandas numpy
streamlit run app.py
```

Decisions are easier when the numbers are clear—and clearer still when they never leave your device.
