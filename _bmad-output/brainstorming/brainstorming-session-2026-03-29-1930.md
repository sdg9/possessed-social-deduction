---
stepsCompleted: [1, 2, 3]
inputDocuments: []
session_topic: 'Station Fall - mobile social deduction game with corrupted-UI infection mechanic'
session_goals: 'Wide-open exploration of day-one design - stress test, expand, find blind spots'
selected_approach: 'ai-recommended'
techniques_used: ['reverse-brainstorming', 'cross-pollination', 'morphological-analysis']
ideas_generated: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35]
context_file: ''
current_phase: 'endgame-exploration'
---

# Brainstorming Session Results

**Facilitator:** Steven
**Date:** 2026-03-29 / 2026-03-30

## Session Overview

**Topic:** Station Fall — a digital social deduction game (phone-based, played in-person) featuring the "Nudge" mechanic where dormant infected players see corrupted action labels, creating genuine confusion during accusations.

**Goals:** Wide-open exploration of a day-one design. Stress test mechanics, expand the design space, find blind spots, and generate novel ideas across all dimensions of the game.

**Player Count:** 6-8 (designed with conviction, not hedging for 4)

### Session Setup

- Existing detailed design document provided as context (see: original-design-doc.md in repo root)
- References: Panic Station, Secret Hitler, Blood on the Clocktower, The Thing, Slay the Spire, Twilight Imperium, Dead of Winter
- Key innovation: Dormant infected players unknowingly sabotage through corrupted UI ("Nudge" mechanic)
- Dropped: Async play, gas cans, memory fragments as starting items, sequential captain-picks-team draft
- Platform: In-person with phones. App handles hidden state, table handles social deduction. Not a phone game you play together — a tabletop game that uses phones for what cards/moderator can't do.

## Technique Selection

**Approach:** AI-Recommended Techniques
**Analysis Context:** Day-one game design needing both creative expansion and critical examination

**Recommended Techniques:**

1. **Reverse Brainstorming:** Stress test the foundation
2. **Cross-Pollination:** Expand the design space from unexpected domains
3. **Morphological Analysis:** Map the design space systematically

**Note:** Session naturally evolved from structured reverse brainstorming into collaborative design exploration as ideas built on each other. Techniques blended organically.

---

## Ideas Generated

### The Proximity Dilemma (Ideas #1-3)

**[Mechanics #1]: The Avoidance Death Spiral**
_Concept:_ If infection spreads through proximity/trading, rational players scatter. Everyone picks different rooms, avoids interaction, and social deduction collapses. The game becomes solitaire with a vote at the end.
_Novelty:_ This isn't an edge case — it's the default rational strategy if we don't solve it. The game is broken at its core without compelling reasons to be near other players.
_Status:_ PROBLEM IDENTIFIED — solved by ideas #2, #3, and room design.

**[Mechanics #2]: The Information-Through-Proximity Engine**
_Concept:_ Being in a room with someone gives you a private hint about them — but only you see it, can't prove it, and might be lying about it. Proximity is the ONLY way to gather intel, so avoiding people means flying blind.
_Novelty:_ Flips infection risk from "cost to avoid" into "price of admission for the game's most valuable resource: information."
_Status:_ CORE MECHANIC — retained.

**[Mechanics #3]: Hidden Objectives as Doubt Multiplier**
_Concept:_ Every player has a secret personal objective. Selfish-looking behavior could be infection OR objective-chasing. Room hints might reveal fragments of someone's objective — which looks suspicious whether they're infected or not.
_Novelty:_ Three-layer doubt stack: Are they infected? Chasing a personal goal? Lying about what they learned about ME?
_Status:_ CORE MECHANIC — retained, refined in ideas #4-5.

### Hidden Objectives Design (Ideas #4-6)

**[Mechanics #4]: The Alignment Spectrum for Hidden Objectives**
_Concept:_ Objectives exist on a spectrum from cooperative-but-unusual to mildly selfish to outright suspicious-looking. Every player has SOME reason to act weird. The infected blend in because everyone's acting a little off.
_Novelty:_ Not about separate win conditions — about creating universal behavioral noise so deviation from "perfect play" is expected.
_Rough ratio:_ ~30% innocent but force odd behavior, ~40% mildly selfish, ~30% look outright suspicious (but are achievable by clean players).
_Status:_ RETAINED — spectrum approach confirmed.

**[Mechanics #5]: Objectives That Gate Your Win**
_Concept:_ Your personal objective must be completed for YOU to count in the crew victory. The station gets repaired, but if you didn't achieve your objective, you personally lose even though the crew "won." Dead of Winter model.
_Novelty:_ Creates genuine prisoner's dilemma — need crew success AND personal goal. Can't sacrifice either. Clean players genuinely MUST act selfishly sometimes, giving infected perfect cover.
_Status:_ CORE MECHANIC — this is what makes objectives compelling rather than ignorable.

**[Mechanics #6]: Drip-Feed Information Discovery (Replaces Memory Fragments)**
_Concept:_ Kill Memory Fragments as a starting mechanic. Hints about other players are earned through play by being in rooms together, one piece at a time. Turn 1 you know your role and your objective. That's it. Everything else you discover by showing up.
_Novelty:_ The information economy IS the game loop. No front-loaded info dump. The game teaches itself as you play. Cognitive load at game start is minimal: your role, your objective, pick a room.
_Status:_ CORE DESIGN DECISION — starting hand is just role + objective.

### Room Activity Design (Ideas #7-9)

**[Mechanics #7]: Room Activity Models — The Core Question**
_Concept:_ Explored five models for what players actually DO in rooms:
- Model A: Binary choice (too simple, feels like voting)
- Model B: Multiple choice menu (form-filling, not engaging)
- Model C: Collaborative mini-game (kills async — but async is now dropped, so revisitable)
- Model D: Contribution spectrum (effort level 1-5, saboteur drags numbers down, ambiguity baked in)
- Model E: Async micro-decisions (2-3 sequential small choices)
_Status:_ Models D and E selected as the interesting design space.

**[Mechanics #8]: The App-Table Split**
_Concept:_ The phone is your private decision space. The table is your public performance space. You make secret choices on your screen while arguing, deflecting, and reading people face-to-face. The app is the engine, the players are the game.
_Novelty:_ Not a phone game you play together — a tabletop social deduction game that uses phones to do what cards and a moderator can't.
_Status:_ CORE DESIGN PHILOSOPHY.

**[Mechanics #9]: Layered Room Actions**
_Concept:_ Each room has one PRIMARY action (effort commitment — how much do you contribute?) plus one SECONDARY choice (directional decision — how do you contribute?). Primary determines magnitude, secondary determines direction. A saboteur might commit high effort but route it wrong.
_Novelty:_ Two axes of hidden information per room visit. "Someone tanked the repair" becomes "did someone not try hard enough OR try hard but make bad calls?" — very different accusations.
_Example:_ Engineering — Primary: commit 1-5 effort. Secondary: "Route power to shields or engines?" Result: partial outcome with ambiguous blame.
_Status:_ STRONG CANDIDATE — needs validation against specific room designs.

### Ship Systems & Cross-Room Interaction (Ideas #10-14)

**[Mechanics #10]: Civilians from Cryosleep**
_Concept:_ Nobody is specialized. All players are civilians woken early from cryosleep by an emergency. No one "belongs" in any room. Explains varied skill levels, justifies why the alien influence goes unnoticed — nobody knows what "normal" looks like.
_Novelty:_ Removes class-based excuses and replaces with universal plausible deniability. Also supports the roguelike reward system — memories returning from cryosleep.
_Status:_ CORE THEME/SETTING.

**[Mechanics #11]: Cross-Room Events as the Core Turn**
_Concept:_ Each turn is a ship-wide EVENT requiring coordinated response across multiple rooms simultaneously. Navigator calls out threats, Engineering responds, Weapons decides to shoot or brace, etc. Players make choices on phones while shouting across the table. Event resolves based on the COMBINATION of all rooms' responses.
_Novelty:_ Rooms aren't isolated puzzles — they're interconnected systems. Sabotage cascades across rooms. Figuring out WHERE failure originated is a multi-room deduction problem.
_Status:_ CORE MECHANIC.

**[Mechanics #12]: Action Phase / Debrief Phase Split**
_Concept:_ Each turn has two distinct beats:
1. **Stations** (30s-2min) — Event fires, players respond from rooms, cross-room communication in real-time
2. **Mess Hall** (open-ended) — Everyone debriefs. Results revealed. Private hints delivered. Accusations, discussion, voting.
_Novelty:_ Clean separation: Stations = the GAME happens. Mess Hall = the SOCIAL DEDUCTION happens. App drives Stations, players drive Mess Hall.
_Status:_ CORE STRUCTURE.

**[Mechanics #13]: Comms Room Reimagined — The Scanner**
_Concept:_ Comms isn't about relaying between rooms (everyone's at the same table, can't play telephone). Instead, Comms is the intelligence room — intercept signals, scan players, learn secrets nobody else has. You go there to learn, not to talk.
_Novelty:_ Comms player gets private intel on their phone, chooses what to share or withhold at debrief.
_Status:_ RETAINED — original relay concept killed because it doesn't work in-person.

**Room Ecosystem (DO/GET model):**

| Room | What You DO (during event) | What You GET (private, post-event) |
|------|------|------|
| Navigation | Set course / dodge threats | See next turn's event preview |
| Engineering | Allocate power / repair systems | Hint about a roommate's objective |
| Weapons/Shields | Shoot or defend | See result accuracy (was damage real or sabotaged?) |
| Comms/Scan | Scan a player OR intercept signal | Private intel on one player's infection status (fuzzy) |
| Security | Watch a room's feed | See what choices were made in another room (not by who) |
| Med Bay | Run diagnostics | Blood test equivalent — limited uses |

**[Mechanics #14]: Event Deck with Escalation**
_Concept:_ App draws from an event deck with severity tiers that escalate as the game progresses. Early: minor, 1-2 rooms. Mid: multi-room coordination. Late: catastrophic cascades where every room matters.
_Novelty:_ Natural dramatic arc without scripting. Early turns forgive (learning space), late turns punish (rewards deduction). Early turns also give "free" turns for intel rooms without group cost.
_Status:_ RETAINED — starting as deck, future potential for dynamic/reactive events.

| Turn | Severity | Rooms Involved |
|------|----------|----------------|
| 1-2 | Minor | 1-2 rooms |
| 3-4 | Moderate | 2-3 rooms |
| 5-6 | Major | 3-4 rooms |
| 7+ | Critical | All rooms |

### Draft & Turn Order (Ideas #15-16)

**[Mechanics #15]: Room-Based Turn Order Priority (SUPERSEDED by #22)**
_Concept:_ Original idea — room choice this turn determines draft position next turn. Low-power solo rooms grant early picks, high-power rooms push you later. Constant trade between power-now and choice-later.
_Status:_ SUPERSEDED by MOTHER assignment system (#22). Core insight retained: room choice should have draft consequences.

**[Mechanics #16]: Everyone Participates Every Turn**
_Concept:_ No team assembly by a leader. Every player picks a room, every player acts, every player gets info. Nobody sits out. Leadership is emergent based on information and trust, not assigned.
_Novelty:_ Solves the Secret Hitler "never picked for the team" feel-bad. Infected can't be locked out of play. Clean players always have agency.
_Status:_ CORE DESIGN DECISION.

### The Brig System (Ideas #17-20)

**[Mechanics #17]: The Brig — Containment, Not Elimination**
_Concept:_ Players vote to put someone in the Brig. Brigged player isn't dead — they're contained. Assigned to a room by the group, actions visible to a designated guard, can still contribute but can't sabotage secretly. Can argue for release at each debrief.
_Novelty:_ Doesn't kill social interaction — transforms it. Brigged player is still talking, pleading, potentially useful. Cost: you weaken a crew member AND tie up a guard. Wrongly brigging a clean player is devastating.
_Brig capacity:_ Up to 2 players.
_Release:_ By vote at debrief.
_Status:_ CORE MECHANIC.

**[Mechanics #18]: Player Count Sweet Spot — 6-8**
_Concept:_ Stop designing for 4. Build the best possible experience for 6-8 players. Every system tuned for that range. No watered-down small-player variant.
_Novelty:_ Most social deduction games hedge with wide player counts and suffer. Confident player count means every seat is essential and every system is tight.
_Status:_ CORE DESIGN DECISION.

**[Mechanics #19]: Brig Activities — Contained But Not Idle**
_Concept:_ Brigged players have a limited action menu each turn:
- **Cooperative:** Advise (recommend room priorities), Remote assist (small bonus to one room, guard sees which)
- **Subversive:** Tamper (attempt sabotage, guard may catch you), Plea (formal release request to all players)
- **Information:** Eavesdrop (partial info about one room you're not in)
_Guard benefit:_ Gets a hint about brigged player each turn. Multiple turns = accumulated certainty.
_Status:_ RETAINED — needs further design.

**[Mechanics #20]: Guard Rotation**
_Concept:_ Guard duty rotates rather than being dedicated. Combined with the "can't repeat your room" rule, this happens naturally.
_Status:_ RETAINED — fits with room rotation rule.

### Room Rotation & MOTHER (Ideas #21-22)

**[Mechanics #21]: Room Rotation — Can't Repeat**
_Concept:_ You can't pick the same room you were in last turn. Forces movement, prevents camping, naturally rotates guard duty. Creates deduction signal — where you go next is always a real choice.
_Novelty:_ Simple rule, massive design impact.
_Status:_ CORE RULE. (May soften to "strong preference weighting" rather than hard rule — TBD.)

**[Mechanics #22]: Ship AI as Draft Arbiter — "MOTHER"**
_Concept:_ Players submit ranked room preferences simultaneously. The ship's AI ("MOTHER") assigns rooms based on priorities, weighting, and its own logic. Players don't fully understand MOTHER's algorithm.
_Novelty:_ Three wins:
1. **Speed** — simultaneous submission, 15 seconds instead of 2-minute sequential draft
2. **Mystery layer** — assignment system itself becomes suspicious, opening game modes where MOTHER is the threat
3. **Mechanical design space** — infected could have priority override, players who got 3rd choice get weight next turn, abilities can manipulate assignments

**Game Mode Variations enabled by MOTHER:**

| Mode | What's Actually Happening |
|------|--------------------------|
| Classic | Infected player(s) + dormant, MOTHER is neutral |
| Rogue AI | All players are clean, MOTHER is actively sabotaging assignments |
| Puppet Master | MOTHER is controlled by an infected player remotely |
| Chaos | Random — players never know which mode they're in |

_Status:_ CORE MECHANIC — replaces sequential draft entirely.

### Roguelike Reward System (Ideas #23-25)

**[Mechanics #23]: Post-Event Rewards — The Roguelike Layer**
_Concept:_ After each event, players gain something based on where they were and what happened. Not just information — tangible items and abilities that change capabilities. Over 6-8 turns, each player builds a unique small kit. Thematically: cryosleep memories returning, items found in rooms.
_Novelty:_ Transforms "same actions every turn" into evolving capabilities. Creates asymmetry — I know what I have, you don't. Infected can acquire sabotage tools that feel earned.

**Reward types:**
- **Abilities (memories):** "You remember medical training" → partial scan from any room once. "You recall override codes" → force your first room choice next turn.
- **Items (found in rooms):** Repair kit, scanner fragment, comms bypass.
- **Status effects:** "Radiation exposure" → fuzzy hints next turn. "Strange residue" → others get a hint something's off about you even if clean.

**Passive vs. Active split for cognitive load:**

| Type | Examples | Mental Load |
|------|----------|-------------|
| Passive | Better hints, resist one Nudge corruption | Zero — app handles it |
| Active single-use | Scanner, comms bypass, priority override | Low — one decision, gone |
| Active persistent | Reusable scan ability | Medium — rare, ~1 per game |

_Status:_ CORE MECHANIC — ~1 reward per turn, half passive, manageable on phone.

**[Mechanics #24]: Fully Hidden Inventory**
_Concept:_ Everything acquired is completely private. No public hand size, no visible abilities. You can bluff about capabilities: "I can prove you're infected" — can they? Or faking a scanner to see your reaction? The app tracks everything silently.
_Novelty:_ Most item games have visible hand sizes. Hiding everything means bluffing about CAPABILITIES, not just intentions.
_Status:_ CORE DESIGN DECISION.

**[Mechanics #25]: Brig Rewards — MOTHER's Private Channel**
_Concept:_ Brigged players don't find physical items — they're locked up. But MOTHER has a direct line to them. Each turn in the Brig, MOTHER feeds you: memory fragments, cryptic ship hints, suspicions about other players. Is MOTHER helping? Manipulating? Running her own agenda?
_Novelty:_ Being brigged becomes its own experience. You come OUT knowing things nobody else does — making your release both desired and dangerous. "What did MOTHER tell you in there?"
_Status:_ RETAINED — plays beautifully into Rogue AI mode.

---

## Current Gameplay Loop (Working Model)

**One Turn of Station Fall (~5-8 minutes):**

1. **EVENT ALERT** (~15s) — App announces event to all. Severity visible. Table reacts.
2. **ROOM DRAFT** (~15-30s) — All players submit ranked room preferences simultaneously. MOTHER assigns rooms. Can't repeat last room.
3. **STATIONS** (~1-2min) — All rooms act simultaneously on phones. Table talk represents ship comms. Cross-room callouts. Effort + direction choices. Nudge corruption active for infected.
4. **RESULTS** (~30s) — Event outcome shown to all (group result, not individual contributions). Private hints about roommates delivered to phones.
5. **MESS HALL DEBRIEF** (~3-5min) — Open discussion. Share/lie about actions and hints. Brig vote. Release vote. Reward/item discovery.
6. **CYCLE** — New draft weights calculated. Next event drawn (escalating). Repeat.

**Full game: ~6-8 turns. 30-60 minutes total.**

---

## Evolution from Original Design Doc

| Element | Original Doc | Current Direction |
|---------|-------------|-------------------|
| Platform | Async mobile game | In-person with phones, app handles hidden state |
| Player count | 4-7 | 6-8, designed with conviction |
| Draft | Sequential captain picks team | Simultaneous ranked preferences, MOTHER assigns |
| Rooms | Isolated missions with card play | Interconnected ship systems responding to events |
| Actions | Secret card from hand | Effort commitment + directional choice on phone |
| Information start | Memory fragments (3 cards, 1 false) | Nothing — drip-fed through room proximity |
| Items | Gas cans for defense/win condition | Roguelike rewards — items, abilities, passives |
| Eliminated players | Ghost Protocol | Brig — contained but active, MOTHER communion |
| Turn structure | 9-step round | 5-step: Event, Draft, Stations, Results, Debrief |
| Threat model | Always infected player(s) | Variable — infected, rogue AI, puppet master, unknown |
| Win condition | 5 missions / quarantine all infected | Binary: ship arrives safely or doesn't (see endgame) |
| AI system | None | MOTHER — draft arbiter, info source, potential antagonist |
| Setting | Damaged space station | Colony ship — Earth is dying, heading to new planet |
| Self-destruct | Not present | Available but extreme — humanity goes extinct |

---

## Open Design Questions (Queued for Exploration)

1. **Endgame design** — How does a game end? What are win/lose conditions for crew and infected across all modes? (CURRENTLY EXPLORING)
2. **Nudge mechanic refinement** — How does Nudge work against the new effort+direction room model? Most impactful in dormant/rogue AI modes.
3. **MOTHER's personality and interface** — How does she communicate? What does interacting with her feel like?
4. **Specific room decision design** — What do the actual phone screens look like for each room?
5. **Infection spread mechanics** — How does infection transfer in the new room model (no forced trading)?
6. **Reward balance** — What specific items/abilities exist? How many per game? Power curve?
7. **Event deck design** — What are the actual events? How do they test different room combinations?
8. **Cross-room interaction specifics** — How does Navigator calling out to Engineering actually work on phones?
9. **Onboarding** — How do new players learn this in-person? First turn tutorial?
10. **MOTHER game mode variations** — Detailed rules for Rogue AI, Puppet Master, Chaos modes.

---

## Endgame Exploration (In Progress)

Four endgame models under discussion:

**[Endgame #1]: Destination-Based** — Progress bar toward safety. Win by arriving before ship fails critically.

**[Endgame #2]: Cascading System Failure** — 4-5 ship systems with health bars. Any at zero = crisis. Two at zero = game over. Creates triage decisions.

**[Endgame #3]: The Final Event** — Last turn is always a massive multi-room crisis. Everything before is preparation. Ship health going in determines difficulty.

**[Endgame #4]: Combined (#2 + #3)** — Manage systems across turns 1-6, then face a final crisis on turn 7-8 whose difficulty scales with ship health. Infected strategy = slowly erode systems. Crew strategy = notice erosion and identify source.

**Infected win condition models:**
- Model A: Ship fails (hard for 1 vs. 5-7)
- Model B: Survive undetected to end (influence reaches destination)
- Model C: Achieve specific sabotage goal (knock system to zero, infect X players)
- Leaning: B + C combined

**Open sub-question:** How does endgame work in Rogue AI mode where there's no infected player? Crew realizes MOTHER is the threat? Vote to shut MOTHER down (but lose her systems if wrong)?

_Decision pending — Steven reviewing options._

### Endgame Continued — Theme, Win Conditions, and MOTHER Shutdown

**[Endgame #5]: Gradient Arrival Spectrum** — REJECTED
_Concept:_ Ship arrives in varying states of health, outcomes on a spectrum from perfect colonization to crash landing.
_Why rejected:_ Social deduction needs binary winners and losers. "I won, you lost!" is the point. Gradient only works in fully co-op games like Hanabi.

**[Theme #1]: Colony Ship — Earth Is Dying**
_Concept:_ Earth is dying. Players are civilians on a one-way colony ship heading to a new planet for habitation or a cure. Woken early from cryosleep by an emergency.
_Infected motivation:_ Came from the target planet, wants to get the ship to return to Earth (to spread influence).
_Rogue MOTHER motivation:_ Wants to return to Earth to corrupt other AI systems.
_Key insight:_ Both infected and rogue MOTHER have the same observable goal (redirect/sabotage the mission), making it hard to distinguish which threat you're facing.
_Status:_ STRONG THEMATIC DIRECTION — needs mechanical refinement.

**[Endgame #6]: Binary Arrival**
_Concept:_ Ship either arrives safely (crew wins) or doesn't (crew loses). Systems accumulate damage over 6-8 turns. Final turn is a culminating crisis. If enough systems are above threshold, crew wins. Post-game REVEAL of all hidden information — infection status, objectives, MOTHER's mode.
_Status:_ DIRECTION CONFIRMED — binary outcome with dramatic reveal.

**[Endgame #7]: The Override Vote** — EVOLVED into MOTHER Shutdown (#9)
_Concept:_ Crew votes to override MOTHER on individual systems, locking them in place. Surgical but complex.
_Evolution:_ Steven pushed toward binary MOTHER on/off rather than room-by-room, which is cleaner and more thematic.

**[Endgame #8]: Room-by-Room MOTHER Lockout** — SUPERSEDED by #9
_Concept:_ Disable MOTHER from individual rooms at a cost.
_Why superseded:_ Doesn't make sense to lock an AI out of one room — she's the ship's AI, it's all or nothing.

**[Endgame #9]: MOTHER Shutdown — The Kill Switch**
_Concept:_ Binary state — MOTHER is ON or OFF. Crew votes to shut her down. One player must go to AI Core room to execute and MAINTAIN the shutdown. If they leave, she reboots. While off, ALL rooms lose her support — everything harder across the board.
_Parallel to Brig:_

| | Brig (Traitor) | Shutdown (MOTHER) |
|---|---|---|
| Action | Lock up a player | Turn off MOTHER |
| Costs a person | Guard | AI Core operator |
| Neutralizes target | Player can't freely sabotage | MOTHER can't manipulate |
| If wrong | Wasted 2 crew | Crippled entire ship |
| Reversible | Vote to release | Operator leaves room |

_Status:_ CORE MECHANIC for Rogue AI mode.

**[Endgame #10]: Imperfect Shutdown — MOTHER Fights Back**
_Concept:_ When shut down, MOTHER retains influence over one random room each turn. Crew doesn't know which. AI Core operator might get a fuzzy hint. Shutdown is damage reduction, not elimination.
_Escalation path:_ Fully active → Shutdown (1 room lingers) → Hard shutdown (2 operators? late-game ability? fully offline)
_Status:_ RETAINED — adds tension to the shutdown decision.

**Infected player can weaponize MOTHER shutdown:** Push crew to shut down MOTHER in Classic mode (where she's fine) to cripple the ship. Same dynamic as brigging an innocent player.

**Puppet Master mode:** TABLED for later. Noted concern: requiring 1 operator for AI Core + 1 guard for Brig to contain one puppet master is steep for crew. Advanced mode problem — core modes (Classic + Rogue AI) need to be solid first.

### Self-Destruct Mechanic

Players have option to vote for self-destruct if they believe things are too compromised. Result: everyone likely loses (humanity goes extinct — one-way colony ship, Earth is dead). Extreme last resort. Possible future edge case: a game mode where self-destruct is actually the right call.

**Design goal:** Players should almost never want to self-destruct. The "keep fighting" incentive comes from the binary win condition — even a damaged ship can still make it if the final crisis goes well.

---

## Development & Testing Notes

**Bot/Simulation Testing (HIGH PRIORITY for later):**
Steven wants the ability to test the game with AI bots that act reasonably for their role. Use cases:
- Solo testing: 1 human + 6 bots to test full game flow
- Balance simulations: hundreds of automated games to tune parameters (Nudge corruption rates, event severity curves, MOTHER manipulation impact)
- Playtesting gap: reliable 7-player groups are hard to assemble, bots fill the gap

---

## Open Design Questions (Updated)

1. ~~**Endgame design**~~ — Direction confirmed: binary arrival + system health + final crisis. Details still needed.
2. **Nudge mechanic refinement** — How does Nudge work against the new effort+direction room model? Most impactful in dormant/rogue AI modes.
3. **MOTHER's personality and interface** — How does she communicate? What does interacting with her feel like?
4. **Specific room decision design** — What do the actual phone screens look like for each room? What decisions do players make?
5. **Infection spread mechanics** — How does infection transfer in the new room model (no forced trading)?
6. **Reward balance** — What specific items/abilities exist? How many per game? Power curve?
7. **Event deck design** — What are the actual events? How do they test different room combinations?
8. **Cross-room interaction specifics** — How does Navigator calling out to Engineering actually work on phones?
9. **Onboarding** — How do new players learn this in-person? First turn tutorial?
10. **MOTHER game mode variations** — Detailed rules for Rogue AI, Puppet Master, Chaos modes.
11. **Win condition details** — Exact thresholds for crew win vs. infected win. What "ship arrives safely" means mechanically.
12. **Hidden objective catalog** — Specific objectives across the alignment spectrum. How many? How assigned?
13. **Room list finalization** — Confirm room set including AI Core. How many rooms for 6-8 players?
14. **Bot/simulation architecture** — How to build AI players for testing. Behavior models per role.
15. **Why crew rotates rooms** — Thematic justification for civilians not camping one station (beyond the mechanical rule). Cryosleep skill recovery? MOTHER assigns shifts?
