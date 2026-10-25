# Train Buddy V16 — GitHub staging

This folder contains a staging copy of the recovered `BanDOG-Telegram-Game-v16.zip` `index.html`.

## What this stage does
- Adds the game at `/train-buddy/` without replacing the existing site's root page.
- The main site adds a **Train Buddy Preview** link.
- Keeps the V16 source file's gameplay code unchanged in the staged copy.

## Important status
- The source archive describes this as V16 based on V15 Daily, with Buddy Coins, daily mission rewards, and daily streak rewards.
- This is still a single-file browser game using `localStorage`; it is not yet integrated with Telegram Web Apps authentication.
- It does not yet provide a server-backed shared leaderboard or authoritative cross-device currency/score storage.
- The homepage and game-folder changes are staged on the `feature/train-buddy-v16` branch for review. They have not been merged to `main`.

## Next stages (not implemented here)
1. Verify the preview in a real browser and confirm V16 behavior is preserved.
2. Merge and publish the static preview only after review.
3. Configure `@BanDOGTrainBuddyBot` in BotFather to open the published HTTPS URL.
4. Add a server-side backend and database with Telegram init-data validation before global leaderboards or shared Buddy Coins are enabled.

Never commit Telegram bot tokens or other secrets into this repository.
