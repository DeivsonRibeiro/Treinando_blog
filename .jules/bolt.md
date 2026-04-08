## 2026-02-02 - Avoid lazy loading on above-the-fold images
**Learning:** Adding `loading="lazy"` to images that might be in the initial viewport can negatively impact the Largest Contentful Paint (LCP) metric by delaying image discovery and rendering.
**Action:** Only use `loading="lazy"` for images that are definitely below the fold. For primary or hero images, favor `decoding="async"` and file size optimization.
