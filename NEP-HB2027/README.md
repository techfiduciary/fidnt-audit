# NEP-HB2027 — FIDNT contribution to the FY 2027 budget-review commons

A standard-contribution node: FIDNT's independent verification pass on the Department of
Public Works and Highways (DPWH) lines in **HB 10858 (House General Appropriations Bill,
FY 2027)** against the **2027 NEP**, published in the formats and under the discipline the
coalition's datasets already use.

**Live page:** <https://techfiduciary.github.io/fidnt-audit/NEP-HB2027/>

## Stage and units statement (read first)

- **Stages compared:** the 2027 NEP (as filed, identical to GAB_FILED) vs **HB 10858 House
  bill project lists**. The first pass under review states its dataset reads as 2nd reading
  while the printed volumes show 3rd-reading footers — **that reading is unconfirmed and we
  flag it rather than resolve it.**
- **Units:** all figures below are **billions of pesos (₱B)**, project level, as aggregated
  by the source passes. Source documents print in thousands; no additional conversion was
  applied by FIDNT beyond the sources' own.
- **Scope:** DPWH project lists only. No whole-budget, MOOE, or special-provision analysis
  is claimed here.

## What we verified (aggregate)

| Finding | Value | Source basis |
|---|---:|---|
| DPWH additions — local projects | +₱87.2B | four-pile sort, project level |
| DPWH removals — foreign-assisted | −₱73.0B | four-pile sort, project level |
| Net change, DPWH | +₱11.5B | sum of the piles |
| House-bill projects not in NEP | 6,033 (₱165.6B) | project match, mostly access roads + multi-purpose buildings |
| NEP projects dropped | 1,160 (₱68.4B) | project match |
| Lines paying for an object the same bill already pays for | 17 (₱3.1B) | named-case review (see `findings.csv`) |
| New farm-to-market roads | 353 (+₱5.92B), **no stated length on any line** | drilldown items |
| NIA new lines | 145 (+₱5.74B) replacing 108 dropped; pump-station repair ₱3.0B → ₱0.46B | drilldown items |
| New DPWH money not placeable to a district | ₱37.8B | geo attribution gap |

## Method (so it can be repeated)

1. Lay the two project lists side by side (NEP vs House bill).
2. Sort every project into four piles: unchanged / raised-or-cut / added by the House /
   removed by the House.
3. Sum each pile; reconcile to the printed bill totals.
4. For duplications: exact-amount and same-object review across the bill's own volumes —
   a **screening lead, not a finding of wrongdoing**; package/phase/lot/segment differences
   are ambiguous 50/50 signals and were not treated as scope identity.
5. Report provisional results with named, page-cited cases; everything else stays an
   aggregate until it can be tied to a printed line.

## Caveats we adopt (from the coalition's own discipline)

- "Not in the NEP" does not prove a project is improper; some are renamed NEP items.
- Candidate matches and deltas are **provisional**; unmatched rows are not proof of policy
  change.
- Districts are inferred from engineering offices and town names; the ₱37.8B unplaced money
  is the measure of that inference's limit.
- Flags and thresholds are starting points, not editorial standards.
- Validate every lead against the original documents before filing anything anywhere.

## Files

- `index.html` — the contribution page (same content, publishable form).
- `findings.csv` — the named, page-cited duplication cases and the aggregate ledger
  (CC BY 4.0, attribution table below).

## Sources (cite if you use this)

- **House Insertions 2027 — First Pass** (S. Lava, BetterGov × People's Budget Coalition,
  10 Oct 2026) — four-pile sort and aggregates.
- **kimileeee/gab-fy2027-dataset** v0.1.0 (2026-10-09) and its `DATA_DICTIONARY.md` — stage
  taxonomy and table discipline this contribution follows.
- **csiiiv/DPWH-NEP-HB-2027-ANALYSIS** — three-stage comparison workbench; HB volumes I-B/I-C;
  NEP Vol. II-B snapshot (SHA-256 recorded).
- **research.bettergov.ph — DPWH FY2027 NEP Patterns** (11,372 entries; 90%+ title-similarity
  screening; "review list, not a finding of wrongdoing").
- **AJ Montesa, "The FY 2027 House GAB: An Assessment"** (People's Budget Coalition) —
  ₱116.3B / ₱202B cross-budget context.
- **House bill PDFs (Vol. I-B, I-C) and the NEP (CR 638)** — print of record.

## License

FIDNT's own findings in this folder are **CC BY 4.0** (attribute "FIDNT audit node —
fidnt-audit/NEP-HB2027"). Upstream datasets remain under their respective terms; no upstream
data file is republished here.
