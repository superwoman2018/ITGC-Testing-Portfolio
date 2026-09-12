[scenario.md](https://github.com/user-attachments/files/32143601/scenario.md)
# Scenario

**Organization:** CloudNative (fictional) — same company as the other five
portfolio projects.
**Objective:** Perform an actual ITGC test of controls — not study ITGC in
the abstract, but produce a walkthrough, a sample, and a conclusion the way a
Big 4 IT audit associate actually would.

## Why Change Management, specifically

Change Management is usually the first ITGC domain a new IT audit associate
gets assigned, because it's high-frequency (meaning a real sample, not just
one transaction) and because the design-vs-operating-effectiveness
distinction shows up clearly here: CloudNative's CI/CD pipeline is
*structurally* well-designed — branch protection rules make it hard to
deploy without an approving review. That's a design conclusion. Whether it
actually operated that way for 260 real deployments across a quarter is a
separate question, and it's the one this exercise actually tests.

This also connects back to Project 04 (GRC Control Automation), which
referenced CloudNative's change management record (EV-025) as an evidence
source — this project is what actually interrogates that evidence rather than
just citing that it exists.

## Why the sample has two exceptions instead of zero

A clean 25-for-25 result would be a worse portfolio piece, not a better one —
it would read as either an artificially easy sample or a reviewer who didn't
look hard enough. Real ITGC testing at this frequency almost always turns up
something. The two exceptions here are deliberately different in kind:

- **Sample #14** is an evidence-retention problem, not a control-failure
  problem — the approval was real and timely, but the CI log proving the test
  ran had already expired by the time of testing. The report is explicit about
  that distinction, because conflating "we can't prove it happened" with "it
  didn't happen" is a common overreach in real audit work, and drawing that
  line correctly is part of the actual skill.
- **Sample #25** is a genuine timeliness miss — the emergency-change SLA was
  breached, not just barely but by 16 hours. This one doesn't get softened;
  the substance of the change was fine (a real incident, a real fix), but the
  control as documented wasn't met, and the conclusion says so plainly.

## The conclusion is the hardest part to get right

A 2-of-25 exception rate (8%) is a judgment call, not a formula: is that
"operating effectively with exceptions noted," or is it pervasive enough to
conclude the control failed? I concluded the former — both exceptions are
narrow, specific, and fixable, and neither points to a systemic breakdown in
the underlying control design. A different reviewer might reasonably set the
threshold differently. That's the actual conversation a senior reviewer would
have with an associate presenting this workpaper, and it's the part of this
exercise most worth being able to defend out loud.
