# Support KPI and staffing calculator

**Live page:** https://mika-dulata.github.io/support-kpi-calculator/

How many agents do you need once an AI assistant takes its share? And how much of that share is actually solved?

## What it calculates

- **Agents on shift** for your service level target, using Erlang C on the human queue.
- **Human queue** = conversations the bot hands over + "contained" conversations that weren't solved and come back.
- **Real containment** = reported containment × verified solved rate.
- **Cost per verified resolution** = (agent hours + AI usage) ÷ problems actually solved.
- Occupancy, average wait and a small table of service level by headcount.

## Assumptions

- Erlang C assumes nobody abandons the queue.
- Chat concurrency is a simple divisor of handle time, which is optimistic.
- Conversations handled by a person count as 95% solved.
- No skills routing, languages or separate P1 security queue. Size that one on its own.

Defaults are illustrative and don't come from any company. Everything runs in the browser, one HTML file, no tracking.

Related: [Handoff playbook](https://mika-dulata.github.io/support-handoff-playbook/) · [Self-custody support lab](https://mika-dulata.github.io/support-lab/) · [LinkedIn](https://www.linkedin.com/in/meruyert-nurkaliyeva)

MIT License · Meruyert Nurkaliyeva
