# FourFold MVP Sound Design

## Audio direction
FourFold should feel calm, polished, responsive, and satisfying. Use short sounds with soft transients and avoid loud, childish, or stressful effects. Sound effects are more important than background music for the MVP.

All audio should be optional through Settings, with separate toggles for sound effects, music, and haptics.

## Required MVP sounds

### 1. Tile select
**Trigger:** Player taps an unselected word tile.

**Purpose:** Confirm that the tap registered.

**Feel:** Soft, rounded click with a tiny warm pluck. Very short and quiet.

**Asset:** `tile-select.mp3`

### 2. Button tap
**Trigger:** Player taps a standard button such as Play, Packs, Stats, Settings, Shuffle, or Back.

**Purpose:** Provide consistent navigation feedback.

**Feel:** Clean, cushioned, neutral click. Quieter than a success sound.

**Asset:** `button-tap.mp3`

### 3. Tile deselect
**Trigger:** Player taps a selected tile to remove it from the guess.

**Purpose:** Confirm that the selection was removed.

**Feel:** Use the tile-select sound at lower volume or a softer reversed variation. A separate asset is optional for MVP.

### 4. Correct group
**Trigger:** Player submits four words that form a valid category.

**Purpose:** Reward progress and confirm the answer.

**Feel:** Two or three warm ascending notes with a subtle sparkle. Positive but understated.

**Asset:** `group-correct.mp3`

### 5. Wrong guess
**Trigger:** Player submits an incorrect group.

**Purpose:** Communicate “try again” without making the player feel punished.

**Feel:** Muted low wobble or cushioned tick. Never use an alarm, harsh buzzer, or embarrassing fail sound.

**Asset:** `guess-wrong.mp3`

### 6. Hint reveal
**Trigger:** Player uses a hint.

**Purpose:** Make the help feel like a discovery rather than a penalty.

**Feel:** Short airy shimmer followed by one warm note.

**Asset:** `hint-reveal.mp3`

### 7. Shuffle
**Trigger:** Player shuffles the unsolved word tiles.

**Purpose:** Make the board rearrangement feel intentional and responsive.

**Feel:** Very short soft whoosh or light movement sound. This can be created later; it is not essential for the first prototype.

### 8. Puzzle complete
**Trigger:** Player solves all four groups.

**Purpose:** Mark the main reward moment and reinforce completion.

**Feel:** Three warm ascending notes with a gentle bright chime. Celebratory but calm.

**Asset:** `puzzle-complete.mp3`

### 9. Daily puzzle ready
**Trigger:** Player opens Home and a new Daily Four is available.

**Purpose:** Draw attention to the daily challenge without creating pressure.

**Feel:** One soft, welcoming two-note cue. Optional for MVP; the visual Daily Four card is sufficient initially.

## Optional later sounds
- Streak milestone
- Daily reminder notification
- Pack unlocked
- New difficulty unlocked
- Game-over or no-mistakes-left feedback
- Share-result confirmation
- Background ambient music loop

## Implementation guidance
- Keep most UI sounds under one second.
- Keep the completion sound under two seconds.
- Play feedback immediately after the action.
- Avoid overlapping sounds when multiple tiles animate together.
- Keep sound effects comfortably audible at low device volume.
- Do not require music for the game to feel complete.
- Pair important sounds with visual feedback and optional haptics.
- Save the player’s sound, music, and haptic preferences locally.

## MVP priority
1. Tile select
2. Button tap
3. Correct group
4. Wrong guess
5. Hint reveal
6. Puzzle complete
7. Shuffle
8. Daily puzzle ready

The first six sounds are enough for a polished MVP. Shuffle and Daily puzzle ready can be added after the core puzzle loop feels good.
