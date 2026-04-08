## 2025-01-31 - LCP and Lazy Loading Caution
**Learning:** Adding `loading="lazy"` to images that are close to or in the initial viewport can negatively impact the Largest Contentful Paint (LCP) metric by delaying the start of the image fetch.
**Action:** Always verify the position of an image before adding `loading="lazy"`. If in doubt or if it's the primary image, omit lazy loading and consider `decoding="async"` or `fetchpriority="high"` instead.
