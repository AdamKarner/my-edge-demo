# My Edge v53 — public demo upload checklist

The approved demo is packaged as **three static files** with all original 23 training payloads retained:

- `index.html` — ~0.49 MB
- `assets/training_payload_part1.js` — ~13.81 MB
- `assets/training_payload_part2.js` — ~13.79 MB

These are generated from the v53 split-payload package. HTML loads both companion files using relative references. **Keep this exact layout**.

## Phone-friendly GitHub upload
1. Download `My_Edge_Public_Demo_Upload.zip` from the ChatGPT project conversation and extract it.
2. Open this public `my-edge-demo` repository, branch `main`, and upload `index.html` into repo root. Commit.
3. Create/open folder `assets/` and upload both `.js` files there. Commit.
4. In **Settings → Pages**, select **Deploy from a branch**, **main**, **/(root)**, save.
5. Inspect **Actions / Pages deployment**; test `https://adamkarner.github.io/my-edge-demo/` on phone and tablet. Verify training library and decks, dashboard, role controls, notifications and offline demo.

**Important:** The repository currently must not be described as live until the entry file and payload files exist and deployment is verified. The v53 file contains illustrative, simulated data, not working production integrations. Public content was authorized by project owner. Do not publish private repository documents, API credentials, or operational secrets.

## File checksum verification (SHA-256)
```text
index.html 105753f03e44c0d9df4b5834a1c2b0d4b749cc23e329895a3dfad7c6c8e79da3
assets/training_payload_part1.js 4f6c71494560f5a8665d4af457ab64d1924b2330e34deffd8d13a103d3f6c90b
assets/training_payload_part2.js 0ebb7f6c22494ed87bc7a49b56308ff5332221a7e7d20169a96f855dcaed459b
```
