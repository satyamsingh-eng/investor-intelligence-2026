# C3A LABS — INVESTOR INTELLIGENCE 2026

Dual-track realistic investor targeting system for C3A Labs / SARVAX.
Replaces the celebrity-heavy targeting model with a realism-first model:
current authority, demonstrated pre-seed/seed deployment, AI/B2B/fintech
thesis, small-team tolerance, and a real access path.

## Mission

Find decision-makers who actively invest in product-first, small-team AI
companies at pre-seed/seed, and who are reachable by C3A Labs — not
prestige profiles with no plausible route to a check.

## Structure

```
INVESTOR-INTELLIGENCE-2026/
├── README.md                      ← this file
├── index.html                     ← master entry: mission + both sections
├── 00-SYSTEM/
│   ├── EVIDENCE_STANDARD.md       ← confidence levels, anti-fabrication rules
│   ├── SOURCE_REGISTER.md         ← every source URL used, with status
│   ├── CORRECTIONS_LEDGER.md      ← conflicts and corrections vs prior reports
│   ├── EXTERNAL-CONTROL-SET.md    ← India/global routes kept outside the two tracks
│   └── external-control-set.html  ← rendered appendix for the control set
├── CORNELL/
│   ├── index.html                 ← Cornell track report
│   └── DATA/
│       ├── INVESTOR_MASTER.csv
│       └── PEOPLE_MASTER.csv
├── MIT/
│   ├── index.html                 ← MIT track report
│   └── DATA/
│       ├── INVESTOR_MASTER.csv
│       └── PEOPLE_MASTER.csv
```

## Track separation

Cornell and MIT are separate reports for separate readers. The index page
carries the master summary and links into both. No cross-contamination of
records: a Cornell row never appears in the MIT dataset, and vice versa.

## Realism gate (applied before any firm or person is ranked)

1. Current investment authority — partner/principal with a live fund role.
2. Demonstrated pre-seed/seed deployment — named recent deals, 2024-2026.
3. AI/B2B/enterprise/fintech/agent relevance — thesis or portfolio evidence.
4. Small-team and product-first tolerance — fund stage and check size fit.
5. Real access path — warm intro, public application, or verified contact.
6. Cornell or MIT affiliation kept as an access signal, never as a
   substitute for stage or thesis fit.

## Evidence separation (never blurred)

- University affiliation evidence (official university page or fund page)
- Current role and identity evidence (official firm page)
- Firm stage evidence (official fund page / portfolio page)
- AI thesis evidence (official thesis page / named portfolio)
- Contactability evidence (Apollo work email + LinkedIn, verified only)
- Warm-introduction and access evidence (named program, board, class)

Apollo corroborates identity and contact only. It never proves affiliation,
investment authority, thesis, stage, or check size.

## Contact gate

A person appears on the people board only with BOTH a verified LinkedIn and
a confirmed email. Failures are removed or replaced; firm-level mentions
stay labeled with the honest status.

## Public edition = contact-minimized

Work email, role, and LinkedIn only. No phones, no personal emails, no
Apollo IDs, no raw payloads.
