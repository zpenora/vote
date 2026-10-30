# AHMED HQ website | GitHub Pages edition

A standalone black-and-gold HTML/CSS/JavaScript landing page with a **clickable vote button**, star-rating reviews and helpful reactions. No Supabase, accounts, servers, tokens, or build tools are required.

## Publish on GitHub Pages

1. Create a new public GitHub repository (example: `ahmed-hq`).
2. Upload **`index.html`** from this ZIP to the repository root and commit it.
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch **main** and folder **/(root)**, then save.
6. Open the URL that GitHub Pages provides, typically `https://YOUR_USERNAME.github.io/ahmed-hq/`.

The website contains the invite link: https://discord.gg/naHB2YVwKR

## Voting and reviews limitations

**Important**: GitHub Pages hosts static content and cannot store a single shared vote/review count by itself. This version uses browser `localStorage`:

- Visitors can click **🔥 Click to Vote**; the button changes to **✓ Voted! Click to Undo**.
- Their vote is retained on refresh, but only on that device/browser.
- Visitors can leave a 1–5 star review; the review is visible only to that same browser.
- Stats are labeled to make clear they are per-browser, not global.
- Clearing site data or using a different browser resets the local vote/review.

To support real shared votes/reviews across all users, you would need a separate service or server-side storage (not available through pure static GitHub Pages alone).
