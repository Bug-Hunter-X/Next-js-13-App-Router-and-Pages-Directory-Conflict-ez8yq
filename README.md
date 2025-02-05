# Next.js 13 App Router and Pages Directory Conflict

This repository demonstrates a common issue when migrating or working with Next.js 13's App Router alongside the legacy Pages directory.  The presence of both `pages/index.js` and `app/page.js` creates a route collision. 

The problem manifests as unexpected rendering behavior – either the wrong component renders, or the application throws errors. 

**Solution:** Remove one of the conflicting files (`pages/index.js` or `app/page.js`) depending on which approach you want to use. The App Router (`app` directory) is the recommended approach for new projects.