# FourFold listing and player research

## 1. Recommended positioning and player promise

**Position FourFold as a calm, fair, explainable word-grouping game—not as a generic brain-training app and not as a copy of a competitor.** The core promise is:

> **Spot the pattern. Finish the four.** Group 16 words into four fair categories, understand why each group works, then return for one quiet Daily Four or keep playing in local Practice and five themed packs.

FourFold’s differentiators are concrete and MVP-compatible:

- **A legible 16-to-4 loop:** a real 4×4 board, four groups of four, category labels, and short explanations.
- **Low pressure:** no required timer, gentle wrong-guess feedback, optional hints, and Practice that does not change the Daily Four streak.
- **Private ownership:** bundled content, progress, stats, streaks, settings, and optional reminders stored on-device; no account, backend, cloud sync, payments, or server analytics in the MVP. [1] [2]
- **Enough depth without a volume claim:** Daily Four, Practice, and five bundled packs—Food & Drink, Travel & Places, Movies & TV, Home & Everyday Life, and Nature & Animals. [1] [2]
- **A quiet completion loop:** results show solved groups, mistakes, hints, completion time, and streak impact; native text sharing is optional and spoiler-safe. [1] [2]

Use **“fair”** and **“explainable”** only as content-quality commitments: each board must have one intended partition, no equally defensible alternate solution, and a readable explanation. Do not promise “easy,” “always solvable,” or a guaranteed streak. The 16-word format is recognizable, but public criticism of comparable games repeatedly flags overlapping categories, obscure knowledge, and arbitrary-feeling answers; this is qualitative evidence, not a population estimate. [20] [21] [22] [23]

**Hard boundary for all store assets:** say **“play offline after installation”** and **“progress stays on this device”** only after the final release-build and dependency audit. Do not imply global synchronization, endless remote content, cloud recovery, multiplayer, leaderboards, live events, or cross-device progress. The OS share sheet, browser legal pages, app stores, and any future SDK are outside the game’s local storage boundary. [1] [2] [37] [38]

## 2. Keyword and discovery map

### 2.1 Intent map

| Priority | Cluster | Terms to validate | Best use | Evidence boundary |
|---|---|---|---|---|
| Primary | Mechanic | word groups; word grouping; word group puzzle; group words; four groups; 16 words; category puzzle | Apple title/subtitle/keywords; Google title/short/full description; first screenshot | These are observed competitor/listing phrases and high-intent hypotheses, not guaranteed-volume terms. [14] [15] [16] |
| Primary | Daily habit | daily word puzzle; daily word game; daily challenge; daily puzzle; daily word connections | Subtitle, promotional text, Google short description, Daily Four page/listing | FourFold has one local date-selected Daily Four; do not imply a globally synchronized feed. [1] [2] |
| Secondary | Puzzle genre | word puzzle; word association; logic puzzle; brain teaser | Natural description prose and experiments | “Logic puzzle” and “brain teaser” are broader and can attract mismatched traffic; avoid unsupported cognitive/health efficacy claims. [14] [15] |
| Secondary | Depth | practice puzzle; themed word puzzles; category game; word association game | Full description, packs custom page/listing | Use only to describe the shipped Practice and five packs. [1] [2] |
| Long-tail | Explicit intent | group 16 words into four; word grouping puzzle offline; four groups word puzzle; daily category word puzzle; calm word grouping game | Apple Ads Search Match/exact campaigns; Google search-keyword custom listing; campaign landing pages | Long-tail demand is unverified; validate before spending scarce metadata space. [14] [15] |
| Mood/benefit | Calm/privacy | calm word puzzle; quiet puzzle; low-pressure puzzle; no timer; offline word game; on-device progress; no account | Subtitle/description, calm/offline custom pages, creative | These are benefit hypotheses and product claims, not evidence that a majority prefers them. [17] [18] |
| Negative/avoid | Policy and mismatch | NYT; Connections; Wordle; Red Herring; Connections-style; best; #1; addictive; brain training; IQ; improve your memory; infinite puzzles; new puzzles forever; cloud sync; leaderboard; multiplayer; free/price claims; download now | Never use in FourFold metadata or creative unless a factual, policy-reviewed context requires it | Apple and Google prohibit misleading, irrelevant, competitor, ranking, price, or unsupported claims. [3] [4] [5] |

**Keyword rule:** use the owned phrase **“word groups”** or **“word grouping”** before abstract genre language. “Connections-style” is recognizable research language but should not be FourFold metadata; competitor names and copycat positioning create policy and confusion risk. [3] [4] [14]

### 2.2 Validation workflow

1. **Baseline:** capture the exact locale, field, character/byte count, date, and submitted hypothesis in a metadata sheet.
2. **Apple discovery:** run Search Match and Apple Ads keyword suggestions; separate discovery from brand/category campaigns, record actual queries and installs, and promote converting queries to exact match. Apple recommends this discovery-to-exact workflow. [13]
3. **Google discovery:** create one search-keyword custom listing only for a validated mechanic cluster and one for a daily cluster; keep each page’s screenshots and copy faithful to the intent. Google supports search-keyword custom listings and keyword variations. [9]
4. **Store read:** compare impressions with product-page/listing views, downloads, conversion, and review/support language. Impressions alone cannot establish keyword success; Apple and Google do not publish a complete stable ranking formula. [5] [6] [10]
5. **Review mining:** after launch, collect the exact words players use for the mechanic, daily habit, calmness, fairness, hints, and offline use. Keep repeated patterns separate from individual anecdotes.
6. **Locale gate:** localize the puzzle corpus and UI before adding a locale. Do not mechanically translate English keywords; test search relevance, long words, category wrapping, dates, and conversion in-market. [11] [12]

### 2.3 Platform differences

| Topic | Apple App Store | Google Play |
|---|---|---|
| Main text surfaces | Name, subtitle, keywords, promotional text, description, category | Title, short description, full description, category, feature graphic/video |
| Search posture | Text relevance from title, subtitle, keywords, primary category plus behavior such as downloads, ratings, and reviews; keyword field has a documented 100-byte reference, while another Apple guide says 100 characters—validate in App Store Connect. [5] [7] | Relevance plus quality, ratings/reviews, downloads, user behavior, personalization, and surface-dependent signals; weights are proprietary. [6] |
| Custom targeting | Up to 70 custom product pages; distinct assets, keywords, promotional text, localization, and URLs; analytics become useful after at least five first-time downloads. [8] | Up to 50 custom store listings, including country, ad, audience, lapsed, and search-keyword segments. [9] |
| Testing | Product Page Optimization can test up to three treatments; wait for platform confidence rather than reacting to a small swing. [19] | Store listing experiments support one asset variable at a time, up to two variants; run at least a week to cover weekday/weekend patterns. [10] |
| Video | Optional app preview, 15–30 seconds, up to 500 MB, app-only footage, portrait or landscape. [18] | Optional YouTube URL; public/unlisted, embeddable, ad-free, captioned, with real gameplay in the first 10 seconds and at least 80% representative gameplay recommended. [17] |

## 3. Exact Apple App Store listing draft

**Recheck every limit, trademark, availability result, category label, and locale behavior immediately before submission.** Apple’s public references currently contain a 100-byte versus 100-character keyword discrepancy, so the App Store Connect validator is authoritative for the target locale. [5] [7]

### 3.1 Metadata

- **App name:** `FourFold: Word Groups` — **21 characters / 21 UTF-8 bytes**.
- **Subtitle:** `Calm daily word puzzles` — **23 characters / 23 UTF-8 bytes**.
- **Promotional text:** `A calm Daily Four: group 16 words into four fair categories. Practice by theme, use a hint when needed, and keep your progress on your device.` — **142 characters / 142 UTF-8 bytes**, below the current 170-character reference. Promotional text is for current conversion messaging; Apple says it does not affect search ranking. [7] [5]
- **Keyword field starting hypothesis:** `association,logic,offline,practice,category,streak,calm,shuffle,hint` — **68 ASCII characters / 68 bytes**. Validate acceptance and demand per locale. Remove terms already covered by title, subtitle, company name, or category if applicable; do not treat this as a ranking guarantee. [5] [7]

**Why this split:** the name carries brand plus mechanic; the subtitle carries daily use and mood; the keyword field tests distinct mechanic, intent, and recovery terms. Do not duplicate `word`, `groups`, `daily`, or `puzzle` merely because they feel relevant—first validate whether their coverage and category treatment already make them redundant.

### 3.2 Description (plain text; draft is below 4,000 characters)

```text
Find the pattern. Finish the four.

FourFold is a calm word-grouping puzzle built around a simple challenge: sort 16 words into four groups of four. Each group has a category to discover, and each solved group comes with a clear explanation.

Start with the Daily Four, a short local puzzle selected for your device date. Finish it to update your local streak, then keep playing without pressure in Practice or explore five themed packs:

• Food & Drink
• Travel & Places
• Movies & TV
• Home & Everyday Life
• Nature & Animals

FourFold is designed for a quiet, satisfying session:

• Read a clean 4×4 word board.
• Select four words and test a connection.
• Shuffle the unsolved tiles when a new view helps.
• Use an optional hint when you need a nudge.
• Get gentle feedback for a wrong guess and a clear explanation for a correct group.
• See mistakes, hints, completion time, streak impact, and local stats.
• Share a spoiler-safe result through your device’s share sheet.

No account is required. After installation, bundled puzzles, progress, streaks, stats, settings, and optional reminders work on your device. Practice never changes your Daily Four streak. There is no required timer, server leaderboard, cloud save, or online connection needed to play.

FourFold is a small daily reset for word lovers, puzzle fans, and anyone who enjoys finding the idea that brings four words together.
```

The description explains the core loop before secondary features, names all five launch packs, and avoids claims of global synchronization, endless supply, cloud sync, payments, multiplayer, or server analytics. Keep it synchronized with the final binary and privacy disclosures. Apple requires accurate metadata and actual in-app representation. [3] [7]

### 3.3 Category, age, privacy, and support checklist

- **Primary category:** Games; choose the most accurate available Games subcategory, expected to be **Puzzle**, in the final App Store Connect taxonomy. A secondary category is optional and should describe the core experience, not the pack themes. Categories control browsing/filter and Games-versus-Apps placement; verify in the current UI. [12]
- **Age rating:** answer from the final bundled corpus and actual UI. Review Movies & TV content for recognizable titles, characters, logos, quotes, artwork, or music rights before shipping or showing it in assets. [3]
- **App Privacy:** complete from a final release-build and SDK/network audit. On-device-only gameplay can qualify as not collected when it never leaves the device, but third-party SDK behavior must be included and disclosures must stay accurate. [37]
- **Support URL:** public, reachable support page with contact route, version/build context, FAQ for offline/local progress, and a way to report an ambiguous puzzle.
- **Privacy URL and Terms:** public HTTPS pages; distinguish the native app from browser legal traffic and OS share recipients.
- **Screenshots/previews:** upload only real supported-device captures. Apple allows 1–10 screenshots and up to three previews per supported device size/language; recheck current dimensions and device matrix before upload. [18] [19]
- **Ratings prompt:** use Apple’s system API after several meaningful completions including a Daily Four, on a natural result-screen pause. Never use a custom imitation, sentiment gate, reward, or five-star request. Apple’s system prompt is automatically limited to three appearances in 365 days. [24]
- **Reviews:** respond with empathy and a concrete fix or explanation; do not solicit only positive ratings or disclose personal information. [24] [25]

### 3.4 Apple custom product pages

Start with three, not a speculative portfolio:

| Page | Audience/traffic | First frame | Keyword family | Asset emphasis |
|---|---|---|---|---|
| Daily Four | Daily-puzzle searches and creator links | `One quiet puzzle for today.` | daily, challenge, streak | Home Daily Four card, result, local streak |
| Calm/offline | Low-pressure/privacy intent | `Word puzzles, offline and on-device.` | offline, calm, practice | Board, Settings/local stats, no-timer proof |
| Themed packs | Theme-led campaigns | `Practice by theme.` | category, word groups, practice | Packs screen, five named themes, board |

Route only matching traffic. Wait for enough first-time downloads to interpret conversion; run one major asset hypothesis at a time. [8]

## 4. Exact Google Play listing draft

**Recheck the current Play Console validator immediately before submission.** Google currently documents title ≤30 characters, short description ≤80, and full description ≤4,000; metadata must be concise, accurate, natural, and not a keyword block. [4] [6]

### 4.1 Metadata

- **Title:** `FourFold: Word Groups` — **21 characters** (≤30).
- **Short description:** `Group 16 words into four. Calm daily puzzles, themed packs and practice.` — **72 characters** (≤80).

### 4.2 Full description (draft; below 4,000 characters)

```text
FourFold is a calm daily word puzzle about finding the pattern between words.

Group 16 words into four categories on a clear 4×4 board. Select four tiles, submit your guess, and reveal a group with its category explanation. A wrong guess gives you gentle feedback so you can look again; an optional hint can help when you are stuck.

Play the Daily Four for a small daily ritual and a local streak. When you want more, choose Practice or explore five themed packs:

• Food & Drink
• Travel & Places
• Movies & TV
• Home & Everyday Life
• Nature & Animals

FourFold is made for short, low-pressure sessions. There is no required timer. Shuffle the unsolved tiles, solve at your own pace, then see your mistakes, hints, completion time, and streak impact on the result screen. Local Stats show completed puzzles, current and best streaks, average mistakes, hints used, and completion rate.

Your play stays simple and private. No account is required. After installation, the bundled puzzles, progress, stats, streaks, settings, and optional Daily Four reminder stay on your device. FourFold works offline and Practice never changes your Daily Four streak. Share a spoiler-safe result through the Android Sharesheet when you want to show how you did.

Find four fair groups. Take a quiet minute. Play FourFold.
```

Do not repeat the short description verbatim in the full description, add a keyword block, claim “best,” imply competitor affiliation, or make price/ranking/health claims. [4] [6]

### 4.3 Feature graphic concept

**Working master:** 1024×500, warm neutral field, centered FourFold four-tile mark, cropped real 4×4 board, and one line: **`Spot the pattern. Finish the four.`** Keep key content inside a center-safe area because Play surfaces and the video play button can obscure edges. Use no device frame, store badge, price, ranking, testimonial, or “download now” CTA. Confirm the current Console validator before export. [17]

### 4.4 Custom listings

Start with two focused pages:

1. **Daily Four/streak:** Home card first, local streak/result proof, daily-intent copy and campaign URL.
2. **Themed packs/Practice:** Packs first, five themes, practice depth, theme-specific campaign URL.

Add a search-keyword listing for a mechanic cluster only after Play search/conversion data exists. [9]

### 4.5 Category, age, privacy, and support checklist

- **Category:** Games, with the most accurate Puzzle-style taxonomy available; verify current Play Console classification.
- **Target audience/content rating:** declare the actual intended age groups and complete IARC from the final corpus; do not select children solely to widen reach. Child-inclusive selection can trigger Families requirements. [26]
- **Data safety:** every published app must complete the form and provide a public Privacy Policy, including no-data apps. Audit Play Core review behavior, OS sharing, permissions, Expo/native dependencies, and every SDK before final answers. [38]
- **Privacy/Support URL:** public HTTPS Privacy Policy and support destination; explain local storage and that selected share text is handed to the OS Sharesheet/recipient app.
- **Ratings/reviews:** call the native Play in-app review API only after sufficient demonstrated play, with an app-owned cooldown. Do not ask whether the player likes the app, request five stars, force a dialog, or offer a reward; Play quotas may suppress the dialog. [27] [28]
- **Assets:** provide at least two valid screenshots for publication, but prepare six high-resolution portrait screenshots; keep taglines short and no more than 20% of an image. Alt text should be ≤140 characters. [17]
- **Video:** one public/unlisted, embeddable, ad-free YouTube URL with captioned real gameplay. [17]

## 5. Complete visual listing package

### 5.1 Icon directions

Produce three genuinely different, centered, no-wordmark masters for controlled testing:

1. **Tile Grid:** four rounded tiles in a compact square, one subtly offset or highlighted.
2. **Negative-Space Link:** four blocks whose gaps create a quiet interlocking mark.
3. **Four-Block F:** an abstract “F” made from four geometric blocks.

Deliver Apple 1024×1024 source/layered workflow and Google 512×512 32-bit PNG. Do not bake in corner masks or drop shadows for Google; test dark/tinted variants and thumbnail recognition. Apple favors simple, centered, recognizable icons with little/no text; Google dynamically applies masking/shadow. [29] [30]

Use warm off-white/ink neutrals and a FourFold accent, not a competitor-like four-color tile system. Every category state must also have a label, border, pattern, icon, or position cue; never rely on color alone. [1] [29]

### 5.2 Screenshot order and overlay copy

Capture six real-UI portrait masters from the actual build. Prepare Apple device-scaled exports and Google 1080×1920 portrait exports where supported; recheck current device requirements immediately before upload. Apple allows up to 10 screenshots; Google supports up to eight per supported device type and recommends real gameplay early. [17] [18]

| Order | Real UI state | Overlay copy | Proof job |
|---:|---|---|---|
| 1 | Puzzle: readable 4×4 board with four tiles selected | **`16 words. Four groups.`** | Explain the mechanic immediately |
| 2 | Correct group locked with category label and explanation | **`Find the aha.`** | Prove fairness/learnability |
| 3 | Results: solved groups, mistakes, hints, time, streak impact, Share Result | **`A quiet win, clearly explained.`** | Show completion and recovery without pressure |
| 4 | Home Daily Four ready/in-progress/complete card plus streak | **`One daily puzzle. No pressure.`** | Explain the habit loop |
| 5 | Packs with Practice and all five launch themes | **`Practice by theme.`** | Show finite, shipped depth |
| 6 | Stats or Settings with local stats, reminder, sound/haptic controls | **`Your progress stays on this device.`** | Prove local ownership |

Keep copy short, factual, localized, and within safe areas. No splash-only art, fingers, device mockups, fake UI, competitor names, prices, ranking claims, cloud sync, timer, account, leaderboard, or unshipped feature. [17] [18]

### 5.3 Preview-video storyboard

Create one portrait **20–24 second** gameplay-first master with captions that communicate while muted:

| Time | Footage | Caption |
|---|---|---|
| 0–2s | Real board/poster frame | `16 words. Four groups.` |
| 2–7s | Select four words, show immediate response | `Spot the pattern.` |
| 7–11s | Submit; category and explanation appear | `Every group has an explanation.` |
| 11–14s | Gentle wrong guess recovery or optional hint | `A hint is a nudge.` |
| 14–19s | Finish remaining groups and Results | `A quiet win, clearly explained.` |
| 19–24s | Home Daily Four, local streak, Share Result entry | `Daily Four. Practice by theme.` |

Keep at least 80% representative UI/gameplay for Google, put core gameplay within the first 10 seconds, and use only app footage. Apple previews are 15–30 seconds and ≤500 MB; Google requires an ad-free, public/unlisted, embeddable YouTube URL. Validate codec, orientation, poster frame, captions, and device-size delivery. [17] [18]

### 5.4 Share-result asset

**MVP:** text-only, spoiler-safe native share sheet; no image-card system required.

```text
FourFold • Daily Four • 4/4 groups • 1 mistake • 0 hints • 03:42 • streak 7

Can you solve today’s four?
```

Populate real values and omit unavailable fields. Use iOS Activity View and Android Sharesheet with `text/plain`; do not imply accounts, multiplayer, referral tracking, leaderboards, or online sync. If a future release adds a locally generated image card, use a warm neutral background, FourFold mark, date/status, four numbered result rows, mistakes, hints, time, and streak—never the category answers. [31] [2]

### 5.5 Localization notes

- Launch English with all UI strings, puzzle words, category explanations, pack names/descriptions, overlays, video captions, share text, reminder copy, support, Privacy Policy, and Terms externalized.
- Add a second locale only after search/conversion/review evidence; localize the puzzle corpus, not only metadata.
- QA long words, category wrapping, larger text, contrast, dark mode, touch targets, text-to-speech labels, date formats, local-date rollover, and reminder copy.
- Movies & TV content requires a rights review for recognizable titles, logos, characters, artwork, quotes, music, and clips. Use generic examples in creative until rights are confirmed. [3] [4] [11]

### 5.6 A/B test sequence

Run one major variable at a time and predeclare metric plus guardrails:

1. **Icon:** Tile Grid vs Negative-Space Link vs Four-Block F.
2. **Screenshot 1:** mechanic-first `16 words. Four groups.` vs calm-first `One quiet puzzle for today.`
3. **First-three sequence:** mechanic → explanation → results vs mechanic → Daily Four → packs.
4. **Video:** strong screenshot-first page vs gameplay preview.
5. **Custom intent:** Daily Four vs Calm/offline vs themed packs, only with matching traffic.
6. **Locale:** English-market copy vs one localized mechanic/mood treatment.

Apple’s PPO supports up to three treatments and recommends confidence before applying a winner; Google recommends one asset at a time and at least a week. Judge conversion alongside crash/support/review quality and beta feedback, not impressions alone. [10] [19]

## 6. Player research synthesis

### 6.1 Recurring cross-game patterns

The reviewed comparator set was **10 representative games/listings**: NYT Connections, Connect Words, Connect The Words, Words: Associations/Words Connections, Red Herring, Associations–Colorwood, Wordscapes, Wordnect, Connect16, and Word Association Match. Store pages and visible reviews are selective and self-selected; none supports population percentages.

**What players repeatedly like:**

- The immediate, understandable **16-to-four mechanic**, followed by an “aha” when a hidden relationship becomes visible. [14] [20] [21]
- A **short daily ritual** and optional continued play/practice; stats and streaks can make improvement visible for some players. [20] [25]
- **Untimed or low-pressure play**, especially when a player can leave and return rather than lose progress. [23] [34]
- Hints, definitions, explanations, and themed content when they preserve agency and clarify the solve. [21] [35]
- Calm sensory presentation—quiet colors, music, sound, or scenic framing—when it does not interfere with readability or play. [34] [36]

**What players repeatedly dislike:**

- **Ads and monetization interruptions**, including frequent interstitials, difficult-to-close ads, ad-gated hints, coins, subscriptions, or paywalls in short puzzle sessions. [32] [33] [34] [35] [36]
- **Ambiguous or overlapping categories:** five plausible words, arbitrary exclusions, red herrings that feel like author-intent guessing, or obscure trivia without enough explanation. [20] [21] [22] [23]
- **Weak or unavailable hints**, especially when help is monetized or does not narrow the puzzle usefully. [32] [33] [35]
- **Repetition and shallow variety:** repeated words, categories, backgrounds, or finite-content ceilings despite large volume claims. [32] [34] [36]
- **Readability and pacing failures:** small text, low contrast, unclear color semantics, transient explanations, auto-advance, freezes, or lost progress. [22] [32] [33] [34]
- **Pressure or guilt:** streaks, timers, lives, forced waits, and competitive layers can motivate some players but alienate others. [20] [25] [36]

### 6.2 Competitor-specific signals (not general player facts)

- **NYT Connections:** makes the canonical 16-to-four, daily, stats, hints, streak, and sharing ecosystem legible; its own guidance says overlap is intentional, while public critiques focus on ambiguity, obscure knowledge, and mistake pressure. This supports FourFold’s explanation/fairness emphasis but does not prove universal dissatisfaction. [20] [21] [22]
- **Connect Words / Connect The Words:** visible reviews like the core challenge and unlimited attempts, while recurring excerpts complain about ads, repeated content, questionable categories, small text, and limited navigation. Treat this as directional QA input, not a rating-market estimate. [32]
- **Words: Associations / Megarama:** positive excerpts mention thinking, learning, calming distraction, and daily play; negative excerpts emphasize ad friction, coin/hint monetization, obscure vocabulary, freezes, and progress loss. [35]
- **Red Herring:** no-timer play, free daily puzzles, difficulty choices, hints, and definitions are attractive; reviews object to five-or-more plausible fits, obscure references, and paid/ad friction. Android evidence is bundle-level and not safely Red-Herring-specific. [23]
- **Associations–Colorwood:** wood presentation, sounds, and calm framing receive praise; visible complaints include ads, hints that fail or require ads, changing board visibility, transient explanations, freezes, and weak rewards. [33]
- **Wordscapes:** relaxing scenery, music, unlimited tries, teams/events, and long progression are strengths for some; sampled complaints focus on ads, failed rewards, repetition, dictionary friction, and grind. It is a broader word game, not a direct mechanic match. [34] [36]
- **Connect16/Wordnect/Word Association Match:** competitor metadata confirms recognizable language around offline play, local/device progress, no timer, themed packs, category puzzle, and daily routine; this validates messaging vocabulary, not search volume or preference prevalence. [14]

### 6.3 FourFold product priorities

1. **Fairness before volume:** remove a board if a fresh solver can defend two solutions.
2. **Explanation as reward:** show category label and short rationale long enough to read.
3. **Useful, free hints:** reveal one bounded clue/member; never gate help behind ads, payment, or accounts.
4. **No interruption economy:** no ads, purchases, subscriptions, lives, or forced waits in the MVP; only say “no ads” after the final binary/SDK audit.
5. **Readable calm:** high contrast, long-word wrapping, category label plus non-color cue, low-amplitude motion, independent sound/music/haptic controls.
6. **Forgiving habit:** local current/best streak without shame; Practice never changes Daily Four.
7. **Reliable local persistence:** cold start, background/foreground, offline restart, date rollover, exit/resume, and reset must not lose progress.
8. **Honest finite scope:** five packs and Practice, not “infinite” or “new puzzles forever.”

## 7. Concrete MVP-compatible product changes

### Puzzle design and fairness

- Add a pre-release **fairness worksheet** for every board: intended partition, rationale for each group, every tempting alternate grouping, specialist/region-specific knowledge flags, and a fresh-solver outcome.
- Reject boards with a reasonable alternative full partition, a fifth defensible word, obscure knowledge without a clue, or a category label that cannot explain the distinction plainly.
- Curate the first puzzle and Daily Four ramp for common vocabulary; use pack descriptions and category explanations to support unfamiliar but fair terms.
- Keep shuffled unsolved tiles visually stable enough to inspect; solved groups remain locked and labeled. [1] [2]

### Difficulty

- Do not add difficulty modes to the MVP. Instead, tune the bundled corpus into an approachable first puzzle, fair Daily Four range, and varied Practice/pack ordering.
- Treat completion time as optional result information, not a timer or score pressure.
- Use controlled red herrings: one tempting but weaker association can be satisfying; several equally defensible fits are a defect.

### Hints and wrong guesses

- Implement the shipped hint as one useful clue or one group member; record use locally without invalidating completion.
- Keep wrong-guess feedback brief: shake, deduct one mistake, clear selection, preserve solved progress, and return control.
- Hold the solved category/explanation on-screen until the player can choose Home, Practice, or Share Result; do not auto-advance too quickly.

### Ads and monetization stance

- Keep the MVP free of ad SDKs, rewarded ads, IAP, subscriptions, coins, paid hints, and forced waits.
- Do not add “no ads” to metadata until the release-build/dependency audit confirms it. The safer launch claim is the verified no-account/offline/local-progress posture.
- Do not introduce a third-party analytics or attribution SDK solely to imitate a competitor; it would change privacy disclosures and product scope. [10]

### UI/readability

- Maintain 4×4 readability at default and larger text sizes; wrap/scale long words without shrinking them into illegibility.
- Pair color with category text, border, pattern, icon, or position. Check contrast in light/dark modes and on older devices.
- Use generous touch targets, visible selected state, disabled Submit until four tiles are selected, and clear remaining-mistake state.
- Test loading/error recovery: missing/invalid puzzle returns to Home/Packs, never a blank or looping screen. [2]

### Sound/haptics

- Keep soft selection/correct/wrong/completion cues, with independent sound effects, music, and haptics toggles.
- Wrong feedback must not feel punitive; avoid loud alarms or persistent music.
- Test muted play, interruption by calls/other media, Bluetooth, reduced motion, and accessibility settings.

### Notifications

- Offer one optional local Daily Four reminder with player-selected time and neutral copy: **“Your Daily Four is ready.”**
- Explain local notification value before requesting permission; request from Settings after enable, never on splash, Welcome, first puzzle, or after denial. [1] [2]
- Never send catch-up spam or imply the streak is time-critical.

### Sharing

- Ship text-only, spoiler-safe native sharing. Include groups solved, mistakes, hints, time, and streak only when available.
- Cancel returns to Results; no account, profile, leaderboard, or referral tracking.
- Treat OS share recipients and browser legal pages as outside FourFold’s local storage boundary. [1] [2]

### Onboarding

- Keep Welcome to one sentence plus the actual 16-word/four-group explanation; offer **Start Playing**, **How It Works**, and visible **Skip**.
- Keep the interactive tutorial under one minute and demonstrate select, submit, wrong guess, hint, and correct explanation. No login or permission prompt.
- Begin a real bundled puzzle immediately after onboarding; after completion return to Home and point to Daily Four, Practice, Packs, Stats, and Settings. [1] [2]

### Later work (clearly outside MVP)

Only consider after quality and conversion evidence: image share cards, deep links/Universal Links/App Links, additional custom pages/locales, opt-in diagnostics/analytics, explicit difficulty modes, larger content drops, or remote content. Each would require a new privacy, product, and QA decision; none should appear in launch copy.

## 8. Pre-launch review and QA checklist

### Product and content

- [ ] First-time player understands the mechanic in ≤1 minute without a permission prompt.
- [ ] Every launch board has one intended partition and documented rationale.
- [ ] Fresh solvers found no equally defensible alternate partition or fifth-word collision.
- [ ] Category label/explanation is factually correct, readable, and persistent long enough.
- [ ] First puzzle, Daily Four, Practice, and all five packs load from the bundle offline.
- [ ] Practice never changes Daily Four completion or streak.
- [ ] Daily date key is deterministic; date change does not duplicate or crash.
- [ ] Mistake, hint, shuffle, resume, game-over, and completion states match the flows. [2]

### Reliability and accessibility

- [ ] Cold launch, background/foreground, app kill/restart, offline restart, exit/resume, reset, and share cancellation tested.
- [ ] Missing/invalid content returns to recoverable Home/Packs state.
- [ ] Long words, larger text, contrast, dark mode if supported, reduced motion, screen reader labels, and touch targets tested.
- [ ] Sound, music, and haptics toggles persist independently; muted gameplay remains understandable.
- [ ] Battery, memory, and responsiveness checked on representative older devices.

### Privacy, SDK, and policy

- [ ] Release build and every dependency audited for network calls, identifiers, crash/analytics/ads/attribution, authentication, remote config, and diagnostics.
- [ ] App Privacy and Google Data safety completed from the final build, including third-party SDK behavior. [10]
- [ ] Public HTTPS Privacy Policy, Terms, Support URL, contact route, and version/build context work.
- [ ] Store claim “offline/on-device/no account/no ads” is used only where verified.
- [ ] Apple age rating and Google target audience/IARC answers match actual content; child targeting is not used merely for reach. [26]
- [ ] Movies & TV words, titles, logos, artwork, quotes, characters, and music have rights clearance or are replaced with generic examples. [3] [4]
- [ ] Metadata contains no competitor names, rankings, fake testimonials, price claims, unsupported efficacy, or unshipped features.

### Store assets

- [ ] Name/subtitle/title/short description/keyword bytes and characters recorded per locale.
- [ ] Apple keyword validator behavior checked against the current locale because public documentation differs.
- [ ] Six screenshots show real UI, correct states, localized overlays, and no fake/cloud/timer/account UI.
- [ ] Screenshot dimensions/device matrix rechecked immediately before upload.
- [ ] Preview is 15–30 seconds for Apple, ≤500 MB, app-only; Google video is public/unlisted, embeddable, ad-free, captioned, and gameplay-first. [17] [18]
- [ ] Google feature graphic and 512×512 icon pass the current validator; no baked-in mask/shadow.
- [ ] Poster frame and muted captions communicate the mechanic without audio.

### Reviews and notifications

- [ ] Native rating API only after several meaningful completions including a Daily Four.
- [ ] No custom prompt, sentiment gate, reward, five-star request, or prompt after failure/denial/onboarding. [24] [27]
- [ ] Local reminder is opt-in, contextual, editable, and neutral.
- [ ] Support/review response playbook tags fairness, repetition, hints, readability, crashes, offline, reminders, sharing, and sound/haptics.

## 9. Measurement plan and experiment backlog

### What can be measured without server analytics

| Funnel | Metrics | Decision use | Caveat |
|---|---|---|---|
| Discoverability | Impressions, search/browse source, custom-page/listing impressions | Is the message surfaced? | No complete ranking formula; impressions are not success. [5] [6] |
| Consideration | Product-page/listing views, video engagement where available | Do assets earn attention? | Store-level aggregate only. |
| Acquisition | First-time downloads, conversion, attributed campaign traffic, UTM/source/listing/country/language | Which page/audience converts? | Apple custom pages need enough first-time downloads; Google dimensions are store reports. [8] [9] [10] |
| Quality | Ratings, review themes, support contacts, crash reports | Does experience match promise? | Review corpus is self-selected; tag themes, do not calculate prevalence. |
| Early experience | Closed-beta completion observations, fairness reports, tutorial comprehension, offline/resume checks | What to fix before scale? | Qualitative evidence, not representative population research. |
| Creative | Watch-through, saves/comments, store visits, creator link traffic | Which hook merits another pilot? | Views alone do not establish installs or retention. |

Track each experiment in a sheet: hypothesis, audience, locale, exact treatment, platform, start/end, primary metric, guardrails, sample/eligibility, decision, and follow-up. Because FourFold has no server analytics, do not invent D1/D7/D28 cohorts; use beta feedback, local QA, support, store reviews, and store conversion.

### Experiment backlog

| ID | Hypothesis | Variable | Primary read | Guardrail/decision |
|---|---|---|---|---|
| E1 | A clearer mark improves recognition | Three icon concepts | Store conversion | Keep only with no review/support regression |
| E2 | Mechanic-first wins cold traffic | Screenshot 1 mechanic vs calm | Conversion | Retain factual winner |
| E3 | Explanation increases trust | First three: mechanic → explanation → result vs mechanic → Daily Four → packs | Conversion plus fairness comments | Prefer the sequence reducing “what is this/why wrong?” |
| E4 | Video adds understanding | Preview vs screenshot-first | Conversion | Do not assume video wins; test it |
| E5 | Calm/offline attracts distinct intent | Custom page/listing copy and first asset | Page/listing conversion | Use only for matching traffic and verified claims |
| E6 | Daily framing improves daily-intent traffic | Daily Four custom destination vs default | Conversion | Keep as targeted acquisition, not default-page proof |
| E7 | Pack creative expands qualified traffic | Themed-pack destination | Conversion/comments | Do not infer pack demand from views alone |
| E8 | Recovery/reveal creative earns better engagement | Connection reveal vs wrong-guess recovery vs quiet reset | Watch-through, comments, store visits | Recut only repeatable hooks |
| E9 | Localized language improves relevance | One market-specific locale treatment | Conversion/review language | Add one locale at a time |
| E10 | Fairness improvements change review quality | Content fixes before/after release | Fairness/repetition/support tags | Ship fixes before new feature claims |

## 10. 30/60/90-day execution plan

### Days 0–30: scope lock, fairness, and store readiness

- Freeze the mechanic-first/calming promise and remove competitor-adjacent claims.
- Audit every puzzle for alternate solutions, obscure knowledge, fifth-word fits, factual rights, and explanation quality.
- Test onboarding, first puzzle, hint, wrong guess, shuffle, Daily Four date rollover, Practice isolation, local persistence, reset, offline restart, share cancellation, long words, contrast, and larger text.
- Audit release build/dependency tree for network calls, identifiers, ads, analytics, crash reporting, attribution, auth, and remote config.
- Draft final Apple/Google metadata, privacy/support/legal pages, age/content answers, keyword hypothesis sheet, and six screenshot wireframes.
- Produce three icons, six screenshot captures, feature graphic master, and 20–24-second video master from the actual build.
- Recruit 15–30 closed-beta players and ask structured questions about fairness, ambiguity, hint usefulness, calmness, notification timing, sharing, readability, sound/haptics, and crashes.

**Exit gate:** a new player can understand and complete a bundled puzzle without login, network, or permission prompt; no store claim contradicts the build.

### Days 31–60: submit, launch, and learn

- Fix beta defects before expanding creative.
- Complete final SDK/privacy/rights/age audits and recheck platform limits/dimensions immediately before submission.
- Launch default listing plus only the Apple Daily Four/calm/offline/themed pages and Google Daily Four/packs listings that have real matching traffic.
- Publish one gameplay preview, creator/community pilot, and permission-based support channel; no review incentives.
- Monitor store conversion, crashes, support questions, Daily Four completion feedback, and review themes.
- Do not change several store variables in the first days unless fixing factual/policy errors.
- Start E1 icon test, then E2 screenshot 1, then E3 first-three sequence; wait for Apple confidence or Google’s week-plus guidance. [10] [19]

**Exit gate:** one default creative family is directionally credible on conversion and does not create fairness, readability, crash, privacy, or expectation-gap complaints.

### Days 61–90: optimize and decide what not to build

- Run E4 video versus screenshot-first and one matching custom-page/listing test.
- Tag review/support language into recurring versus isolated themes; prioritize puzzle fairness, repetition, readability, hint usefulness, resume/offline, notifications, sharing, and sound/haptics.
- Expand only the strongest campaign intent or one locale after localized UI/corpus QA.
- Decide whether image share cards, deep links, additional pages, opt-in diagnostics, or new content justify their privacy and engineering cost; keep all as later work until evidence supports them.
- Refresh metadata/assets only when the product or validated player language changes.
- Publish a 90-day decision memo with exact treatments, metrics, caveats, unresolved risks, and the next single experiment.

## References

[1]: https://github.com/codewithkin/fourfold/blob/main/plans/user-stories.md "FourFold MVP user stories"
[2]: https://github.com/codewithkin/fourfold/blob/main/plans/user-flows.md "FourFold MVP user flows"
[3]: https://developer.apple.com/app-store/review/guidelines/ "Apple App Review Guidelines"
[4]: https://support.google.com/googleplay/android-developer/answer/13393723?hl=en "Google Play store listing best practices"
[5]: https://developer.apple.com/app-store/search/ "Apple App Store search"
[6]: https://support.google.com/googleplay/android-developer/answer/4448378?hl=en "Google Play search discovery"
[7]: https://developer.apple.com/help/app-store-connect/reference/app-information/platform-version-information/ "App Store Connect platform version information"
[8]: https://developer.apple.com/help/app-store-connect/create-custom-product-pages/configure-multiple-product-page-versions/ "Apple custom product pages"
[9]: https://support.google.com/googleplay/android-developer/answer/9867158?hl=en "Google Play custom store listings"
[10]: https://support.google.com/googleplay/android-developer/answer/9859173?hl=en "Google Play store listing performance reports"
[11]: https://developer.apple.com/help/app-store-connect/manage-app-information/localize-app-information/ "Apple localized app information"
[12]: https://developer.apple.com/app-store/categories/ "Apple App Store categories"
[13]: https://ads.apple.com/app-store/best-practices/keywords "Apple Ads keyword best practices"
[14]: https://apps.apple.com/is/app/connect16-daily-word-puzzle/id6759406712?platform=ipad "Connect16 listing language benchmark"
[15]: https://apps.apple.com/ai/app/connect-word-group-puzzle/id6799974657 "Connect: Word Group Puzzle listing"
[16]: https://play.google.com/store/apps/details?id=com.ham.game.connections&hl=en_US "Connections: Daily Word Puzzle listing"
[17]: https://support.google.com/googleplay/android-developer/answer/9866151?hl=en "Google Play preview assets"
[18]: https://developer.apple.com/help/app-store-connect/reference/app-information/app-preview-specifications/ "Apple app preview specifications"
[19]: https://developer.apple.com/app-store/product-page-optimization/ "Apple Product Page Optimization"
[20]: https://help.nytimes.com/360011158491-New-York-Times-Games/28525912587924-Connections "NYT Connections Help Center"
[21]: https://www.nytimes.com/2023/11/06/crosswords/connections-tips-and-tricks.html "How to Line Up a Great Connections Solve"
[22]: https://www.raphkoster.com/2023/09/02/why-nyts-connections-makes-you-feel-bad/ "Why NYT Connections makes you feel bad"
[23]: https://apps.apple.com/us/app/red-herring/id663596265?see-all=reviews&platform=iphone "Red Herring player reviews"
[24]: https://developer.apple.com/design/human-interface-guidelines/ratings-and-reviews "Apple Human Interface Guidelines: Ratings and reviews"
[25]: https://developer.apple.com/app-store/ratings-and-reviews/ "Apple ratings and reviews"
[26]: https://support.google.com/googleplay/android-developer/answer/9867159?hl=en "Google Play target audience"
[27]: https://developer.android.com/guide/playcore/in-app-review "Google Play In-App Review API"
[28]: https://support.google.com/googleplay/android-developer/answer/9898684?hl=en "Google Play ratings, reviews, and installs policy"
[29]: https://developer.apple.com/design/human-interface-guidelines/app-icons "Apple Human Interface Guidelines: App icons"
[30]: https://developer.android.com/distribute/google-play/resources/icon-design-specifications "Google Play icon design specifications"
[31]: https://developer.android.com/develop/ui/compose/sharing/send "Android Sharesheet guidance"
[32]: https://apps.apple.com/us/app/connect-words-puzzle-game/id6476164708?see-all=reviews&platform=iphone "Connect Words player reviews"
[33]: https://apps.apple.com/us/app/associations-colorwood-game/id6749696890?see-all=reviews&platform=iphone "Associations Colorwood player reviews"
[34]: https://apps.apple.com/us/app/wordscapes-word-game/id1207472156?see-all=reviews&platform=iphone "Wordscapes player reviews"
[35]: https://apps.apple.com/us/app/words-connections-word-game/id6465991134?see-all=reviews "Words - Connections player reviews"
[36]: https://play.google.com/store/apps/details?id=com.peoplefun.wordcross&hl=en_US "Wordscapes Google Play listing"
[37]: https://developer.apple.com/app-store/app-privacy-details/ "Apple App Privacy details"
[38]: https://support.google.com/googleplay/android-developer/answer/10787469?hl=en "Google Play Data safety"
