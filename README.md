VEYFIR UPDATE ACCEPTANCE TEST — NOT A PRODUCT RELEASE
Original source: 5234f1487b7aa6603fb2152c3de1088d42f1c046
Proposed branch: codex/windows-web-e2e-20261029
Test public-key SHA256: F8E7F2FDA938A19EDE4935802E711B4B643B01E4F668122894138D3A7589A334
Separate AppId/mutex/profile. No OBS/FFmpeg native payload or runtime installer. Normal WPF application/update UI, no recording qualification.
Do not run while gaming. Close production Veyfir before testing to avoid global-shortcut conflicts. All test windows request the left display.
Nothing published or installed by preparation. Exact owner approval and account access are required before publishing even this dedicated branch.
Local loopback-only test: False. Local HTTP validates install/update/signatures, not production TLS or GitHub delivery. No certificate, firewall or security-policy changes are needed.
Also verify current/no reinstall, bad signatures/platform metadata, offline, interruption/retry and no downgrade. Compilation and signed-bundle checks do not establish this acceptance.
The matching Windows test source archive remains local and is excluded from the proposed public branch. Do not upload DerivedSource/.git, development evidence or FeedStages wholesale. Private test key existed only in preparation memory and is cleared; rebuild with a new test identity if additional signatures are needed.
The production installer/feed/key and installed user data remain separate. Never send these9.1.x test builds as official Veyfir.
HOSTED TRIAL: actual GitHub release assets, dedicated test-feed branch, test signing key and new installation identity.
Do not upload ProposedBranch wholesale. Prepare the separate allowlisted HostedUpload set; owner approval must identify its exact hashes before any public writes.
After approval: create each windows-v9.1.x tag as a clearly named PRERELEASE, never Latest, targeting only the test branch. Upload only its pinned test installer; the A release also carries the unchanged test bootstrap and notices.
Publish only the approved test feed pair to the dedicated test branch. Advance A, B, C, D in order: same bootstrap A-to-B, then normal in-app B-to-C-to-D. Never edit the production feed/main branch or website.
This lightweight fixture tests hosted transport and normal update UI, not the OBS runtime or full-product recording. Those acceptance criteria remain separate.
