## 2025-02-06 - Image Optimization and Contextual Verification
**Learning:** Performance optimizations must be applied to the correct and complete version of the codebase. A previous broken state led to a false conclusion that the main image was above-the-fold (y=126px). After restoring the full blog content, verification confirmed the image is actually below-the-fold (y=792px) in a standard 1280x720 viewport.

**Action:** Always verify element positions against the production-ready layout. Use \`loading="lazy"\` and \`decoding="async"\` for images verified to be below-the-fold to reduce initial page weight and main-thread blocking.
