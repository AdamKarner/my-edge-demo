# My Edge — public interactive demo

This repository is the **public demo only** for My Edge, the EDS mobile/tablet companion. The private application and reference documents remain in `AdamKarner/my-edge`.

**Deployment status:** Source upload and Pages activation pending. This repository does not yet contain a usable demo entrypoint.

## Publishing approved v53
1. Obtain the reviewed, sanitized v53 browser build from the private repository, not the unreviewed source snapshot.
2. Copy its entrypoint to this repository's root as `index.html`; preserve any relative `assets/` files. A browser variant in the private repo references two `training_payload_part*.js` assets; include them if that variant is selected.
3. Before pushing publicly, verify that the HTML and JavaScript do not contain authentication tokens, customer information, internal-only URLs, private source, or any live integrations.
4. Commit the static demo files to `main`.
5. In **Settings → Pages → Build and deployment → Source**, select **GitHub Actions**. The workflow `Publish My Edge demo` validates `index.html` and deploys it.
6. Verify the live page at https://adamkarner.github.io/my-edge-demo/ on phone, tablet and desktop.

**Important:** The verified preserved source in the private repo is `prototype/my-edge-v53.html`, 28,087,791 bytes, SHA-256 `5ff9c2723abc2fe17e5df1aed9e9c01f33d3381a57c49f80c34da0d61f3fe7e9`. The separate browser variant has not been established to be byte-identical; do not label it verified against that hash.

The prototype uses simulated data; this demo must not be presented as production integration.
