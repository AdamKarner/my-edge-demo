# My Edge — interactive demo

Public demo-only repository for My Edge, the EDS agent phone/tablet companion. Development source remains private in `AdamKarner/my-edge`.

## GitHub Pages
Use **Settings → Pages → Deploy from a branch → main → / (root)**.

Expected site URL once an approved demo is uploaded and Pages is enabled:
https://adamkarner.github.io/my-edge-demo/

**Status:** The public repository does not yet contain `index.html`. It is not a live interactive demo.

## Publishing the approved v53 prototype
The preserved original v53 HTML is in the private repository at `prototype/my-edge-v53.html` (28,087,791 bytes; SHA-256 `5ff9c2723abc2fe17e5df1aed9e9c01f33d3381a57c49f80c34da0d61f3fe7e9`). There is also a distinct browser variant in `prototype/My_Edge_Interactive_v53_Official_EDS_Branding.html` and associated `prototype/assets/training_payload_part1.js`, `training_payload_part2.js`; do not assume equivalent versions without verification.

Before publishing, review and sanitize HTML and all referenced JavaScript for secrets, real customers or dealers, internal URLs and live integrations. Transfer only cleared demo files: place the HTML as `index.html` at the repository root and required static assets under `assets/`. Large HTML files may need Git CLI rather than GitHub's browser upload.

Validate the site on desktop, tablet and phone. Prototype actions and data are simulated, not live Edge or PCRS functionality.
