## 2025-02-03 - Confirming Below-the-Fold Images
**Learning:** Adding `loading="lazy"` to images that are above-the-fold can hurt LCP. To safely optimize, I used a Playwright screenshot of the 1280x720 viewport to confirm the image was indeed below the fold.
**Action:** Always verify image position with a screenshot before applying lazy loading.

## 2025-02-03 - Handling Truncated or Complex Filenames
**Learning:** The `list_files` tool and sometimes bash output can truncate long filenames or hide special characters (like multiple dots). This can lead to errors when trying to manipulate those files.
**Action:** Use `ls -b` to see exact filenames and use wildcards (`*`) for robust file operations.
