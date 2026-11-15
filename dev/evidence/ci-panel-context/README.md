# CI panel context follow-up

Credit: Jpp-matata’s panel in Community31; dr-chambre’s two non-blocking review suggestions. Exact reviewed/tested base `0a636a84c281e341850ee92aca70b9d149419ddf`; foldable code commit `7ea08f1bc1224ca3ef955ed4fcde372415a31c8a` (one commit, six files).

Adds one translated paragraph and guidance link: compare failures with the same tests/build settings on the base before calling regressions, and disclose slow matmul_v4_rc_stage3_* suites excluded from unit totals. No API/count/status/JavaScript change. English/German plus Spanish/French/Chinese source-reviewed; no native-speaker review.

Actual macOS arm64/Python3.11.14 results with all8 pinned requirements: site build0 without translation warnings,21 maintained Python tests pass. All81 original source blobs verified before patching. Generated HTML in all5languages contains both messages/link; remove only the inserted paragraph and each developer page matches the unmodified-base build exactly. All34 other generated files are byte-identical. Logs and commands/dependency versions accompany this entry; personal paths in public evidence are sanitized.

Executed commands in isolated patched source: `python3.11 -B site/build.py --out <local-task>/rendered` and `python3.11 -B -m unittest discover -s site/tests`. The unmodified-base build was used only for content comparison, not a new runtime-regression claim. To reconstruct from the code branch, install the pinned site/requirements.txt into an isolated Python3.11 environment and use the same build/test entry points. That reconstruction from the publication commit was not separately executed; committed source bytes match the validated files.

Not run: JavaScript tests, browser/live-fetch/layout, native BTX tests/builds, seeds or hosted jobs. No release qualification. Final source/evidence review reverified all81 files and artifact hashes without rerunning tests. This evidence does not republish the private/group catch-up note or internal cleanup logs.
