# ResearchTrace static preview — release and scientific boundaries

**Release:** NFDI4DS-2026-preview-2026-10-17  
**Distribution:** Public, read-only GitHub Pages HTML. No application backend.  
**Source:** `dennis-fast/scientific-process-core@603d88764cbc6940e5264a77a41acc92a93b7ba6` (**private repository**).  
**Generator:** `tools/build_researchtrace_demo.py` (cases `grinsztajn` and `synthetic`).  
**Frozen scientific inputs:** `research/meta/m5/empirical-slice.yaml`, `research/meta/m7/fifth-slice.yaml`, including its qualified decision.  
**Verification:** The upstream integration suite passed on Python 3.11–3.13, with 302 tests on Python 3.13 at the recorded checkpoint. For this distribution, SHA-256 digests and exact byte lengths of the two HTML exports are recorded in [release-manifest.json](release-manifest.json).

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
