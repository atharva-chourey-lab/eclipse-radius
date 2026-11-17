# SOURCES.md — Paper 3: Eclipse-radius re-reduction

Author: Atharva Chourey
Affiliation: Atharva Chourey Lab (independent research lab)

Status: Manuscript in preparation — not yet peer-reviewed.

Paper file: `paper.md` (this directory)
Project sources root: `~/workspace/eclipse-radius/`
Precedent sweep: `~/workspace/papers/precedent-sweep/SWEEP.md`

Rule applied throughout: every quantitative claim in the paper traces to a number in the files below. Where a needed number is not in the sources, the paper says so explicitly (§4.2, item 10) and no number is supplied.

---

## 1. Headline numbers — value as used, and exact source

| # | Quantity | Value as used in paper | Source file (section) |
|---|---|---|---|
| 1 | Corrected mean radius (Q2) | 959.494 ± 0.044″ (SE) | `RESULTS.md` headline results + §5; verified in `outputs/q1_q2_results.json` (`q2.R_mean_arcsec` = 959.4941078, `q2.R_se_arcsec` = 0.0443479) |
| 2 | Median-based radius | 959.481″ | `RESULTS.md` §5; `outputs/q1_q2_results.json` (`q2.R_median_arcsec` = 959.4808607) |
| 3 | Mean Watts→LOLA correction δ̄ (±15° merged) | +0.100″ | `RESULTS.md` headline results + §3. Lab recomputation from `outputs/corrected_series.csv` (`delta_bar_w15`): mean +0.0996″, n = 27 |
| 4 | Per-event δ̄ range | −0.003″ to +0.194″ | `RESULTS.md` headline results; recomputed from `outputs/corrected_series.csv` (min −0.00346, 2002-12-04; max +0.19385, 1979-02-26) |
| 5 | South-window mean δ̄_S | +0.271″ (every event positive; range +0.136…+0.353″) | `RESULTS.md` §3; recomputed from `outputs/corrected_series.csv` (`delta_bar_S_w15`): mean +0.2706″, min +0.1357″, max +0.3531″ (1912-04-17) — agrees with RESULTS.md |
| 6 | North-window mean δ̄_N | −0.071″ (range −0.179…+0.072″) | `RESULTS.md` §3; recomputed from `outputs/corrected_series.csv` (`delta_bar_N_w15`): mean −0.0715″, min −0.1793″, max +0.0723″ |
| 7 | South−north asymmetry | +0.34″ | `RESULTS.md` headline results (S−N asymmetry +0.34″) |
| 8 | Q1 published: scatter / Spearman ρ / p | 0.237″ / −0.193 (≈ −0.19) / 0.336 (≈ 0.34) | `RESULTS.md` §4 table; `outputs/q1_q2_results.json` (`published`: 0.237216, −0.192701, 0.335552) |
| 9 | Q1 corrected (±15°): scatter / ρ / p | 0.196″ / −0.245 (≈ −0.24) / 0.218 (≈ 0.22) | `RESULTS.md` §4 table; `outputs/q1_q2_results.json` (`corrected_w15`: 0.196000, −0.244848, 0.218357) |
| 10 | Q1 corrected (±7.5° / ±30°): scatter, ρ, p | 0.205″, −0.273, 0.169 / 0.194″, −0.226, 0.257 | `RESULTS.md` §4 table; `outputs/q1_q2_results.json` (`corrected_w7p5`, `corrected_w30`) |
| 11 | Scatter shrink, primary window | 17.4% (13–18% across windows) | `RESULTS.md` §4; `outputs/q1_q2_results.json` (`q1_scatter_shrink_fraction` = 0.173749) |
| 12 | Q1 lag diagnostics (±15°) | lag −1: ρ = −0.005, p = 0.98; lag +1: ρ = −0.299, p = 0.13 | `RESULTS.md` §4; `outputs/q1_q2_results.json` (`corrected_w15_lag-1`, `corrected_w15_lag+1`) |
| 13 | Q1 verdict | PARTIAL / MIXED (at every window width) | `RESULTS.md` §4; `outputs/q1_q2_results.json` (`q1_verdict`) |
| 14 | IOTA-era diagnostic (1970+, n = 20) | Scatter 0.208″ → 0.141″ (−32%); ρ −0.13 → −0.26, still non-significant | `RESULTS.md` headline results + §4; `outputs/q1_q2_results.json` (`diagnostic_1970plus_*`: 0.207564 → 0.141142; ρ −0.133935 → −0.257992; p 0.573 → 0.272) |
| 15 | Q2 window sensitivity | 959.488 / 959.494 / 959.508″ for ±7.5° / ±15° / ±30° | `RESULTS.md` headline results; verified from `outputs/q1_q2_results.json` means (959.63 + mean ΔR_corr) |
| 16 | Auwers standard | 959.63″ (1891) | `PREDICTION.md` §1, §3 (Q2 comparators); `RESULTS.md` §5 table |
| 17 | IAU 2015 nominal | 959.22″ (helioseismic; Prša et al. 2016) | `RESULTS.md` §5 table; `PREDICTION.md` §3 |
| 18 | Modern eclipse cluster centre | 959.97″; range 959.92–960.02″ | `RESULTS.md` §5 + §7 item 6; `PREDICTION.md` §3 |
| 19 | Lamy et al. 2015 | 959.99 ± 0.06″ | `RESULTS.md` §5 table; `NOVELTY_AUDIT.md` §(b) gives per-eclipse values and mean 959.99 ± 0.06″ |
| 20 | Quaglia et al. 2021 | 959.95 ± 0.05″ (2017 eclipse; LOLA SLDEM-256 + LDEM-128) | `RESULTS.md` §5 table; `NOVELTY_AUDIT.md` §(b) |
| 21 | Guhl 2023 | 960.01 ± 0.12″ (20 Apr 2023 hybrid) | `RESULTS.md` §5 table; `NOVELTY_AUDIT.md` §(b) |
| 22 | R̄ offsets | −0.136″ vs Auwers; −0.476″ (≈0.48) vs cluster; +0.274″ (≈0.27) vs IAU | `RESULTS.md` §5 table |
| 23 | Kubo context range | 959.74–959.88″ | `RESULTS.md` §5 table; `NOVELTY_AUDIT.md` §(b) (Kubo 1993) |
| 24 | Kilcik et al. 2009 (2006 eclipse) | 959.22 ± 0.04″ (ΔR = −0.41) | `RESULTS.md` §5; `data/PROVENANCE.md` §7; `outputs/crosscheck_sources.csv` (2006-03-29 row) |
| 25 | Corrected 2006 value | ΔR_corr = −0.014″ (R = 959.616″); 0.40″ above Kilcik et al. | `RESULTS.md` §5; `outputs/corrected_series.csv` (2006-03-29, `deltaR_corr_w15` = −0.01368) |
| 26 | Space-based cap | < 23 mas peak-to-peak (Bush, Emilio & Kuhn 2010, *ApJ* 716:1381); < 7 mas after correction (Kuhn et al. 2004) | `RESULTS.md` §4, §7 item 5; `NOVELTY_AUDIT.md` §(f) |

## 2. Cross-check numbers (§3.4–§3.5 of the paper)

| Quantity | Value as used | Source |
|---|---|---|
| Overlapping Fiala 1994 / Dunham 2016 events | 9 | `RESULTS.md` §6; `outputs/crosscheck_sources.csv` |
| Disagreements | 7 of 9 | `RESULTS.md` headline results + §6; count verified from `outputs/crosscheck_sources.csv` |
| Sign flips | 5 (1715, 1925, 1976, 1983-06-11, 1987-09-23) | `RESULTS.md` §6 table; `outputs/crosscheck_sources.csv` (rows flagged "SIGN FLIP") |
| 1715: Fiala vs Dunham | +0.48 ± 0.20 (3 obs) vs −0.50 ± 0.20 (3 obs); difference −0.98″ | `RESULTS.md` §6 table; `outputs/crosscheck_sources.csv` (1715-05-03 row) |
| 1925: Fiala vs Dunham | +0.51 ± 0.08 (8 obs) vs −0.21 ± 0.17 (11 obs); difference −0.72″ | Same as above (1925-01-24 row) |
| Remaining seven pairs | 1976: +0.04 / −0.38 (−0.42); 1987-09-23: −0.11 / +0.10 (+0.21); 1981: −0.02 / −0.21 (−0.19); 1983: +0.09 / −0.10 (−0.19); 1980: −0.03 / −0.18 (−0.15); 1979: −0.11 / −0.05 (+0.06); 1984: +0.09 / +0.13 (+0.04) | `RESULTS.md` §6 table; `outputs/crosscheck_sources.csv` |
| Hayakawa compiled values | 1925: 960.14 ± 0.08″ (ΔR +0.51); 1715: ≥ 959.91″ (ΔR ≥ +0.28) | `RESULTS.md` §6; `data/PROVENANCE.md` §7 |
| Hayakawa 1715 re-derivation | 959.98 ± 0.23″ (ΔR = +0.35) | `RESULTS.md` §2b, §6, §7 item 3; `NOVELTY_AUDIT.md` §(f) (arXiv:2604.24503) |
| 1715 through this pipeline | Fiala-based: 959.944″; Dunham-based: 958.964″; gap to modern re-derivation ≈ 1″ | `RESULTS.md` §6 ("The 1715 anchor, three ways") |
| 1715 implied vs pipeline limb correction | Implied +0.13″; pipeline δ̄(1715) = +0.166″; difference within 0.04″; without datum term +0.54″ | `RESULTS.md` §2b; `data/PROVENANCE.md` §3 |
| Fiala substitution — Q1 | Published scatter 0.163″, ρ = −0.285 (p = 0.150); corrected scatter 0.175″, ρ = −0.277 (p = 0.163); verdict unchanged | `RESULTS.md` §6; `outputs/q1_q2_results.json` (`fiala_substituted_*`) |
| Fiala substitution — Q2 | R̄ = 959.581″ (median 959.565″); |Δ| vs Auwers = 0.049 ≤ 0.06 (mean band); median 0.005″ outside its band | `RESULTS.md` §6; `outputs/q1_q2_results.json` (`fiala_substituted_q2`: 959.580774, 959.565347) |
| Table-choice effect on Q2 | ~0.09″; tables' mutual disagreement up to 0.98″ | `RESULTS.md` headline results + §6 |
| 1715–1979 pair | Fiala values: +0.48 vs −0.11 (0.59″, claimed direction); Dunham 2016 values: −0.50 vs −0.05 (inverts). 1980 claim as cited: "0.4″ shrinkage", Dunham et al. 1980, *Science* 210:1243 | `RESULTS.md` §6 |
| Post-1991 per-eclipse checks | 1994: Thompson/IOTA −0.27 ± 0.02 vs −0.25; 1999: +0.06 ± 0.06 vs −0.03; 2005: Sigismondi 0.00 ± 0.17 vs −0.06; 2006: Kilcik −0.41, Sigismondi ≈ 0.00…−0.01 ± 0.17 vs +0.09 | `RESULTS.md` §6; `outputs/crosscheck_sources.csv`; `data/PROVENANCE.md` §7 |
| Cross-check sources total | 13 events (9 Fiala; 1994/1999 Thompson-IOTA; 2005 Sigismondi; 2006 Kilcik + Sigismondi) | `RESULTS.md` §9 per-event source statement |

## 3. Methods numbers (§2 of the paper)

| Quantity | Value as used | Source |
|---|---|---|
| Archive size / span | 27 events, 1715-05-03 … 2006-03-29; IOTA-era subset 20 events | `data/PROVENANCE.md` §1; `data/dunham2016_table.csv` |
| Pre-registration | `PREDICTION.md`, git commit `a42d76a`, 2026-11-17, before data touched | `RESULTS.md` header |
| Bead windows | ±15° primary; ±7.5° / ±30° sensitivities; merged N+S | `PREDICTION.md` §2d; `RESULTS.md` §1 |
| Datum term (REFERENCE_TERM) | 0.3707″ (paper text also uses 0.371″ as in RESULTS.md §2b) | `outputs/q1_q2_results.json` (`reference_term_arcsec` = 0.370680); `scripts/correct_and_test.py` |
| Eclipse constant k / Earth radius / mean distance | k = 0.2725076; 6378.137 km; 384,398.55 km → mean-limb radius 1738.091 km | `RESULTS.md` §2b; `data/PROVENANCE.md` §3 |
| LDEM reference sphere | 1737.4 km | `RESULTS.md` §2b; `data/PROVENANCE.md` §3 |
| Watts frame convention | L at +l; B at −b; WA = AA + 0.21° (Scott 1988: 0.214°); Pearson r = 0.87–0.89; reversed-axis r < 0; wrong-L r ≤ 0.80 | `RESULTS.md` §2c; `outputs/q1_q2_results.json` (`watts_frame_convention`) |
| B-sign systematic | Mean shift 0.061″, max 0.148″ | `RESULTS.md` §2c, §8; `outputs/q1_q2_results.json` (`bsign_sensitivity`: 0.061210, 0.148249) |
| 2006 geometry validation | Computed greatest eclipse 10:11:18 UTC vs Espenak 10:11:17.6 UT (0.4 s) | `RESULTS.md` §1; `data/PROVENANCE.md` §4; `outputs/event_geometry.csv` |
| Watts grid specification | 91 L librations, 81 B librations, 1,800 Watts angles, 0.2° steps; VI/122 | `data/PROVENANCE.md` §2 |
| LDEM_128 specification | 128 px/deg (236.901 m/px), NASA PDS LRO LOLA GDR | `data/PROVENANCE.md` §3 |
| 1715 sunspot number | 45.0 (SILSO v2.0 yearly; sparse early observations, pre-1749 caveat) | `RESULTS.md` §8; `data/PROVENANCE.md` §5; `outputs/corrected_series.csv` |
| Morrison & Appleby 1981 datum errors | Up to 0.4″ at some position angles; 66,000 occultations | `RESULTS.md` §3, §7 item 8; `NOVELTY_AUDIT.md` §(d) |
| Sigismondi 2008 edge losses (context) | −0.02…−0.17″ | `RESULTS.md` §5 (filter/detector edge losses quantified by Sigismondi 2008) |
| Archive authors' assessed real errors | ±0.2″ (video era), ±0.4″ (visual era); formal σ ~4× too small | `data/PROVENANCE.md` §1; `RESULTS.md` §8 |
| Software environment | Python 3.12, numpy, scipy 1.18.1, skyfield 1.55, jplephem | `data/PROVENANCE.md` §6 |
| SILSO licence/credit/DOI | CC BY-NC 4.0; "Source: WDC-SILSO, Royal Observatory of Belgium, Brussels"; doi:10.24414/qnza-ac80 | `data/PROVENANCE.md` §5 |

## 4. Dunham Figure 1 extraction table (Appendix Table A1)

All 27 rows of Table A1 are copied, value for value, from `data/dunham2016_table.csv` (year/month/day, type, n_obs, method, deltaR_arcsec, sigma_arcsec), whose provenance — Figure 1, p. 352 of Dunham et al. (2016), rendered at 300 dpi, transcribed by eye, re-verified digit-for-digit in a second pass — is documented in `data/PROVENANCE.md` §1. This satisfies the sweep requirement (SWEEP.md, P3b) that the extraction be tabled in the paper, since the publisher-PDF values are image-only.

## 5. NOVELTY CLAIMS — SWEEP-ADOPTED (superseding "NOVELTY CLAIMS — PENDING SWEEP")

The precedent sweep (`~/workspace/papers/precedent-sweep/SWEEP.md`, run 2026-11-17, P3 section) is binding and has been adopted in the paper (§1.4, §3.5). The earlier "pending sweep" status no longer applies.

### P3a — HOLDS (SWEEP-ADOPTED, scoped)
- **Surviving wording used in the paper:** First re-reduction of the historical Baily's-beads eclipse archive (the Fiala 1715–1991 / Dunham et al. 2016 set) using LOLA lunar topography profiles.
- **Scope condition:** LOLA use on single modern eclipses is prior art and is cited, not claimed — Wang & Barriot (2021, *RAA* 21:11; 2012 eclipse light curve from LRO LOLA DEM), Quaglia et al. (2021, *ApJS* 256:36; 2017 eclipse, LOLA SLDEM/LDEM), IOTA/ES 2019 analysis via Occult (LRO LOLA + Kaguya) — all per SWEEP.md P3a. Kaguya single-eclipse work (Adassuriya et al. 2011; Lamy et al. 2015) is likewise cited as prior art from `NOVELTY_AUDIT.md` §(b).
- **Closest prior recorded by the sweep:** Dunham et al. (2016) itself — it covers the archive and states the Watts basis, listing the modern re-analysis only as future work (§4).
- **Earlier audit position (for the record):** `NOVELTY_AUDIT.md` verdict "seam narrowed but still open" and its "surviving novelty claim" paragraph are consistent with, and now superseded in wording by, the sweep's P3a verdict.

### P3b — NARROWED (SWEEP-ADOPTED, rescoped)
- **Surviving wording used in the paper:** The first systematic (published) comparison of Fiala et al. (1994) against Dunham et al. (2016) over their nine overlapping eclipses (disagreement on 7 of 9), and the identification of Dunham et al.'s 1715 value as a probable sign error.
- **What was removed:** Any presentation of the 1715 anomaly itself as newly noticed. **Binding citation added:** Morrison, L. V., Stephenson, F. R. & Parkinson, J. (1988). Diameter of the Sun in AD 1715. *Nature* 331, 421–423. doi:10.1038/331421a0 — their re-discussion concluded little/no secular change since 1715, incompatible with a large positive 1715 excess. Toulmonde (1997), noted in the sweep as likewise finding no secular variation, is also cited in the paper.
- **Sweep requirement adopted:** The Dunham Fig. 1 extraction is tabled in the paper (Appendix Table A1; §4 above), because those values are image-only in the publisher PDF and the 7-of-9 count rests on this lab's extraction.

### Claims explicitly NOT made (from NOVELTY_AUDIT.md, retained)
- Not the first modern-limb eclipse radius (single-eclipse modern-limb work exists since 2011).
- Not "the field still reduces with Watts" (practice migrated: Kaguya in Occult ~2010; LOLA-only since Feb 2021, Occult 4.12.2/4.12.3).
- Not the first to question/doubt the archive in print (Hayakawa et al. 2026 excluded the 2016 table in a refereed compilation).
- Not a new solar-radius measurement (Q2 is a test of the corrected archive against the pre-existing modern cluster).

## 6. Gaps and numbers NOT found in the sources

- **G1 — Raw bead timings / per-bead position angles / per-limit ΔR values:** not openly obtainable and not in the sources (`PREDICTION.md` §4.2; `RESULTS.md` §8; `data/PROVENANCE.md` §1). The paper states this explicitly (§4.2 items 1–2, 10) and presents no such numbers.
- **G2 — Public repository / DOI for this project:** none is given in the source files. The paper's Data & Code Availability section claims none.
- **G3 — Bibliographic details for several cited works** (e.g. Auwers 1891; Van Flandern 1970; Morrison 1979; Prša et al. 2016; Toulmonde 1997; Scott 1988; given names/initials for Wang & Barriot 2021 and for Young in Wright & Young 2024): not given in the sources. The References list omits those details rather than supplying them, and says so per entry.
- **G4 — South-window maximum, checked, no discrepancy:** an initial draft note suspected a mismatch here; recomputation settled it — `outputs/corrected_series.csv` w15 south maximum is +0.3531″ (1912-04-17), matching `RESULTS.md` §3's +0.136…+0.353″ range. (The +0.357″ figure that prompted the check is the ±30°-window column for a different event, not the primary window.) No internal inconsistency between RESULTS.md and the archived CSV was found in any headline number.
- **G5 — Dunham et al. (2016) page range:** `data/PROVENANCE.md` §1 gives pp. 351–353; SWEEP.md P3a gives pp. 351–354 and doi:10.1017/S1743921316000417. Both are recorded in the paper's References entry; the paper's text uses pp. 351–353 (provenance record) for the article and p. 352 for Figure 1.
- **G6 — 1715 σ in Fiala reproductions:** Sigismondi (2008) AIP 966 Table 1 prints 0.20; the companion reproduction prints 0.02, identified in the sources as a typo in one reproduction; 0.20 adopted (`data/PROVENANCE.md` §7; `outputs/crosscheck_sources.csv` note).
- **G7 — Hayakawa et al. (2026, ApJL) full text:** the novelty audit read the IOPscience abstract page and indexed full text; the publisher PDF timed out on fetch (`NOVELTY_AUDIT.md` header caveat; `data/PROVENANCE.md` §7). The paper keeps that caveat (§4.2 item 9).
- **G8 — No venue, submission, or peer-review status** is claimed anywhere; the status line is "Manuscript in preparation — not yet peer-reviewed." No university, employer, degree, or credential appears anywhere in the paper or this file.

## 7. Authorship block — as printed in the paper

Author: Atharva Chourey
Affiliation: Atharva Chourey Lab (independent research lab)

(This is the final, corrected form per the parent brief's Correction 2, superseding both the original personal-line instruction and the intervening lab-only line.)
