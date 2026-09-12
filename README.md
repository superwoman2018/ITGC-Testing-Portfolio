[README.md](https://github.com/user-attachments/files/32143547/README.md)
# ITGC Testing Portfolio

Sample-based tests of IT General Controls, built to demonstrate the actual
mechanics of ITGC testing — walkthrough, population, sample, attributes,
exceptions, conclusion — the way it's performed in a real IT audit engagement.

## Why this exists

GRC work (policy, risk registers, control mapping) and IT audit work
(testing whether a control actually operated, on a sample basis, across a
period) are different skills. This repo is specifically about the second one:
proving a control worked — or didn't — using real testing methodology, not
just describing what the control is supposed to do.

Every project here is built against the same fictional company, CloudNative,
used in my broader GRC portfolio
([grc-portfolio-2026](https://github.com/superwoman2018)), so the underlying
business context is consistent across both repos.

## ITGC Domains Covered

| # | Domain | Status |
|---|---|---|
| 01 | Change Management | Complete — see folder for full walkthrough and 25-sample test |
| 02 | Access Management | Planned |
| 03 | Computer Operations (backups, batch monitoring) | Planned |
| 04 | Program Development / SDLC | Planned |

## How each project folder is structured

```
0X-domain-name/
├── README.md          # what's in the folder and how to read it
├── scenario.md         # why this domain, and the judgment calls behind it
└── deliverables/
    ├── ..._Walkthrough.docx     # control objective, design walkthrough, conclusion
    └── ..._Test_Sample.xlsx     # the actual sample-by-sample testing workpaper
```

## Disclaimer

This is a portfolio exercise for a fictional company — not a real audit
engagement, and not a substitute for testing performed under a real audit
firm's methodology and quality standards.

## About me

Maimoona Iqbal — GRC professional, CISA certified. Connect on
[LinkedIn](https://www.linkedin.com/in/maimoonaiqbal/) · More write-ups on
[Medium](https://medium.com/@maimoona2018).
