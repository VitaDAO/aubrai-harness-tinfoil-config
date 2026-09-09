# aubrai-harness-tinfoil-config

Public deployment manifest for the **staging** Aubrai harness enclave (Tinfoil confidential container).

| File | Purpose |
|---|---|
| `tinfoil-config.yml` | Deployment manifest: pinned image digest, resources, secret names, exposed HTTP paths |
| `.github/workflows/tinfoil-build.yml` | Attestation workflow that runs on every release tag |

Source code lives in the private `VitaDAO/aubrai-harness` repository; its `deploy/tinfoil/README.md` is the release runbook.
Secrets are referenced by organization-vault name only and are released solely into a correctly attested enclave.
