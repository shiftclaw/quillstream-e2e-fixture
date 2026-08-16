# quillstream-e2e-fixture

Throwaway fixture repository for the **quillstream** end-to-end shared organization.

The quillstream E2E organization connects the DEV GitHub App installation (`152682069`,
account `shiftclaw`) to this repository so that every deployed environment — preview
included — can serve `/api/repos/tree`, `/api/repos/file` and `/api/repos/commit` against
a repository that REALLY exists on GitHub.

Before this repository existed, the shared organization pointed at the synthetic
installation `32000001` that only the locally-mocked transport can serve, so the deployed
preview answered `404 Not Found` on the token exchange and `503` to the browser
(shiftclaw/quillstream#232).

**Nothing here is precious.** Content may be rewritten, truncated or committed to by an
automated test run at any time. Do not store anything you care about.
