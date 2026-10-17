# ResearchTrace static preview — release and scientific boundaries

**Release:** NFDI4DS-2026-preview-story-first-2026-10-17  
**Distribution:** Public, read-only GitHub Pages HTML. No application backend.  
**Source:** `dennis-fast/scientific-process-core@9ebb55120244d8aaa4241e0917a11ad8bcd35ae4` (**private repository**).  
**Generator:** `tools/build_researchtrace_demo.py` (cases `grinsztajn` and `synthetic`).  
**Frozen scientific inputs:** `research/meta/m5/empirical-slice.yaml`, `research/meta/m7/fifth-slice.yaml`, including its qualified decision.  
**Verification:** The upstream integration suite passed on Python 3.11–3.13, with 306 tests on Python 3.13 at the recorded checkpoint. For this distribution, SHA-256 digests and exact byte lengths of the two HTML exports are recorded in [release-manifest.json](release-manifest.json).


## Story-first presentation

The first screen now shows the **full bounded negative Finding**, the source-linked
historical and reconstructed accuracy values, the recorded numerical difference,
the explicit reproduction assessment, and an unresolved-cause qualification.
The values are rounded to six decimals **only in the overview**; exact numerical
precision and provenance remain in the record inspector and embedded JSON.

The three evidence panels provide directly inspectable producing activities,
reproduction context and limitations. The typed graph is optional: open
**Explore the typed evidence graph** to inspect the source-native directional
relations, relation labels and backward/forward/full-state scopes. Column
placement is categorical, not a claimed temporal or causal progression.

This UI is a **presentation-layer change**, not new empirical evidence or
a different scientific-state/admission decision. The same generic renderer
also builds the clearly labeled synthetic Claim-based examples.

Automated CI tests (including headless Chromium DOM rendering of the real
comparison and a generic Finding with no metrics) passed on the source
revision. Browser readability and usefulness on actual presentation devices
still require manual review. No automatic user-evaluation conclusions are drawn.

## What the Grinsztajn case actually shows

The public `index.html` graph is an exact static **projection of already recorded, qualified scientific state**. It contains two distinct RandomForest/electricity test results:

- Historical released default score: **0.8457756371663656**.
- Bounded deterministic CPU reconstruction: **0.8507425245835842**.
- Difference (rerun minus historical): **0.004966887417218624**.

The reconstruction's execution status is `completed`, while its reproduction assessment is `not_exactly_reproduced`. The resulting bounded Finding has `negative_result` status and an explicit unresolved-cause Limitation. No Claim was synthesized from the discrepancy. Recorded estimator seed sensitivity does not establish the cause.

The case does **not** prove historical error, corrective supersession, causal attribution, exact environment equivalence or failure of the source paper's conclusions. It is not a new independent rerun performed for this public distribution.

## Scope and public access

The original scientific state and reproducibility procedures remain controlled by the **private upstream repository**. The published HTML embeds the **selected downstream view** of these records: selected values, graph nodes and relations, source identifiers, source paths and provenance metadata. Relative private source-record paths may appear; they are not publicly resolvable. This public release alone cannot independently reproduce the underlying computation or audit the source repository.

The [synthetic example](examples/synthetic.html) exercises additional Claim-centered paths, support, contradiction and other structures. It is explicitly synthetic, not another empirical study.

Public-disclosure screening on the generated files found no credential markers, email addresses, absolute runner paths or external runtime dependencies. This is a bounded content check, not a blanket security certification.

## Integrity and deployment

The **only files deployed to Pages** are `index.html`, `examples/synthetic.html` and `release-manifest.json`. The GitHub Actions workflow validates each HTML against the checked-in manifest before uploading the static site. No private repository checkout or token is required in the **public** Pages workflow.

For a new release, regenerate from a **deliberately selected and reviewed** private upstream revision, audit the resulting exported HTML, replace the two files and update their manifest checksums in the same reviewed release. Do not automatically pull the private repository or publish arbitrary unreviewed future changes.

**Remaining conference release check:** Open the deployed site and an offline copy on the presentation laptop, verify Finding selection and limitation navigation, and rehearse with the network disabled. Automated syntax/build checks do not replace this manual review.
