# Local verification record

Scope: local implementation verification, not tagged-release or installed-client acceptance. Source identity is the exact skills.lock.json snapshot at verified upstream commit dc963c182b7f82d2ee7abe63d0fa6cb29aeef138; no version tag is claimed.

| Check | Actual result | What it establishes |
|---|---|---|
| Agent Plugins 1.0.0 static validator | PASS, 11 skills | Portable discovery and manifest/MCP rules checked locally |
| Local Markdown/resource links | PASS | Referenced package files resolve |
| Source snapshot hash check | PASS | Full declared source bytes match the lock |
| Plugin Harness entry tests | PASS, 3 | Absolute external store required; plugin store denied |
| Package snapshot tests | PASS, 2 | Relocated source identity and changed-source detection |
| Bundled Harness regression suite | PASS, 128 | Existing state, dispatch, recovery and authority regressions |
| Existing-browser preview check | PASS | Bundled demo synchronization/independent mode/tab state/private-input non-replay |
| Actual viewports | PASS | Phone iframe 390×884, Pad iframe 768×1024; direct Mobile/Tablet/Desktop browser pages at 390×884, 768×1024, 1280×1024 |

The browser receipt/screenshots are generated under dist/preview-evidence by verify_preview.cjs. The demo is explicitly the bundled sample, not a claimed user-specific UI delivery. Real native image generation and baoyu/API calls were not requested for this packaging validation and were not executed. Model quality, host installation and production frontend integration remain NOT VERIFIED.

These local results were recorded before source publication. Current remote CI status is available in the repository's GitHub Actions page. The distributable archive is generated only after schema, link and snapshot checks. Tagged releases, marketplace addition and installing updates remain separate actions.
