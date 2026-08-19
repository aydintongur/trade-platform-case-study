# Trade Platform — Architecture Case Study

*Case study write-up in progress — replace this file with the full text.*

This repo holds the supporting material for an architecture case study
on a B2B trade brokerage platform I built: a Next.js/Supabase app
handling partner onboarding, product matching, deal pipelines, and
commission tracking, with an emphasis on database-enforced security
(row-level security, `SECURITY DEFINER` access control, anonymization
by construction) and empirical verification over assumption.

The underlying codebase is private. This repo contains only:

- **[`code-samples.md`](code-samples.md)** — six short, self-contained
  excerpts illustrating specific engineering decisions (identity
  resolution, database-enforced business rules, anonymization, match
  scoring, currency-safe arithmetic, and a real access-control incident
  and its fix).
- **[`screenshots/`](screenshots)** — eight screenshots of the running
  application (admin and partner-facing), using seed/demo data only.

## Contents

| # | Screenshot | Shows |
|---|---|---|
| 1 | `01-center-overview.png` | Admin overview: deal pipeline, pending commission, needs-attention |
| 2 | `02-center-deal-pipeline.png` | Deal kanban across pipeline stages |
| 3 | `03-center-matching-queue.png` | Matching queue with score breakdown |
| 4 | `04-center-deal-timeline.png` | Deal stage history |
| 5 | `05-center-deal-commission.png` | Commission split, marked paid |
| 6 | `06-partner-anonymous-pool.png` | Anonymized opportunity pool (partner view) |
| 7 | `07-partner-quick-offer-form.png` | Partner quick-listing form |
| 8 | `08-partner-deal-view.png` | Partner deal view (role shown, counterparty never is) |
