# EVIDENCE STANDARD

## Confidence levels

| Level | Meaning | Rule |
|---|---|---|
| CONFIRMED | Two+ independent primary sources agree (official firm page + university page, or firm page + funding announcement) | Reportable as fact |
| LIKELY | One strong primary source, or primary + weak secondary | Reportable with the label |
| POSSIBLE | Single weak/secondary source only | Reportable only as lead |
| NOT VERIFIED | Nothing found, or sources conflict unresolved | Must be labeled; never used for outreach ranking |

## Source hierarchy (strongest first)

1. VC official website / partner bio / portfolio page
2. Funding announcement (company or fund press release)
3. University official source (tech.cornell.edu, mitsloan.mit.edu, entrepreneurship.mit.edu)
4. SEC Form D / ADV filings
5. Reputable financial/tech press (named reporter)
6. LinkedIn (discovery signal ONLY — not proof of role or affiliation)
7. Apollo (contact enrichment ONLY — proves nothing about thesis, stage, or affiliation)

## Anti-fabrication rules (absolute)

- **CONTACT GATE:** a person appears on the people board or contact register
  only with BOTH a verified LinkedIn AND a confirmed email (Apollo-verified
  or publicly posted). Failures are removed or replaced. Firm-level mentions
  of such people remain, labeled with the honest status.
- No guessed emails. Only publicly posted org inboxes or Apollo
  `email_status: verified`.
- No invented LinkedIn URLs. Only from official team pages or Apollo-returned
  `linkedin_url`.
- No assumed university degrees. The university name must appear in a
  verifiable official bio or news source.
- No assumed investment activity. Portfolio pages or announcements only.
- No assumed stage fit. Current fund focus or named recent deals only.
- Old titles and deals are not current. Every role and deal claim is dated.
- Not found = NOT FOUND. Never substitute a lookalike.

## Apollo boundary

Apollo corroborates a current database record (identity, title, employer,
LinkedIn anchor). It does NOT prove: university affiliation, investment
activity, AI thesis, fund stage, check size, or decision rights. It is never
evidence for those fields.

## Apollo synthetic echo stub detection

When queried for a person absent from Apollo's database, the enrichment
endpoint returns `successful: true` with a synthetic stub that echoes the
input name alongside a generated ID but sets `title: null`,
`organization_id: null`, `linkedin_url: null`, and `employment_history: []`.
Any record with all null anchor fields is classified `no_match` and never
treated as a match.

## Corrections ledger

Every research wave is diffed against the prior system. Conflicts,
corrections, and new findings are recorded in
`00-SYSTEM/CORRECTIONS_LEDGER.md`. The ledger overrides conflicting sprint
files. Contradictions are reported with both sides — never silently
resolved.
