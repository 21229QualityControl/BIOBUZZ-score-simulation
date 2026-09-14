# BIOBUZZ Score Simulation

A standalone Monte Carlo simulator for comparing FTC BIOBUZZ Hive-scoring strategies.

It compares a Pollen-only primary robot with a dual-size robot that targets Nectar, including:

- Variable robot cycle times
- Same-speed and +2-second Nectar-cycle comparison presets
- Batch shooting accuracy
- Partner robot contribution
- The four-piece control limit
- The 8-Pollen / 5-Nectar Hive tipping model
- Nectar recycling after a Hive tip
- One-Nectar-per-tip introduction before the final minute
- Release of all remaining Nectar at 1:00
- Expected tips, points, outcome probabilities, and probabilities of reaching at least 7, 8, or 9 tips

Hive score is modeled as 20 points per tip plus 2 points for each ball left in the active Cell when TELEOP ends.

The central result from the default scenarios is that same-speed Nectar capability becomes extremely valuable if a future ranking-point requirement demands more Hive tips. Even a two-second Nectar cycle penalty removes much of that advantage.

## Run it

Open `index.html` in a browser. The simulator has no build step, server, or external dependencies.

The included values are editable starting assumptions, not predictions of actual field performance. Validate the tipping and shooting assumptions with real game pieces and an official field element.
