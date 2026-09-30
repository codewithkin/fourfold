# FourFold MVP User Flows

## Product and state assumptions
- Native app: `/apps/native` using React Native/Expo.
- Marketing/legal site: `/apps/web`.
- No auth, account, backend, cloud, or server connection.
- All puzzle packs ship in the app bundle.
- Progress, settings, streaks, and unfinished puzzles are stored on-device.
- A local date-based key selects the Daily Four. The app should handle a device-date change without crashing or duplicating a completed daily result.

## Global navigation
**Splash → Home** after the first launch has been completed.

Bottom tabs:
1. **Home** — Daily Four, continue state, quick entry points.
2. **Packs** — themed content and practice.
3. **Stats** — local performance history.
4. **Settings** — preferences, reminders, legal links, reset.

The active puzzle is always reachable through a **Continue** action when unfinished.

## Flow 1: First launch

`Open app`
→ Show Splash for 1–2 seconds
→ If `firstLaunch = true`, show Welcome
→ Otherwise show Home.

### Welcome
- Headline: “Find the connection. Complete the four.”
- Supporting text explains 16 words, four groups, and a short session.
- Actions: **Start Playing**, **How It Works**.
- No login, account creation, or permission prompt.

### Onboarding choice
- **How It Works** → interactive tutorial.
- **Start Playing** → interactive tutorial, with a visible **Skip** option.
- **Skip** → first-puzzle intro.

### Interactive tutorial
1. Select four obvious words.
2. Submit and show a correct group.
3. Demonstrate an incorrect guess with gentle shake feedback.
4. Show the hint and remaining-mistake indicator.
5. Show a completed group and category label.

`Tutorial complete or skipped` → First-puzzle intro → **Begin Puzzle** → first bundled puzzle.

## Flow 2: First puzzle to Home

`Begin Puzzle`
→ Puzzle screen
→ Player solves or reaches game-over state
→ Completion/Game Over result screen
→ Show groups, mistakes, hints, time, and streak impact
→ Optional **Share Result** using the native share sheet
→ **Continue to Home**.

On first completion, Home should show the Daily Four as complete and explain where Practice and Packs are located.

## Flow 3: Returning user

`Open app`
→ Splash
→ Read local state.

- If an unfinished puzzle exists → Home shows **Continue**; tapping it opens the saved puzzle.
- If today’s Daily Four is incomplete → Home shows **Play Daily Four**.
- If today’s Daily Four is complete → Home shows completion status and **Practice**.
- If local reminder is enabled, the device may show a local notification; opening it routes to Home or directly to the Daily Four.

## Flow 4: Home

Home layout:
1. Header: FourFold logo, Settings shortcut.
2. Main Daily Four card: ready, in progress, or complete.
3. Secondary cards: Practice, Packs, Stats.
4. Bottom navigation.

Actions:
- Daily card `ready` → Daily Four puzzle.
- Daily card `in progress` → Resume saved puzzle.
- Daily card `complete` → Result summary or Practice.
- **Practice** → Practice selection.
- **Packs** → Packs tab.
- **Stats** → Stats tab.
- **Settings** → Settings tab.

## Flow 5: Puzzle play

`Open puzzle`
→ Load local puzzle data and saved state
→ Show 4×4 word grid, solved-group area, mistake counter, Submit, Shuffle, Hint, and exit/back action.

### Selecting words
- Tap unsolved tile → selected state, optional click sound/haptic.
- Tap selected tile → deselect.
- Four selected → Submit enabled.
- Fifth tap → do nothing or explain “Choose four words.”

### Submit decision
- Fewer than four selected → no submission; show a small instruction.
- Four selected + correct → lock group, show category/explanation, play success feedback.
- Four selected + incorrect → shake, deduct one mistake, clear selection, allow retry.
- Mistakes reach zero → show Game Over; allow result and Practice/Home.
- Four groups solved → show completion celebration and Results.

### Utility actions
- Shuffle → randomize only unsolved tiles.
- Hint → reveal a clue/member and record hint usage.
- Back/exit → save state locally and return to Home; no confirmation is needed for normal exit.

## Flow 6: Daily Four

`Home → Play Daily Four`
→ Create key from local calendar date
→ Load bundled puzzle mapped to that key
→ If incomplete, resume saved state
→ If complete, show the saved result instead of starting a second Daily result.

At completion:
- Update streak according to the local streak rules.
- Save result and completion date.
- Show **Share Result**, **Practice**, and **Home**.

## Flow 7: Practice and Packs

`Home → Practice` → Choose a pack or continue the next available local puzzle → Puzzle screen.

`Packs tab`
→ Show five launch categories:
- Food & Drink
- Travel & Places
- Movies & TV
- Home & Everyday Life
- Nature & Animals

`Select pack` → Show description, completed/available count, and **Play** → Load next local puzzle.

Practice never changes Daily Four completion or streak. It may contribute to total-puzzle stats.

## Flow 8: Results and sharing

`Puzzle complete`
→ Results screen
→ Show solved categories, mistakes, hints, time, and streak.

- **Share Result** → native OS share sheet with a text-only or emoji-safe result card; do not require an account.
- Share cancelled → return to Results.
- **Practice** → Practice selection.
- **Home** → Home.

## Flow 9: Stats

`Stats tab`
→ Read local history
→ Show completed puzzles, current/best streak, average mistakes, hints used, and completion rate.

- No history → show a friendly empty state and **Play Daily Four**.
- Stats are read-only in MVP; reset is handled in Settings.

## Flow 10: Settings

`Settings tab`
→ Show:
- Sound effects toggle
- Music toggle
- Haptics toggle
- Daily reminder toggle/time
- Dark mode toggle if implemented
- Terms of Service
- Privacy Policy
- Reset Progress
- App version/about

### Reminder
`Enable reminder` → Explain local notification → Request OS permission → If granted, schedule local reminder → If denied, leave toggle off and explain how to enable it later in system settings.

`Disable reminder` → Cancel local reminder → Persist setting.

### Legal pages
`Terms` or `Privacy` → Open `/apps/web` URL in browser/web view. If offline, show a retry/unavailable message without blocking gameplay.

### Reset
`Reset Progress` → Confirmation modal →
- Cancel → Settings unchanged.
- Confirm → Delete local stats, streaks, saved puzzle states, and settings that are explicitly included in reset → show success → return to Home.

## MVP edge cases
- App closes during a puzzle: restore the latest saved state.
- Device is offline: all game modes using bundled content still work.
- OS denies notifications: gameplay remains fully available.
- Device date changes: avoid duplicate Daily results and surface a simple “Daily Four unavailable/updated” state if needed.
- Puzzle content is missing or invalid: show a recoverable error and return to Packs/Home; never leave the player on a blank screen.
- Very long words: wrap or scale text without making tiles unreadable.
- Accessibility settings: preserve contrast, touch targets, and readable text sizes.
