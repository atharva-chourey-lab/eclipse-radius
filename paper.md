# A re-reduction of historical eclipse observations: solar radius 959.494 ± 0.044″ and a probable sign error in the canonical archive

Author: Atharva Chourey
Affiliation: Atharva Chourey Lab (independent research lab)

*Manuscript in preparation — not yet peer-reviewed.*

## Abstract

Baily's-bead timings at eclipse path limits have been used to infer corrections, ΔR, to the standard solar radius, and the resulting series has been discussed as evidence of solar-diameter variation linked to the solar cycle. The compilation of Dunham, Sofia, Guhl & Herald (2016) was, by its authors' statement, analysed with lunar limb data from Watts (1963), and its authors called for a consistent re-analysis with modern profile data. We report a pre-registered differential re-reduction of that series: for each of its 27 events (1715–2006), the difference between a modern limb from Lunar Reconnaissance Orbiter LOLA LDEM_128 altimetry and the Watts limb was computed at the event's libration, averaged over registered polar bead windows, and subtracted from the published ΔR. The mean Watts→LOLA correction is +0.100″, but strongly asymmetric: +0.271″ (south) against −0.071″ (north). The corrected mean radius is 959.494 ± 0.044″ (median 959.481″), inconsistent under the registered ±0.06″ bands with Auwers' 959.63″, the modern eclipse cluster (~959.97″) and the IAU nominal 959.22″ alike. No significant sunspot correlation exists before (ρ = −0.19, p = 0.34) or after correction (ρ = −0.24, p = 0.22), and robust scatter shrinks 17.4%, short of the registered 25% collapse criterion: verdict PARTIAL / MIXED. A cross-check finds the 2016 table disagrees with Fiala, Dunham & Sofia (1994) on 7 of 9 overlaps, five sign flips; the 1715 entry (−0.50″ against +0.48″, at identical n and σ) is a probable sign error, and on the 2016 values the classical 1715–1979 shrinkage comparison inverts.

**Keywords:** solar radius — eclipses — Baily's beads — lunar limb — Watts profiles — LOLA — historical observations — data audit

---

## 1. Introduction

### 1.1 The solar-radius and shrinkage question

Whether the Sun's radius is constant, and if not, how it changes, has repeatedly been addressed with eclipse observations. At an eclipse, the times at which sunlight appears or disappears through valleys in the lunar limb — Baily's beads, observed near the northern and southern limits of the path — constrain the Sun's angular radius relative to the lunar limb's position and profile. If that profile is known, bead timings convert into a correction, ΔR, to an adopted standard radius, and a series of such corrections can be examined for secular change, fluctuations, and any association with solar activity.

The vulnerability is structural: an eclipse radius is measured against the Moon. Every error in the adopted limb profile at the bead position angles propagates directly, with reversed sign, into the inferred solar radius. If the datum is systematically wrong in the polar regions — where path-limit beads occur — part of what has been read as solar variation may instead be lunar-profile error, frozen into the archive at reduction and carried forward whenever the published values are reused.

Two distinct claims are entangled here. The first is long-baseline shrinkage: Dunham et al. (1980, *Science* 210:1243, as cited) reported a "0.4″ shrinkage" between 1715 and 1979. That 1715 result was already disputed in print: Morrison, Stephenson & Parkinson (1988, *Nature* 331:421–423) concluded little or no secular change since 1715, incompatible with a large positive 1715 excess. Nothing here claims the 1715 anomaly as newly noticed; the lab's narrower contribution is stated in §1.4 and §3.5. The second claim is shorter-baseline variability: Dunham et al. (2016) present ΔR fluctuations of 0.1–0.3″ as a solar-variability proxy, linked to the cycle through the Sofia–Li W-parameter argument, as described in the sources. This paper tests the archive underlying the second claim, and reports what follows — and does not follow — for the first.

Space-based measurements, as cited in the sources, constrain any true cycle-synchronous radius variation far below the eclipse series' fluctuations: less than 23 milliarcseconds peak-to-peak (Bush, Emilio & Kuhn 2010) and less than 7 milliarcseconds after correction (Kuhn et al. 2004), against residual eclipse scatter of order 0.20″. That tension does not by itself dispose of the eclipse record — bead timings sense an extinction edge, the space results an inflection-point radius — but eclipse fluctuations cannot be promoted to physical variation without confronting the cap, and this paper makes no such promotion.

### 1.2 The historical eclipse archive

The archive under audit is Figure 1 of Dunham, Sofia, Guhl & Herald (2016), "Solar diameter measurements from eclipses as a solar variability proxy", *Proceedings of IAU Symposium 320*, pp. 351–353 (per the provenance record): 27 events, 1715-05-03 to 2006-03-29, each with type, number of observations, method, ΔR relative to 959.63″ at 1 au, and formal error. The ≥1970 subset has 20 events, matching the paper's "20 annular and total solar eclipses". The earlier events (1715, 1878, 1900, 1912, 1922, 1925, 1966) are historical extensions carrying particular weight in any long-baseline argument.

The archive's foundational earlier table is Fiala, Dunham & Sofia (1994), *Solar Physics* 152:97–104 (as cited in the sources); the 1994–2016 relationship matters a great deal, and §3.4–§3.5 are devoted to it.

Three reference values frame the interpretation of any mean radius derived from this archive, and each is used here only as stated in the source materials.

First, the Auwers standard: 959.63″ at 1 au (Auwers 1891) — the archive's own zero-point, and, per the sources, still the almanac prediction standard: Quaglia et al. (2021), as quoted in the audit, state it "is used in all published eclipse predictions — for example, in The Astronomical Almanac", and Wright & Young (2024, §6.4) call it the de facto standard "first published more than a century ago". A first prominent break: Irwin's map for 8 April 2024 used 959.95″.

Second, the IAU nominal radius: 959.22″, identified in the source materials as the IAU 2015 nominal value, helioseismic in basis (Prša et al. 2016, as cited), and described in Rozelot & Kosovichev (2026, §2.5, as cited) as the seismic radius, the field's current best determination.

Third, a modern eclipse cluster: single-eclipse determinations with modern limb data, placed by the sources in the range 959.92–960.02″ — Lamy et al. (2015), 959.99 ± 0.06″; Quaglia et al. (2021), 959.95 ± 0.05″; Guhl (2023), 960.01 ± 0.12″ — giving the cluster centre 959.97″ used in the registered comparison. None is a re-reduction of this archive.

Two Watts-era results mark the spread the archive-era literature itself produced: Kubo (1993, as cited) pooled eclipses of 1970–1991 for radii of 959.74–959.88″; Kilcik et al. (2009) derived 959.22 ± 0.04″ for 29 March 2006 — 0.7″ below the modern cluster, on the audit's characterisation — with a 19-eclipse claim of nonhomologous changes. That 2006 value is confronted in §3.3.

### 1.3 Prior reductions and the Watts datum

The 2016 compilation states (p. 352, per the provenance file) that its table was "analyzed with lunar limb data from 'The Marginal Zone of the Moon' Watts (1963)" — a photographic survey from before spacecraft altimetry. That its datum carries systematic errors is not new: the sources record it as slightly elliptical and offset from the Moon's centre of mass (Van Flandern 1970; Morrison 1979, as cited), and Morrison & Appleby (1981) derived corrections from 66,000 occultations, finding profile errors attaining 0.4″ at some position angles, varying with libration. The VI/122 documentation itself warns that the polar Cassini regions are poorly covered and the northern limb reads too low in a specified range — the polar zones sampled by path-limit beads are the datum's documented weak side.

Meanwhile, reduction practice for new work moved on: Herald reduced Kaguya altimetry into Watts-format profiles in 2009; Occult 4 distributed Kaguya profiles by ~2010–2011; Occult 4.12.2 (14 February 2021) disabled the Kaguya download as "fully superseded by the LOLA dataset", and 4.12.3 removed Kaguya support entirely; current IOTA guidance selects LOLA. The field does not still reduce new eclipses against Watts, and any such statement would be false. What did not migrate is the published archive itself — the 2016 table as printed remained Watts-reduced, and the printed prediction radius separately remained Auwers' (§1.2).

### 1.4 The stated future work, and the status of the novelty question

In §4 of Dunham et al. (2016), the archive's authors stated the remedy themselves, in words quoted in the novelty audit: "The results can be improved with a consistent reanalysis of the observations using the much more accurate lunar profile data that are now available from the Japanese Kaguya and NASA's LRO lunar orbiter observations." The same intention appears in the programme's 2014 and 2015 presentations, and Sôma (2012, as cited) announced a similar intent. The project's novelty audit (2026-11-17; sources searched are listed in that document) found no publication through November 2026 that re-processes the historical bead ΔR series, or a substantial subset of it, with LOLA or Kaguya limbs, or that publishes Watts-to-modern corrections to Dunham et al. (2016)'s ΔR values.

The qualifications, as the audit states them: modern-limb single-eclipse radii have existed since 2011; reduction practice migrated (§1.3); Hayakawa et al. (2026) already excluded the 2016 table from a compilation figure in print; and individual historical events have been re-derived with modern topography — most relevantly 1715, at 959.98 ± 0.23″ (Hayakawa et al. 2026) — narrowing the historical flank without touching the bead series as a series.

> **Novelty — sweep-adopted wording.** The precedent sweep (2026-11-17; `~/workspace/papers/precedent-sweep/SWEEP.md`) adjudicated this paper's two claims, and the manuscript follows its verdicts. **(P3a — HOLDS, scoped):** first re-reduction of the *historical* Baily's-beads archive (Fiala 1715–1991 / Dunham et al. 2016 set) using LOLA profiles. LOLA on single modern eclipses is prior art, cited not claimed: Wang & Barriot (2021; 2012 eclipse, LRO LOLA DEM), Quaglia et al. (2021; 2017 eclipse, LOLA SLDEM/LDEM), IOTA/ES 2019 via Occult (LOLA + Kaguya), plus the Kaguya work in §1.2–§1.3. **(P3b — NARROWED):** the 1715 anomaly was already disputed by Morrison, Stephenson & Parkinson (1988, *Nature* 331:421–423) — little or no secular change since 1715 — with Toulmonde (1997) likewise finding no secular variation, as the sweep notes. The 1715 anomaly is therefore **not** presented as newly noticed; the surviving novelty for §3.4–§3.5 is only the first systematic Fiala-1994-vs-Dunham-2016 comparison and the sign-error diagnosis.

The contribution, in deliberately narrow form: a uniform Watts-to-modern-limb differential correction to the full published ΔR series, under rules registered before the data were touched, testing **Q1** (does the claimed cycle-linked variation survive removal of the Watts datum?) and **Q2** (where does the corrected mean sit, against Auwers, the modern cluster, and the IAU nominal?). A third finding — the 2016/1994 table disagreement — was not registered; it arose from the cross-check after Hayakawa et al. (2026) flagged the table, and is labelled as such throughout. This work executes the archive authors' own stated future-work programme at the level the open data permit: an audit of a method era, not of the named observers.


---

## 2. Methods

### 2.1 Pre-registration and design overview

The audit was pre-registered in `PREDICTION.md`, git-committed (commit `a42d76a`, per `RESULTS.md`) on 2026-11-17 before any archive data were touched, fixing the audit object, correction formula, bead windows, cycle proxy and decision rules. Deviations forced by the data are labelled in `RESULTS.md` §2 and reported in §2.4; the pre-registration was not edited after data acquisition began.

The design is differential, not a re-reduction from raw timings: raw bead timings are not openly obtainable (held in the IOTA / Occult archives; `data/PROVENANCE.md` §1), a limit anticipated in the pre-registration (§4.2). For each event we compute how much the inferred radius changes when the limb model is swapped at fixed timings, and apply that to the published ΔR. The correction changes only the limb model, not the original reductions' solar-edge definition: the registered definition is the inflection point of the limb-darkening function; bead timings sense an extinction edge; the differential design is definition-preserving (`PREDICTION.md` §2a).

### 2.2 Archive and observation selection

The audit object is the 27-event table in Figure 1 (p. 352) of Dunham et al. (2016), transcribed by eye from the figure rendered at 300 dpi into `data/dunham2016_table.csv`, with type, number of observations, method, ΔR (arcsec, relative to 959.63″ at 1 au) and formal σ for each event. Because those values are image-only in the publisher PDF, the extraction itself is part of this paper's contribution, and the full extracted table is reproduced as Table A1 in the Appendix so that every downstream number can be checked against it. The events run from 1715-05-03 to 2006-03-29; the IOTA-era (≥1970) subset has 20 events.

After Hayakawa et al. (2026)'s exclusion of this table (§2.6) was flagged, every value was re-read against the rendered Figure 1 digit-for-digit in a second pass (`data/PROVENANCE.md` §1). The transcription is exact as published, so the disagreements with Fiala et al. (1994) in §3.4 are genuine differences between publications, not digitisation errors in this lab's extraction.

No event was excluded or imputed: all 27 events were correctable under the registered rules (`RESULTS.md` §1).

Event geometry — the greatest-eclipse instant and the geocentric optical libration (l, b) at that instant — was computed from the JPL DE440 ephemeris (`data/de440.bsp`) with the IAU 2009 mean lunar rotation elements, in `scripts/event_geometry.py`, output in `outputs/event_geometry.csv`. Validation: for 2006-03-29 the computed greatest eclipse is 10:11:18 UTC, against Espenak's published 10:11:17.6 UT — reproduced to 0.4 s (`RESULTS.md` §1; `data/PROVENANCE.md` §4, which also records the libration cross-check against the bulletin value).

### 2.3 The Watts→LOLA correction

For event *e* with published ΔR_pub:

$$\Delta R_{\rm corr}(e) = \Delta R_{\rm pub}(e) - \bar\delta(e), \qquad \delta(\theta, \mathrm{lib}) = h_{\rm LOLA}(\theta, \mathrm{lib}) - h_{\rm Watts}(\theta, \mathrm{lib})$$

where δ̄(e) is the mean of δ over the event's bead position-angle window at the event's libration. The sign follows from the tangent-point argument registered in advance: a bead event fixes the centre distance; replacing h_Watts by a higher h_new lowers the inferred radius by δ, so a modern limb that sits above Watts means the Watts-based reduction overstated ΔR (`PREDICTION.md` §2d).

*Bead window.* Per-bead position angles are not published with the ΔR table, so the registered approximation is a polar window: the mean of δ within ±15° of the lunar north point and within ±15° of the south point, merged, is the primary statistic; half-widths ±7.5° and ±30° are registered sensitivities reported for every headline number. The geometry is supported by the archive's own practice: Dunham's reduction used bead events within 30° of the poles (IAU GA 2015 talk, as cited in `RESULTS.md` §2d), and the 2016 paper's Figure 2 analysis likewise used beads within 30 degrees of the lunar north and south poles (`data/PROVENANCE.md` §1).

*Watts profiles.* VizieR catalogue VI/122 (digitised by HMNAO, grid format by USNO), archived as `data/watts.dat.gz` and parsed by `scripts/parse_watts.py`. The grid spans 91 longitude librations, 81 latitude librations and 1,800 Watts angles at 0.2° steps (`data/PROVENANCE.md` §2). Sampling is bilinear in (L, B), then periodic linear interpolation in Watts angle, with the documented conversion WA = AA + 0.21° − 0.022·cos(elongation from ascending node), the offset being Scott (1988)'s value (`doc.txt` §6b).

*Modern profiles.* LOLA LDEM_128 (NASA PDS, LRO LOLA GDR), a global radius grid at 128 px/deg, archived as `data/LDEM_128.IMG`. `scripts/extract_lola_profiles.py` builds silhouette profiles — maximum projected radius per 0.2° axis-angle bin, ±14° band about the limb plane — at each event's libration, as angular height above the 1737.4 km sphere at mean distance 384,398.55 km (`data/PROVENANCE.md` §3).

*Watts frame convention.* The mapping of the Watts grid's (L, B, WA) arguments onto the modern (l, b, axis angle) frame was determined empirically in `scripts/validate_frames.py` by cross-correlating Watts and LOLA profiles for three events over all sign/shift combinations. The winning convention — L entered at +l, **B entered at −b**, WA = AA + 0.21° — gives Pearson r = 0.87–0.89; reversed-axis mappings give r < 0 and wrong-L mappings r ≤ 0.80 (`RESULTS.md` §2c). The B-sign choice is the weakest link in the pipeline and is carried as a declared systematic (§4.2): entering B at +b instead shifts δ̄ by 0.061″ on average (maximum 0.148″).

*Datum referencing.* The classical eclipse constant k = 0.2725076, with Earth radius 6378.137 km at mean distance 384,398.55 km, gives a mean-limb radius of 1738.091 km; LDEM is referenced to a 1737.4 km sphere. Differencing across those datums unaligned would inject a spurious +0.371″ into every δ̄, so a constant datum term (REFERENCE_TERM = 0.3707″) is applied first (`RESULTS.md` §2b). Being constant, it affects only Q2's location; Q1 is invariant to it. External validation: for 1715, Fiala et al.'s +0.48 and Hayakawa et al.'s re-derivation (ΔR = +0.35) imply a correction of +0.13″; this pipeline gives +0.166″, within 0.04″ — without the datum term it would have reported +0.54″.

### 2.4 Deviations from the registered plan

Two deviations were forced by the data and are declared here, following `RESULTS.md` §2.

**(a) Modern limb: Kaguya → LOLA.** The pre-registration named Herald's Kaguya Watts-format profiles (Occult 4) as comparator. That distribution no longer exists: Occult 4.12.2 (14 February 2021) disabled the Kaguya download as "fully superseded by the LOLA dataset", and 4.12.3 removed support entirely. The audit therefore uses LOLA LDEM_128 — the successor the ecosystem adopted. The registered SLDEM2015 spot-checks were not run: SLDEM2015 covers only ±60° latitude and cannot see the polar windows.

**(b) Raw bead timings unavailable.** As §2.1 states, the audit proceeds at the published-ΔR level, as the registered design assumed.

### 2.5 Cycle proxy, metrics and decision rules

The cycle proxy is the SILSO v2.0 annual mean sunspot number for each event's year (`data/PROVENANCE.md` §5). No lag in the primary test; a ±1-year lag check is a registered secondary diagnostic.

Primary metrics, computed identically on the published and corrected series (n = 27): (i) robust scatter = 1.4826 × MAD of ΔR; (ii) Spearman ρ between ΔR and annual sunspot number, with its p-value; (iii) for reference, Pearson r and the OLS slope of ΔR on sunspot number. The published σ values are not used by the registered metrics; the tests are unweighted (`RESULTS.md` §8).

Registered Q1 rules (`PREDICTION.md` §3): **SURVIVES** requires a significant corrected correlation (p < 0.05) with |ρ| ≥ 0.45 and robust scatter ≥ 0.08″. **COLLAPSES** requires non-significance (p ≥ 0.05) and a robust-scatter shrink of ≥ 25% relative to the published series. Anything else is **PARTIAL / MIXED**, reported as such with both metrics printed.

Registered Q2 rule: R̄ = 959.63″ + mean(ΔR_corr), SE = SD/√n, median reported alongside. R̄ is **consistent with Auwers** if |R̄ − 959.63| ≤ 0.06″, **with the modern cluster** if |R̄ − 959.97| ≤ 0.06″, **with the IAU nominal** if |R̄ − 959.22| ≤ 0.06″; otherwise **inconsistent with all three**, and R̄ ± SE is the archive's own number. Systematics are not folded into the band test (`RESULTS.md` §5). If mean and median land in different bands, both are reported.

### 2.6 The transcription cross-check (post-registration)

The cross-check of §3.4 was not registered. It was undertaken after Hayakawa et al. (2026, *ApJL*) excluded Dunham et al. (2016)'s data from their compilation figure "as they have considerable data offsets with their probable source articles" (`RESULTS.md` §6). The 2016 table was compared against Fiala et al. (1994) as reproduced in Sigismondi (2008, AIP Conf. Proc. 966, Table 1), cross-verified against the companion reproduction, and against per-eclipse sources where they exist (log: `outputs/crosscheck_sources.csv`; provenance: `data/PROVENANCE.md` §7). A labelled post-registration sensitivity — Fiala values substituted for the nine overlaps, same limb corrections — is reported in §3.4. The primary correction uses Dunham et al. (2016) for all 27 events; no primary value comes from elsewhere.

---

## 3. Results

### 3.1 The correction: small, positive, and lopsided

Averaged over the registered ±15° polar bead windows, the modern limb sits **δ̄ = +0.100″** above the Watts limb, with a per-event range of −0.003″ to +0.194″ (`RESULTS.md`, headline results and §3; `outputs/corrected_series.csv`; the lab recomputed the mean, minima and maxima from that file and they agree: mean +0.0996″, range −0.003″ to +0.194″). Watts-based reductions therefore overstated ΔR by about 0.1″ on average.

The correction is strongly hemispheric. The south-window mean is **+0.271″** — every event positive, range +0.136″ to +0.353″ — while the north-window mean is **−0.071″**, range −0.179″ to +0.072″. The south-minus-north asymmetry is +0.34″ (`RESULTS.md` §3). A single merged ΔR per event conceals this structure, and Dunham et al.'s 2-parameter fits — whose second parameter is a lunar-centre offset, partially degenerate with a north–south limb asymmetry — dilute it as well (`RESULTS.md` §3). We report the split because any future bead-level re-reduction should expect it.

This matches what was already known: Morrison & Appleby (1981) documented Watts datum errors attaining 0.4″ at some position angles, varying with libration, from 66,000 occultations; the VI/122 documentation independently flags the polar Cassini regions as the charts' weak zone (`RESULTS.md` §3). The correction's plausibility is not new — only its application to this series is (§1.4).

Selected per-event values (full table: `outputs/corrected_series.csv`): 1715, ΔR_pub −0.50″, δ̄ +0.166″, ΔR_corr −0.666″; 1979-02-26, −0.05″, +0.194″ (largest correction), −0.244″; 2002-12-04, −0.22″, −0.003″ (only negative correction), −0.217″; 2006-03-29, +0.09″, +0.104″, −0.014″.

### 3.2 Q1 — cycle-linked variation: PARTIAL / MIXED

Registered metrics, computed identically on both series (n = 27; `RESULTS.md` §4; `outputs/q1_q2_results.json`):

| Series | Robust scatter (″) | Spearman ρ vs SSN | p | Pearson r | OLS slope (″/SSN) |
|---|---|---|---|---|---|
| Published | 0.237 | −0.193 | 0.336 | −0.217 | −0.00072 |
| Corrected (±7.5°) | 0.205 | −0.273 | 0.169 | −0.202 | −0.00070 |
| Corrected (±15°) | 0.196 | −0.245 | 0.218 | −0.198 | −0.00067 |
| Corrected (±30°) | 0.194 | −0.226 | 0.257 | −0.218 | −0.00074 |

Registered secondary diagnostics at ±1-year lag (corrected, ±15°): lag −1, ρ = −0.005 (p = 0.98); lag +1, ρ = −0.299 (p = 0.13).

Applying the registered rules: SURVIVES requires a significant corrected correlation with |ρ| ≥ 0.45 — the correlation is not significant at any window (p ≥ 0.17), so it does not survive. COLLAPSES requires non-significance *and* a scatter shrink ≥ 25% — the shrink is 17.4% at the primary window (13–18% across windows), so it does not collapse either. **Verdict: PARTIAL / MIXED, at every window width.**

Stated plainly: in the published table there is no significant sunspot correlation for the correction to kill — Dunham et al.'s variability claim rests, on the sources' account, on the 0.1–0.3″ fluctuation level and the Sofia–Li W-parameter argument, not on a raw sunspot correlation. In the IOTA-era subset (1970+, n = 20, labelled post-registration diagnostic), scatter shrinks 32% (0.208″ → 0.141″) — about a third of that subset's scatter was the Watts datum — but the correlation remains non-significant (ρ = −0.13 → −0.26; p = 0.57, 0.27).

The residual scatter (~0.20″) remains an order of magnitude above the space-based cap (< 23 mas peak-to-peak, Bush, Emilio & Kuhn 2010; < 7 mas, Kuhn et al. 2004). As `RESULTS.md` §4 states: (i) the residual fluctuations cannot be promoted to physical variation without confronting that cap; (ii) the comparison is not apples-to-apples in edge definition (extinction edge against inflection-point radius), so the cap constrains but does not by itself falsify an extinction-edge record. The Watts datum is responsible for a real, quantified slice of the archive's scatter and level — and not for the rest.

### 3.3 Q2 — the corrected mean radius: 959.494 ± 0.044″, inconsistent with all three

R̄ = 959.63 + mean(ΔR_corr) = **959.494″**, standard error **0.044″**; the median-based value is **959.481″** (`outputs/q1_q2_results.json`: R_mean 959.4941, R_se 0.0443, R_median 959.4809). Mean and median fall in the same registered category, so the registered mean/median clause is not triggered. The result is stable across the registered window sensitivity: 959.488″ / 959.494″ / 959.508″ for ±7.5° / ±15° / ±30°.

| Comparator | Value (″) | Basis, as stated in the sources | R̄ − value (″) | In ±0.06″ band? |
|---|---|---|---|---|
| Auwers 1891 standard | 959.63 | Eclipse-prediction standard (still the almanac value; Quaglia et al. 2021; Wright & Young 2024 §6.4) | −0.136 | No |
| Modern eclipse cluster | 959.97 (centre) | Lamy et al. 2015: 959.99 ± 0.06; Quaglia et al. 2021: 959.95 ± 0.05; Guhl 2023: 960.01 ± 0.12 | −0.476 | No |
| IAU 2015 nominal | 959.22 | Helioseismic (Prša et al. 2016); the seismic radius is the field's current best determination per Rozelot & Kosovichev 2026 §2.5 | +0.274 | No |
| Kubo et al. (context) | 959.74–959.88 | Watts-era pooled eclipses 1970–1991 | −0.25 to −0.39 | — |
| Kilcik et al. 2009 (context) | 959.22 ± 0.04 | 2006 eclipse, Watts/occultation-refined limb era | +0.27 | — |

**Registered verdict: inconsistent with all three.** The corrected archive's own number is 959.494 ± 0.044″ (statistical standard error; declared systematics in §4.2 are of comparable size and are not folded into the band test, per the registered rule).

Removing the Watts datum moves the archive *down*, away from the modern cluster — the published mean already sat at Auwers and the net correction is positive — so the datum is not the reason the archive's mean disagrees with the cluster (`RESULTS.md` §5). This is a test of the corrected archive, not a new radius measurement: the cluster (959.92–960.02″) was already established (§1.2, §1.4), and the corrected archive sits ~0.48″ below it and ~0.14″ below Auwers. §4.1 discusses the two readings the sources offer for that gap.

*The archive-era outlier.* Kilcik et al. (2009)'s 2006 value (ΔR = −0.41) compares with the corrected archive's ΔR_corr = −0.014″ (R = 959.616″) for that eclipse, 0.40″ higher; the corrected mean sits 0.27″ above their value. The corrected series does not support that outlier or its 19-eclipse "nonhomologous" claim (`RESULTS.md` §5).

### 3.4 The transcription cross-check: Dunham (2016) versus Fiala (1994)

Hayakawa et al. (2026) excluded Dunham et al. (2016)'s data from their compilation figure "as they have considerable data offsets with their probable source articles". Following the steer described in §2.6, we itemise that discrepancy here. The lab's digitisation was first re-verified digit-for-digit against the rendered Figure 1 (§2.2): the transcription is exact as published, so every disagreement below is a genuine difference between publications.

Nine events overlap between Fiala et al. (1994) and Dunham et al. (2016). The two tables disagree on **7 of 9** — five of them sign flips (`RESULTS.md` §6; `outputs/crosscheck_sources.csv`):

| Date | Fiala 1994 ΔR (″) | Dunham 2016 ΔR (″) | Difference (″) |
|---|---|---|---|
| 1715-05-03 | +0.48 ± 0.20 (3 obs) | −0.50 ± 0.20 (3 obs) | −0.98, sign flip |
| 1925-01-24 | +0.51 ± 0.08 (8 obs) | −0.21 ± 0.17 (11 obs) | −0.72, sign flip |
| 1976-10-23 | +0.04 ± 0.07 | −0.38 ± 0.09 | −0.42, sign flip |
| 1987-09-23 | −0.11 ± 0.03 | +0.10 ± 0.05 | +0.21, sign flip |
| 1981-02-04 | −0.02 ± 0.03 | −0.21 ± 0.05 | −0.19 |
| 1983-06-11 | +0.09 ± 0.02 | −0.10 ± 0.08 | −0.19, sign flip |
| 1980-02-16 | −0.03 ± 0.03 | −0.18 ± 0.05 | −0.15 |
| 1979-02-26 | −0.11 ± 0.05 (47 obs) | −0.05 ± 0.08 (21 obs) | +0.06 |
| 1984-05-30 | +0.09 ± 0.04 | +0.13 ± 0.07 | +0.04 |

Dunham et al. (2016) is a re-reduction (WinOccult/Solrad 2-parameter solutions, beads within 30° of the poles), not a reprint, and different bead subsets explain differing observation counts (1979: 47 in Fiala et al. against 21). They do not comfortably explain five sign flips, two (1715, 1925) on the programme's most cited anchors, at unchanged n and σ for 1715 (`RESULTS.md` §6). Hayakawa et al.'s compiled values side with Fiala et al.: 1925 as 960.14 ± 0.08″, 1715 as ≥ 959.91″.

Per-eclipse sources for post-1991 events (`RESULTS.md` §6): 1994-05-10, Thompson/IOTA −0.27 ± 0.02 against Dunham et al. −0.25 (agreement); 1999-08-11, Thompson/IOTA +0.06 ± 0.06 against −0.03; 2005-10-03, Sigismondi 0.00 ± 0.17 (southern limit) against −0.06; 2006-03-29, Kilcik et al. −0.41 (§3.3) and Sigismondi ≈ 0.00 to −0.01 ± 0.17 against Dunham et al. +0.09. Cross-check sources exist for 13 events in total (9 Fiala et al.; 1994/1999 Thompson/IOTA; 2005 Sigismondi; 2006 Kilcik et al. and Sigismondi) and none replaces a primary value.

*Sensitivity to the input table (labelled, post-registration).* Substituting Fiala et al.'s nine values, same limb corrections: published scatter 0.163″, ρ = −0.285 (p = 0.150); corrected scatter 0.175″, ρ = −0.277 (p = 0.163) — **Q1 verdict unchanged**. Q2 moves to R̄ = **959.581″** (median 959.565″): consistent with Auwers by the mean band (|Δ| = 0.049 ≤ 0.06), the median 0.005″ outside its band, reported as-is. Which published table one audits changes Q2 at the ~0.09″ level; the limb correction (δ̄ ≈ +0.10″) does not, and is smaller than the tables' mutual disagreement (up to 0.98″).

### 3.5 The 1715 case

The eclipse of 3 May 1715 is the archive's most famous historical anchor, and it can now be stated three ways (`RESULTS.md` §6):

- **Fiala et al. (1994):** ΔR = +0.48 → through this pipeline, **959.944″**.
- **Hayakawa et al. (2026), modern-topography re-derivation:** **959.98 ± 0.23″** — agreement with the Fiala-based value within 0.04″.
- **Dunham et al. (2016):** ΔR = −0.50 → through this pipeline, **958.964″** — irreconcilable with the modern re-derivation by about 1″. No limb correction of the size documented anywhere (≤ 0.4″, Morrison & Appleby 1981) can bridge it.

Two framing points bind the presentation. First, the 1715 anomaly is not new: Morrison, Stephenson & Parkinson (1988) already disputed it in print (§1.1, §1.4). Second, what is new, per the sweep, is the systematic comparison and its diagnosis: the 2016 value has identical n = 3 and σ = 0.20 to Fiala et al.'s and differs from it almost exactly by sign (−0.50 against +0.48). The 1715 point in Dunham et al. (2016) should be treated as an error in that table — **most plausibly a sign error** — until the custodians say otherwise (`RESULTS.md` §6).

The consequence is direct: the 1715-versus-1979 "0.4″ shrinkage" (Dunham et al. 1980) is not supported by the 2016 table's own 1715 value. On Fiala et al.'s values the pair reads +0.48 against −0.11 — 0.59″ in the claimed direction; on Dunham et al. (2016)'s values, −0.50 against −0.05 — **the shrinkage inverts**. This audit takes no position on the 1980 claim itself, which used the era's own reductions; the 2016 table cannot be used to support it.

---

## 4. Discussion

### 4.1 What survives of the shrinkage claim

Three conclusions survive this audit, and three do not.

What survives, first, is a quantified datum effect: a mean level shift of ~+0.10″ in ΔR, about a sixth of the full series' robust scatter, and about a third of the IOTA-era subset's. The error is structured, not white — concentrated in the southern polar window (+0.271″ against −0.071″ north), at the scale Morrison & Appleby (1981) documented for the datum in general. Any future use of Watts-reduced bead values inherits that structure unless it is removed.

Second, a corrected archive exists where none did: 27 events, uniformly corrected, stable across window sensitivity, mean 959.494 ± 0.044″ — a property of the corrected archive, not a new measurement of the Sun. Third, the cross-check stands independently: the two tables disagree on 7 of 9 with five sign flips, and the choice between them moves Q2 by ~0.09″, comparable to the entire limb correction. Reconciling them is now a precondition for any further use of either.

What does not survive is, first, any support from this archive, as published in 2016, for the classical shrinkage comparison: on the 2016 table's own 1715 value the 1715–1979 comparison inverts (§3.5). We repeat the scope limit: this is a statement about the 2016 table, not a verdict on Dunham et al. (1980), which used the era's own reductions, and the 1715 anomaly itself was disputed in print by Morrison, Stephenson & Parkinson (1988) decades before this work.

Second, no cycle-linked variation is established by the corrected series — but none was established by the published series either, at the registered thresholds. The verdict is PARTIAL / MIXED: there was no significant raw sunspot signal in the table to begin with. Any cycle claim resting on this archive must rest on something else — the fluctuation level, or the W-parameter argument — and confront the < 23 mas space-based cap (Bush, Emilio & Kuhn 2010), subject to §3.2's edge-definition caveat.

Third, the corrected archive does not vindicate the archive's mean level: it moves away from the modern cluster. `RESULTS.md` §5 offers two readings the data do not separate: (i) further negative systematics beyond the limb datum — edge definitions; filter/detector losses of −0.02″ to −0.17″ (Sigismondi 2008, as cited); pre-GPS position/timing errors — none modelled here; or (ii) the archive's merged, polar-bead, 2-parameter reductions are not the same measurement as modern full-light-curve or flash-spectrum determinations. Either way, Watts is not the explanation for the gap.

A closing note that cuts both ways: the custodian community has itself de-emphasised bead-derived diameters — Dunham's IOTA pages (2023, updated 2025, as cited in `RESULTS.md` §7) state "we came to realize the difficulty in deriving such information from such recordings". This audit closes out a programme its owners have wound down; the corrected series and cross-check log may be the form in which this archive is most usefully preserved.

### 4.2 Limitations — stated explicitly

The following limitations are declared in `RESULTS.md` §8 and `PREDICTION.md`, and bound every claim above.

1. **Archive size and level of analysis.** n = 27, at the published-ΔR level, because raw bead timings are not openly obtainable. A bead-level re-reduction could distribute the §3.1 asymmetry differently (per-limit values are unpublished) and could supersede the window approximation.
2. **Window approximation.** Per-bead position angles are unpublished; polar windows (±15° primary) stand in for them. Dunham et al.'s bead selection (within 30° of the poles) supports the geometry and verdicts are stable across ±7.5° / ±15° / ±30°, but the approximation remains one.
3. **Selection.** The audit object is one published table, chosen in advance as the canonical archive; §3.4 shows Q2 depends on that choice at ~0.09″. Events outside it are out of scope except as cross-checks.
4. **Libration.** Geocentric (l, b) at greatest eclipse (DE440, IAU mean rotation elements), forced-libration terms ≤ ~0.03° neglected. The original reductions used per-observer topocentric librations; profile variation over the difference is second-order at window-mean level, as assessed in the sources.
5. **Watts B-sign systematic.** The empirical B-sign convention (§2.3) contributes ~0.06″ (mean |Δδ̄|; max 0.15″) — comparable to Q2's SE (0.044″), not folded into it.
6. **LDEM polar caveat (model dependence).** LDEM_128's highest-latitude cells are GMT `surface` interpolations where LOLA tracks are sparse; the polar windows inherit that smoothing. The DE421-ME/DE440 frame difference is at arcsec level, negligible at 0.2° sampling. Generally, the correction is a Watts→LOLA statement, not a Watts→truth statement.
7. **Not modelled (registered).** Pre-GPS timing/position errors; filter/detector extinction-edge losses; personal equation. The archive authors' own assessed real errors (±0.2″ video, ±0.4″ visual) exceed most corrections here — this is a datum audit, not a claim that corrected values are accurate to their formal σ (~4× too small, as the source paper assesses; the registered metrics do not use them).
8. **The 1715 sunspot number** (45.0) rests on sparse early observations (SILSO v2.0, pre-1749 caveat). It enters Q1 as registered; excluding 1715 changes no verdict — its leverage is on Q2 via ΔR (§3.4–§3.5), not via sunspot number.
9. **Cross-check source access.** The Fiala et al. (1994) values were read via Sigismondi (2008)'s two reproductions, cross-verified against each other (access route in `data/PROVENANCE.md` §7); one discrepancy between them (1715's σ: 0.20 against 0.02) was resolved to 0.20, matching Dunham et al. (2016)'s σ, and is logged in `outputs/crosscheck_sources.csv`. Hayakawa et al. (2026) *ApJL* details in the novelty audit come from the IOPscience abstract page and indexed full text; the publisher PDF timed out on fetch.
10. **Numbers not in the sources.** The sources give no per-bead timings, no per-limit published ΔR values, and no bead-level re-reduction; this paper presents no such numbers.

### 4.3 What a bead-level re-reduction would need

The obvious next step, identified in the sources and endorsed here, is a re-reduction from raw bead timings — per-bead position angles, per-limit solutions, LOLA profiles directly — which would retire the window approximation, distribute the asymmetry at bead level, and, if the custodians also reconcile the two tables, settle which published table the archive actually is. Until then, `outputs/corrected_series.csv` and `outputs/crosscheck_sources.csv` are the lab's deliverables.

---

## Data & Code Availability

All inputs, scripts and outputs are archived in `~/workspace/eclipse-radius/` (local archive at the time of writing; no public repository or DOI is claimed, and none is given in the source files).

- **Pre-registration:** `PREDICTION.md` (commit `a42d76a`). **Results:** `RESULTS.md`. **Novelty audit:** `NOVELTY_AUDIT.md`. **Sweep:** `~/workspace/papers/precedent-sweep/SWEEP.md`.
- **Data:** `data/dunham2016_table.csv` (Table A1), `data/watts.dat.gz` / `watts_grid.npz` (VizieR VI/122), `data/LDEM_128.IMG` / `lola_profiles.npz` (NASA PDS LDEM_128), `data/de440.bsp` (JPL DE440), `data/silso_yearly.csv` (WDC-SILSO v2.0; CC BY-NC 4.0; credit "Source: WDC-SILSO, Royal Observatory of Belgium, Brussels", doi:10.24414/qnza-ac80). Full provenance: `data/PROVENANCE.md`.
- **Scripts, in run order:** `scripts/parse_watts.py`, `event_geometry.py`, `extract_lola_profiles.py`, `validate_frames.py`, `correct_and_test.py`. Environment (`data/PROVENANCE.md` §6): Python 3.12, numpy, scipy 1.18.1, skyfield 1.55, jplephem.
- **Outputs:** `outputs/corrected_series.csv`, `outputs/q1_q2_results.json`, `outputs/crosscheck_sources.csv`, `outputs/event_geometry.csv`.

Every number in this paper is regenerated by re-running the scripts, in the order above, on the datasets as archived (`RESULTS.md` §9).

---

## Appendix — Table A1. The Dunham et al. (2016) Figure 1 extraction

The archive is image-only in the publisher PDF; this extraction (`data/dunham2016_table.csv`; Figure 1 at 300 dpi, transcribed by eye, re-verified digit-for-digit, §2.2) is the audit object and part of the contribution. ΔR and σ in arcseconds, relative to 959.63″ at 1 au.

| Date | Type | n_obs | Method | ΔR (″) | σ (″) |
|---|---|---|---|---|---|
| 1715-05-03 | Total | 3 | visual | −0.50 | 0.20 |
| 1878-07-29 | Total | 12 | visual | +0.55 | 0.15 |
| 1900-05-28 | Total | 8 | visual | +0.12 | 0.09 |
| 1912-04-17 | Hybrid | 26 | photoes | −0.29 | 0.22 |
| 1922-09-21 | Total | 4 | visual | +0.20 | 0.40 |
| 1925-01-24 | Total | 11 | visual | −0.21 | 0.17 |
| 1966-05-20 | Hybrid | 9 | photoes | +0.03 | 0.05 |
| 1970-03-07 | Total | 4 | visual & proj. | −0.05 | 0.12 |
| 1972-07-10 | Total | 14 | visual & proj. | −0.02 | 0.61 |
| 1973-06-30 | Total | 7 | visual & proj. | +0.40 | 0.20 |
| 1976-10-23 | Total | 14 | projection | −0.38 | 0.09 |
| 1979-02-26 | Total | 21 | visual & proj. | −0.05 | 0.08 |
| 1980-02-16 | Total | 36 | projection | −0.18 | 0.05 |
| 1981-02-04 | Annular | 52 | projection | −0.21 | 0.05 |
| 1983-06-11 | Total | 26 | video & proj. | −0.10 | 0.08 |
| 1984-05-30 | Hybrid | 27 | video | +0.13 | 0.07 |
| 1987-03-29 | Hybrid | 11 | photoes | −0.19 | 0.08 |
| 1987-09-23 | Annular | 44 | video | +0.10 | 0.05 |
| 1988-03-18 | Total | 20 | projection | −0.13 | 0.14 |
| 1991-07-11 | Total | 23 | video | 0.00 | 0.06 |
| 1994-05-10 | Annular | 75 | video | −0.25 | 0.03 |
| 1995-10-24 | Total | 25 | video | +0.11 | 0.06 |
| 1998-02-26 | Total | 44 | video | +0.16 | 0.04 |
| 1999-08-11 | Total | 19 | video | −0.03 | 0.04 |
| 2002-12-04 | Total | 13 | video | −0.22 | 0.06 |
| 2005-10-03 | Annular | 69 | video | −0.06 | 0.03 |
| 2006-03-29 | Total | 105 | video | +0.09 | 0.16 |

*Method labels are reproduced as in the source CSV ("photoes" as archived). Dates are given in ISO form; the source CSV stores year, month and day as separate fields.*

---

## References

Only works cited in the project source materials are listed. Details are given only where the sources give them; details the sources do not give are omitted rather than supplied.

- Adassuriya, J., Gunasekera, S. & Samarasinha, N. (2011). *Sun and Geosphere* 6(1):17–22.
- Auwers, A. (1891). [Standard radius 959.63″; no further details in the sources.]
- Bush, R. I., Emilio, M. & Kuhn, J. R. (2010). *Astrophysical Journal* 716:1381.
- Dunham, D. W. et al. (1980). *Science* 210:1243.
- Dunham, D. W., Sofia, S., Guhl, K. & Herald, D. (2016). Solar diameter measurements from eclipses as a solar variability proxy. *Proceedings of IAU Symposium 320*, pp. 351–353 (provenance record) / 351–354 (sweep record). doi:10.1017/S1743921316000417.
- Fiala, A. D., Dunham, D. W. & Sofia, S. (1994). Variation of the solar diameter from solar eclipse observations, 1715–1991. *Solar Physics* 152:97–104.
- Guhl, K. (2023). *Journal for Occultation Astronomy* 2023-4, pp. 12–15.
- Guhl, K. & Tegtmeier, J. (2018). *Journal for Occultation Astronomy* 2018-3, pp. 19–21.
- Hayakawa, H., Sôma, M., Rozelot, J.-P. et al. (2026). *Astrophysical Journal Letters*. arXiv:2607.02347; doi:10.3847/2041-8213/ae84b7.
- Hayakawa, H. et al. (2026). arXiv:2604.24503. [1715 re-derivation, 959.98 ± 0.23″.]
- Kilcik, A., Sigismondi, C., Rozelot, J.-P. & Guhl, K. (2009). *Solar Physics* 257:237–250.
- Kubo, Y. (1993). *Publications of the Astronomical Society of Japan* 45:819–829.
- Kuhn, J. R., Bush, R. I., Emilio, M. & Scherrer, P. H. (2004). *Astrophysical Journal* 613:1241.
- Lamy, P. et al. (2015). *Solar Physics* 290:2617–2648.
- Morrison, L. V. & Appleby, G. M. (1981). *Monthly Notices of the Royal Astronomical Society* 196:1013–1020.
- Morrison, L. V., Stephenson, F. R. & Parkinson, J. (1988). Diameter of the Sun in AD 1715. *Nature* 331:421–423. doi:10.1038/331421a0. [Required citation per the precedent sweep: prior published dispute of the 1715 result.]
- Morrison, L. V. (1979). [No further details in the sources.]
- Prša, A. et al. (2016). [IAU 2015 nominal radius basis; no further details in the sources.]
- Quaglia, L., Irwin, J., Emmanouilidis, K. & Pessi, A. (2021). *Astrophysical Journal Supplement Series* 256:36.
- Quaglia, L. (2024). *Journal for Occultation Astronomy* 14(2) (2024-2).
- Rozelot, J.-P. & Kosovichev, A. G. (2026). Do Modern Observations Pin Down the Solar Radius to Converge on New Standards? arXiv:2605.23794.
- Scott (1988). [Watts-angle offset; no further details in the sources.]
- Sigismondi, C. (2008). *AIP Conference Proceedings* 966:341–348.
- Sôma, M. (2012). *Bulletin of the Korean Astronomical Society* 37(1).
- Toulmonde, M. (1997). [No further details in the sources.]
- Van Flandern, T. C. (1970). [No further details in the sources.]
- Wang & Barriot (2021). *Research in Astronomy and Astrophysics* 21:11. [Given names/initials not given in the sweep.]
- Watts, C. B. (1963). The Marginal Zone of the Moon. [Machine-readable form: VizieR catalogue VI/122.]
- Wright, E. & Young (2024). *Astronomical Journal* 168:163, §6.4. [Second author's initial not given in the sources.]

*End of manuscript.*
