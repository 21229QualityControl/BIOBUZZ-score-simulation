# BIOBUZZ Score Simulation

A standalone Monte Carlo simulator for comparing FTC BIOBUZZ Hive-scoring strategies.

It compares a Pollen-only primary robot with a primary robot capable of intaking and shooting both Pollen and Nectar, including:

- Shared primary-robot settings that apply to every simulation
- Reusable primary strategy configurations for targeted Nectar count and added cycle time
- Reusable partner cycle/load configurations with shared partner accuracy and jitter settings
- Automatic generation of every primary-strategy × partner combination
- Batch shooting accuracy
- Partner robot contribution
- The four-piece control limit
- The 8-Pollen / 5-Nectar Hive tipping model
- Nectar recycling after a Hive tip
- One-Nectar-per-tip introduction before the final minute
- Release of all remaining Nectar at 1:00
- Expected tips, points, outcome probabilities, and probabilities of reaching at least 7, 8, or 9 tips

Hive score is modeled as 20 points per tip plus 2 points for each ball left in the active Cell when TELEOP ends.

The central result from the default scenarios is that same-speed Nectar capability becomes extremely valuable if a future ranking-point requirement demands more Hive tips. A two-second Nectar cycle penalty removes much of that advantage; when targeting only two Nectar per cycle, the slower dual strategy often scores fewer points than remaining Pollen-only.

## Run it

Open `index.html` in a browser. The simulator has no build step, server, or external dependencies.

The included values are editable starting assumptions, not predictions of actual field performance. Validate the tipping and shooting assumptions with real game pieces and an official field element.

Public page-load and completed-simulation counters are provided by the hosted GoatCounter service. Each page load and simulation run is counted independently; displayed totals may be cached for up to four hours.
