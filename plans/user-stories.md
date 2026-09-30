# FourFold MVP User Stories

## Product scope
FourFold is a 100% on-device 2D word-grouping game built in `/apps/native` with React Native/Expo. The MVP has no authentication, accounts, cloud sync, backend, or server connection. Game content ships with the app and player progress is stored locally. `/apps/web` hosts the marketing site and linked Terms of Service and Privacy pages.

## MVP principles
- Get a first-time player into a puzzle quickly.
- Make every tap feel immediate through visual, sound, and optional haptic feedback.
- Prefer fair, understandable puzzles over clever but ambiguous ones.
- Keep the Daily Four as the main home-screen action.
- Work fully offline after installation.
- Never require an account or internet connection to play.

## Epic 1: First launch and onboarding

### US-01 — Open FourFold for the first time
**As a** new player, **I want** to see the FourFold identity immediately, **so that** I know the app opened correctly.

**Acceptance criteria**
- A short splash screen shows the FourFold logo and a lightweight four-tile animation.
- The splash screen does not delay the app unnecessarily.
- The player reaches Welcome without a login or permission request.

### US-02 — Understand the value proposition
**As a** new player, **I want** to understand the game in one sentence, **so that** I can decide whether to play.

**Acceptance criteria**
- Welcome says: “Find the connection. Complete the four.”
- Supporting copy explains that the player groups 16 words into four categories.
- Primary action is **Start Playing**; secondary action is **How It Works**.

### US-03 — Learn through an interactive tutorial
**As a** new player, **I want** to try the mechanic before committing, **so that** I understand how to play.

**Acceptance criteria**
- Tutorial demonstrates selecting four words, submitting, a wrong guess, a hint, and a correct group.
- Feedback is immediate and non-punishing.
- Tutorial can be skipped and remains under one minute.

### US-04 — Begin the first puzzle
**As a** new player, **I want** to start a real puzzle after onboarding, **so that** I experience the core loop immediately.

**Acceptance criteria**
- A short “Your first FourFold starts now” transition leads to the puzzle.
- The first puzzle is bundled locally and does not require network access.
- After completion, the player reaches the Home screen.

## Epic 2: Home and navigation

### US-05 — See what to do next
**As a** returning player, **I want** the Home screen to show the most important action, **so that** I can start quickly.

**Acceptance criteria**
- Home prominently shows the Daily Four card.
- The card shows status: ready, in progress, or complete.
- The card shows the current streak and a **Play Daily Four** or **Continue** action.
- Bottom navigation includes Home, Packs, Stats, and Settings.

### US-06 — Resume an unfinished puzzle
**As a** player, **I want** to leave and resume a puzzle, **so that** progress is not lost.

**Acceptance criteria**
- Selected groups, mistakes, hints, and board state are saved locally.
- Reopening the app returns the player to the puzzle or lets them continue from Home.

## Epic 3: Core puzzle play

### US-07 — Read the puzzle board
**As a** player, **I want** to see 16 clear word tiles and the goal, **so that** I know what to solve.

**Acceptance criteria**
- The board uses a clean 4×4 layout with readable text and strong contrast.
- The screen shows four groups to solve and the remaining mistake count.
- There is no required timer in the MVP.

### US-08 — Select and deselect words
**As a** player, **I want** to select four words, **so that** I can test a connection.

**Acceptance criteria**
- Tapping a tile visibly selects it with color, scale, and optional haptic feedback.
- Tapping it again deselects it.
- A fifth tile cannot be selected until one of the four is deselected.

### US-09 — Submit a guess
**As a** player, **I want** to submit my four selected words, **so that** the game can evaluate them.

**Acceptance criteria**
- Submit is disabled until four tiles are selected.
- Correct groups lock into a row and reveal a category label and short explanation.
- Solved tiles leave the active grid.

### US-10 — Recover from a wrong guess
**As a** player, **I want** clear but gentle feedback when I am wrong, **so that** I can try again without feeling punished.

**Acceptance criteria**
- The tiles shake briefly and a mistake is deducted.
- No progress is lost.
- At zero mistakes, the puzzle ends with a clear result state.

### US-11 — Shuffle the board
**As a** player, **I want** to rearrange unsolved tiles, **so that** I can see new possible connections.

**Acceptance criteria**
- Shuffle changes the visual order of unsolved tiles only.
- Solved groups remain locked.
- Shuffle does not change the puzzle solution.

### US-12 — Use a hint
**As a** player, **I want** optional help, **so that** I can continue when stuck.

**Acceptance criteria**
- A hint reveals one useful clue or identifies one member of a group.
- The hint is optional and does not require payment or an account in the MVP.
- Hint use is recorded in the result but does not make the puzzle impossible to finish.

### US-13 — Complete a puzzle
**As a** player, **I want** a rewarding completion moment, **so that** solving feels satisfying.

**Acceptance criteria**
- All four groups animate into a completed state.
- Success includes a short chime and optional haptic feedback.
- Results show groups solved, mistakes, hints, completion time, and streak impact.

## Epic 4: Daily, practice, and packs

### US-14 — Play the Daily Four
**As a** player, **I want** one curated daily puzzle, **so that** I can build a simple habit.

**Acceptance criteria**
- The daily puzzle is selected from bundled content using the device date.
- The same device date always opens the same daily puzzle.
- A completed Daily Four cannot be replayed for another result that day.
- Streak logic is local and clearly explained.

### US-15 — Practice without pressure
**As a** player, **I want** unlimited practice puzzles, **so that** I can play without affecting my daily streak.

**Acceptance criteria**
- Practice is available from Home and Packs.
- Practice does not replace or alter the Daily Four.
- Practice results can still count toward total puzzles played.

### US-16 — Browse themed packs
**As a** player, **I want** to browse categories, **so that** I can choose topics I enjoy.

**Acceptance criteria**
- MVP includes Food & Drink, Travel & Places, Movies & TV, Home & Everyday Life, and Nature & Animals.
- Each pack shows its description and progress.
- All launch content is local; no store or server is required.

## Epic 5: Stats and settings

### US-17 — View local stats
**As a** player, **I want** to see my progress, **so that** I can track improvement.

**Acceptance criteria**
- Stats show puzzles completed, current/best streak, average mistakes, hints used, and completion rate.
- Stats are derived from local play history.
- Empty states explain what will appear after the first puzzle.

### US-18 — Control sound, haptics, and appearance
**As a** player, **I want** control over feedback and appearance, **so that** the app fits my preferences.

**Acceptance criteria**
- Settings provide independent toggles for sound effects, music, haptics, notifications, and dark mode if supported.
- Sound and haptic preferences persist locally.
- Music is optional and never required for gameplay.

### US-19 — Manage a local daily reminder
**As a** player, **I want** an optional reminder for the Daily Four, **so that** I can maintain my routine.

**Acceptance criteria**
- Permission is requested only after the value is explained.
- Reminders are local device notifications; no server is used.
- The player can disable or change the reminder in Settings.

### US-20 — Read legal information
**As a** player, **I want** to open the Terms of Service and Privacy Policy, **so that** I can understand the app’s terms.

**Acceptance criteria**
- Settings links to the relevant pages on `/apps/web`.
- The app does not claim to collect cloud data when there is no account or server connection.
- Links gracefully show an unavailable state if the device is offline.

### US-21 — Reset local progress
**As a** player, **I want** to reset my progress, **so that** I can start over.

**Acceptance criteria**
- Reset is inside Settings and clearly marked as destructive.
- A confirmation step explains that local stats, streaks, and puzzle progress will be deleted.
- Cancel leaves all data unchanged.

## Explicitly out of MVP
- Accounts, authentication, cloud save, multiplayer, leaderboards, social profiles, remote content, server analytics, payments, subscriptions, and live content delivery.
