# Agent Memory (v13, World Calendar canon)

## Purpose

This is the compact mutable state file for the writing agent.

The agent should read this file first before writing a chapter.

It is NOT the source of immutable canon.

Immutable canon lives in the other knowledge files and in `world_calendar.md`.

After every accepted chapter, update this file.

---

## WORKING STATE — AFTER CHAPTER 9

CURRENT INSTALLMENT: Season 1 — The Architect
CURRENT ARC: Era 2 — Elena, First Major Loss, and the Darkest Point (foundation-building phase)
CURRENT CHAPTER: Chapter 9 — Old Names, New Signs
CURRENT WC YEAR: WC15–16 (bridge; ends just before departure for the field operation)
CURRENT LOCATION: Guild headquarters / en route to the eastern forest
CURRENT POV: The Architect (first-person)

### Canonical chapter sequence so far

| Chapter                              |      WC | Location                                               | Key state at chapter end                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ------------------------------------ | ------: | ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Chapter 1 — Awaken                   |     WC0 | House of Father and Mother                             | Reborn as an infant with adult mind; parents established; magic has rules; silent vow to build a peaceful place                                                                                                                                                                                                                                                                                                                                                                                         |
| Chapter 2 — Learning to See          |  ~WC2–4 | Family home / village outskirts                        | Systematic observation and testing deepen; mana-lit stone and ambient magic established; unnamed Iris cameo establishes the two families already know each other                                                                                                                                                                                                                                                                                                                                        |
| Chapter 3 — First Light              | WC0–WC8 | Home village                                           | Household fire-globe observation establishes early magical pattern-testing; parents begin moving toward finding someone who can answer the Architect's questions; Teacher's home is seen from afar                                                                                                                                                                                                                                                                                                      |
| Chapter 4 — Teacher's Test           |     WC9 | The Teacher's house/study                              | The Teacher meets and accepts the Architect as an exceptional prospective student; formal apprenticeship is set to begin at WC10                                                                                                                                                                                                                                                                                                                                                                        |
| Chapter 5 — First Lessons            |    WC10 | The Teacher's house/study                              | Formal apprenticeship begins; The Teacher's core teaching method established (patience/observation before technique; theory bound to consequence); first successful spell (warming a stone via ambient Mana) after a real failure (drawing Mana from his own body); foreshadowing of "overconfidence about one's own limits" planted                                                                                                                                                                    |
| Chapter 6 — The Shape of Confidence  | WC11–14 | The Teacher's house/study; family village              | Architect advances rapidly, outperforms older Academy students in a "reality check" test; first independent research (mana-lit stone lifespan vs. temperature fluctuation) recognized by The Teacher as genuine research; reputation begins spreading among Mages; The Teacher delivers his most direct warning yet about untested limits; Mother echoes it — direct foreshadowing for WC16/Darkest Point                                                                                               |
| Chapter 7 — Two Signals in the Noise |    WC15 | Village square, harvest fair                           | The Architect formally meets Elena and Iris for the first time, triggered by a runaway lantern-golem cart; ACQUAINTANCE established with both, strictly platonic with Iris (12); The Teacher shows unexplained sharp attentiveness toward Elena; Elena plans to remain in the area a few more days                                                                                                                                                                                                      |
| Chapter 8 — A Name to Grow Into      |    WC15 | Village square/inn; nearby lake; village gate          | Over Elena's remaining days in the area, the Architect deepens genuine, non-romantic friendship with both Elena and Iris; Elena declines to give him a casual nickname, framing a name/title as something to grow into (direct seed for the WC35 "Architect" title); Iris's indirect caretaking pattern surfaces for the first time; Elena departs, promising the paths will cross again                                                                                                                |
| Chapter 9 — Old Names, New Signs     | WC15–16 | Teacher's house / family home / Iris's yard / Guild HQ | The Architect's overconfidence escalates into an active persuasive act to join the coming operation as an observer; Scout reports unusual, organized Demon activity; the old adventuring party (minus the now-Guild-Master tanker) decides to reunite; Guild Master introduced, providing support while staying behind; Father extracts a strict "observe only, retreat immediately" promise; Iris gives a directly foreshadowing farewell line; group departs for the eastern forest at chapter's end. |

**Continuity note:** Chapter 3 spans childhood material across WC0–WC8 and overlaps the broader period covered by Chapters 1–2. Treat its metadata as a chapter coverage range, not as a single chronological point. Chapter 6 similarly spans WC11–14 as a coverage range, ending at WC14. Chapter 7 and Chapter 8 both occur within WC15, with Chapter 8 immediately following Chapter 7 across the span of Elena's stated multi-day stay. Chapter 8 is the current chronological endpoint, still at WC15.

---

## PRE-WRITING CONTINUITY PROTOCOL — MANDATORY

Before writing ANY new chapter, the agent MUST establish the immediate narrative handoff from the previous accepted chapter.

### Step 1 — Identify the previous accepted chapter

1. Read `29-agent-memory.md` first.
2. Read `12-continuity-tracker.md`.
3. Identify `CURRENT CHAPTER` and `CURRENT WC YEAR`.
4. Locate the corresponding previous chapter file from the chapter sequence.
5. If the previous chapter filename is not known, search the available chapter files by **chapter number/title**, not by guessing.

### Step 2 — Read the previous chapter's metadata FIRST

Before drafting prose, locate and read that chapter's `## Chapter Metadata` and `## Continuity Update`.

Extract at minimum:

- Installment
- WC year / WC range
- POV
- Location
- Characters present
- Conflict
- Emotional objective
- Plot objective
- New facts
- Character changes
- Relationship changes
- World changes
- New objects / locations
- Foreshadowing
- Revealed secrets
- Unresolved questions

The previous chapter's metadata is the **handoff contract** for the next chapter.

### Step 3 — Determine the starting state of the new chapter

Explicitly establish:

- Where the story starts relative to the previous chapter
- How much time has passed
- Architect's computed age
- Current location
- Current POV
- Characters physically present
- Relationships at the start
- Active unresolved threads inherited from the previous chapter
- Foreshadowing that must remain active
- Secrets that must remain unrevealed

If any of these cannot be determined from the previous chapter metadata, inspect the previous chapter's prose and then the relevant canon files. **Do not invent a bridge merely to make the transition convenient.**

### Step 4 — Check the broader continuity chain

After reading the immediate previous chapter, check the relevant earlier chapter metadata when needed.

Priority order:

`29-agent-memory.md`
→ `12-continuity-tracker.md`
→ immediate previous chapter metadata
→ earlier chapter metadata
→ immutable canon / `world_calendar.md`
→ relevant character, relationship, magic, technology, mystery, or location files

Do NOT reread every chapter by default. Use the shortest evidence chain that can establish continuity.

### Step 5 — Perform a pre-write continuity check

Before drafting, verify:

- WC chronology is monotonic unless an intentional flashback is explicitly marked.
- Character ages match the Aging Rate System.
- Characters do not know information they have not yet learned.
- Secrets remain within their permitted reveal window.
- Relationship states continue from the previous chapter rather than resetting.
- Objects, locations, injuries, promises, and unresolved questions carry forward correctly.
- The Architect's first-person voice and adult-mind/child-body constraint remain consistent.
- No personal name is invented for The Architect.
- No romantic framing is introduced for underage characters.
- Any chapter-specific metadata must agree with the continuity tracker.

### Step 6 — After the chapter is accepted

Update BOTH:

- `29-agent-memory.md` — mutable current state / handoff summary
- `12-continuity-tracker.md` — durable chapter record

Never update memory from a draft that has not been accepted.

---

## CURRENT STORY STATE

The WC16 "First Major Loss" lead-up sequence is now formally underway. The reunited party (Father, Mother, The Teacher, Scout, plus the Architect as a strictly-observer-only addition) has departed for the eastern forest to investigate unusual Demon activity. The Guild Master, introduced this chapter, remains behind coordinating support. This is now the immediate setup for WC16 itself — the next chapter is the natural point for the battle to occur, pending explicit confirmation this is what the owner wants next.

---

## ACTIVE CHARACTERS

- **The Architect (15):** analytical, curious, pragmatic; has now experienced sustained, ordinary friendship valued for himself rather than his ability — a new emotional register built directly on top of Chapter 7's first taste of being seen as a person.
- **Elena (23.75):** established as warm, direct, perceptive, playfully teasing; keeps personal observation notes; can perceive Mana visually under strong disturbance; has shared a personal reflection on the loneliness of being seen only as "history" rather than a person; has departed the area, promising the paths will cross again.
- **Iris (12):** plainspoken, dry, practical, quietly observant; now shown exhibiting her first on-page indirect caretaking gestures (sharing food, offering to handle errands, a single dry vote of confidence in the Architect's character). Strictly platonic — no attraction framing until she is textually an adult (~WC21+).
- **The Teacher:** dry, guarded, weathered mage; not present in Chapter 8; his unexplained sharp attentiveness toward Elena (Chapter 7) remains unresolved and untouched.
- **Father:** retired A-rank swordsman; not present in Chapter 8, remains a stable emotional anchor.
- **Mother:** retired A-rank healer/enchantress; not present in Chapter 8.
- **The Scout/Investigator:** newly introduced on-page; female, scarred jaw, cautious and direct; discovered the unusual Demon activity that triggers the reunion.
- **The Guild Master:** newly introduced on-page; large, weathered, former tanker of the original five-person party; stays behind to coordinate Guild support; shows a guarded, evaluating attitude toward the Architect.

## CURRENT RELATIONSHIPS

- **Architect ↔ Father:** Father sides with the Architect's request to join the mission, but only under a strict, explicit condition (observe only, retreat at first danger) — a promise now structurally primed to be broken.
- **Architect ↔ Mother:** Mother's fear about her son's unusual nature is now openly stated for the first time, not merely implied.
- **Architect ↔ The Teacher:** mentorship continues in background; not directly advanced this chapter.
- **Architect ↔ Elena:** ACQUAINTANCE, moving toward FRIEND (`37-relationship-state-machine.md`) — deepened through several days of unstructured shared time; still no romantic framing. Elena has departed but explicitly signaled intent to return.
- **Architect ↔ Iris:** deepened through a brief platonic farewell scene; Iris's warning line is now active, direct foreshadowing.
- **Elena ↔ Iris:** confirmed, established close friendship; unchanged this chapter.
- **Architect ↔ wider Mage community:** unchanged from Chapter 6/7's growing regional reputation.

## CURRENT POLITICAL STATE

- No significant political changes established through WC15.

## CURRENT WORLD STATE

- Era 2 (Elena, First Major Loss, and the Darkest Point) continues its foundation-building phase.
- Magic remains established as rule-governed, costly, and dangerous if misused.
- A small lake outside the village is newly established as a recurring, non-registry backdrop tied to Iris and Elena's shared childhood.

## RECENT EVENTS

- **WC15 (Chapter 8):** Over the several days Elena remains in the area, she and the Architect spend unstructured time together — sitting at the inn steps, walking to a nearby lake, and sharing a final evening meal before her departure. Elena shares a personal reflection about being treated as "a walking history book" rather than a person; the Architect privately recognizes a resonance with his own hidden burden without disclosing it. Elena deliberately refuses to invent a casual nickname for him, instead framing a real name/title as something to be grown into. Iris participates with small, indirect caretaking gestures (sharing food, offering to accompany him on errands, a dry vote of confidence in his character) and one flat, non-jealous observation about Elena talking to the Architect more than to her. Elena departs the following morning, promising the paths will cross again.

## RECENT EMOTIONAL EVENTS

- The Architect experiences, for the first sustained stretch on-page, friendship valued for himself rather than his competence — building directly on Chapter 7's first glimpse of being seen as a person.
- A quiet moment of private resonance when Elena describes the loneliness of being treated as history rather than a person — the Architect recognizes a parallel to his own hidden burden but does not disclose it.
- Elena's refusal to assign him a casual nickname, reframed instead as "a name to grow into," lands as a small but weighty moment the Architect does not yet fully understand.
- Iris's dry, unprompted vote of confidence in his character — his first experience of being defended, however lightly, by someone his own general age group.

## ACTIVE MYSTERIES

- Who/what was the WC16 Demon ("The Unburied One") — see `26-mystery-board.md`. Keep backstage in Season 1.
- The Teacher's unfinished remark from Chapter 4 about "someone who thought this way" remains open and unaddressed.
- The Teacher's uncharacteristic sorrow from Chapter 6 remains open and unaddressed.
- The Teacher's unusually sharp attentiveness toward Elena in Chapter 7 remains open and unaddressed — not a formal mystery-board entry.
- (New, minor) Elena's brief cautious reaction upon hearing the Architect describe The Teacher's isolated, guarded teaching style — left deliberately unexplained, a very light gesture toward the still-open Teacher/Elena beat; not a formal mystery-board entry.

## PENDING FORESHADOWING

- "The Architect's City" nickname (~WC28–31) pays off at the WC35+ renaming to "Elena."
- The Teacher's WC10 line — "overconfidence about one's own limits is the real danger" — remains active foreshadowing for WC16 and the Darkest Point.
- The Teacher's WC14 line — "con chưa từng thực sự thất bại theo cách khiến con phải trả giá thật sự" — remains the clearest direct foreshadowing planted so far for WC16's First Major Loss. Do not resolve or call back explicitly before WC16.
- Mother's WC14 line — "có những thứ trên đời không có quy luật để tìm ra... chỉ có thể được cảm nhận, được chấp nhận, hoặc được mất đi" — direct, conscious thematic seed for Elena's WC23 "people are not variables" breakthrough. Do not resolve before WC23.
- The Teacher's remark about the Eterna experiencing time differently (Chapter 7) — gentle, early groundwork for the eventual emotional weight of Elena's long lifespan relative to the Architect's own. Do not over-explain; let it recede until it becomes relevant much later.
- (New, Chapter 8) Elena's "a name to grow into" motif — direct, deliberate thematic seed for the WC35 "Architect" title. Use sparingly; do not resolve before WC35.
- (New, Chapter 8) Elena's reflection on being seen only as "a walking history book" — plants groundwork for her later insistence on being treated as a full person, relevant again at WC23 and after her death.
- Iris's WC16-adjacent line — "Người ta thường hay không cần mang theo vũ khí vì họ nghĩ việc quan sát sẽ không thể trở nên nguy hiểm..." — direct foreshadowing for the Architect breaking his "observe only" promise at WC16.
- The Architect's promise to his father (observe only, retreat immediately) — must be referenced again, and broken, when WC16 occurs.
- Guild Master's passing remark about "what you all used to do back then" — light, unexplained; agent's discretion on future development.

## UNRESOLVED THREADS

- Unburied One's confirmed/unconfirmed destruction at WC40 — owner's discretion on whether this is ever settled on-page.
- Why The Teacher stopped taking students before the Architect (raised Chapter 4) — remains open.
- Whether the visiting Mage professor or any of the three unnamed Academy students from Chapter 6 recur later — currently one-time background characters; agent's discretion.
- Why The Teacher reacted with unusual sharpness upon seeing Elena (Chapter 7) — currently unexplained; agent's discretion on whether and when to develop this further.
- (New, minor, non-canon-critical) Elena's brief cautious reaction to hearing about The Teacher's teaching style — currently unexplained; agent's discretion.

## THINGS THE READER KNOWS

- The Architect was reincarnated into an infant body with adult memories.
- He instinctively analyzes magic as a system with rules, and has completed his first genuinely successful piece of independent magical research.
- His parents are retired A-rank adventurers: Father is a swordsman; Mother is a healer/enchantress.
- The Teacher is connected to the parents' former five-person adventuring party.
- The Architect has now formally met Elena and Iris and spent several additional days building genuine friendship with both; Elena is Eterna and ages far more slowly than he does.
- The Teacher reacted to Elena with an attentiveness the reader does not yet have an explanation for; Elena, in turn, reacted with brief caution upon hearing about The Teacher's style — the reader does not yet have an explanation for this either.

## THINGS THE CHARACTERS KNOW

- **The Architect:** knows his own reincarnation and Earth-origin memories; has now spent several days building real friendship with Elena and Iris; does not know why The Teacher reacted to Elena the way he did, nor why Elena reacted cautiously to hearing about The Teacher.
- **Father/Mother:** know the Teacher from their former adventuring life; unchanged this chapter (not present).
- **The Teacher:** has shown an unusual, unexplained level of attentiveness toward Elena; has not stated why; not present this chapter.
- **Elena:** knows she is Eterna, a longtime friend of Iris's family; has now spent several days with the Architect, sharing a personal reflection about being seen only as history; has departed, intending to return.
- **Iris:** knows Elena as her closest friend; has spent several more days with the Architect, deepening a purely platonic bond through small caretaking gestures.

## THINGS ONLY THE AUTHOR KNOWS

- The Unburied One's role as a hidden influence on Seraphine's faction (WC16–35) — not known to Seraphine, her faction leadership, the Architect, or the reader in Season 1.
- The specific reason behind The Teacher's uncharacteristic sorrow in Chapter 6, his sharp attentiveness toward Elena in Chapter 7, and Elena's own cautious reaction in Chapter 8 are left open for the agent to develop later without being obligated to resolve them before WC16.

## DO NOT REVEAL YET

- Any explicit WC16 ↔ WC33–35 Demon connection — no earlier than Movie 1, per reveal-discipline notes in `26-mystery-board.md` / `27-conflict-and-antagonist-board.md`.
- The full former-party history (Guild Master, Scout, WC16 battle) — remains backstage until WC16 itself.

## DO NOT CONTRADICT

- The Architect is born WC0 as an infant with full adult memory; he does not "awaken" as an already-grown adult.
- Elena ages at 0.25×, is already an adult (Eterna) when they meet at WC15.
- HARD RULE: all romantic/sexual content requires 18+ actual age (computed via each race's Aging Rate System, never apparent/soul age). Before 18, affection is written only as admiration/hero-worship — never romantic or sexual framing. This applies to every character, with no setting-based exception.
- Iris's romantic feelings never appear before she is 18 (~WC21+); before that, her attachment is written as childhood admiration only. Her WC15 introduction (age 12) is strictly platonic, characterized through plainspoken, practical dialogue and quiet approval — never attraction. Chapter 8's caretaking gestures remain within this same strictly platonic register.
- Seraphine is ageless and is always refused, never accepted, as a romantic partner. She is nicknamed "Sera" by the Architect post-WC35, at her own request, as acknowledgment she's no longer an enemy — not as romantic reciprocation. She is genuinely in love with him; once a Succubus truly falls in love she permanently loses her demonic combat power (ordinary magic only) — this is why she stops fighting and becomes the Son's magic teacher.
- The Princess is named Isolde Veyrand, princess of the Empire of Veyrand. The Architect refuses her even after Elena consents to a second marriage — this is his own principle, from his Earth-origin values, not merely deference to Elena or in-world custom.
- Elena's death and the Son's birth happen the same day (WC35).
- The Architect's death by old age is told inside Movie 1, not Season 1.
- "Builder" ≠ "Architect." The title is earned by respecting agency, not merely by ability.
- The Other Builder is properly named "Other Builder," not "Other Architect."
- WC16 "First Major Loss" (revised v7): not merely The Teacher's death. The Architect's parents (Father, swordsman; Mother, healer/enchantress), The Teacher, and the Scout/Investigator all die in the same battle against a high-tier Demon, defending the Architect after his tactical misjudgment. The Guild Master, absent, survives and later supports the Architect through The Guild.
- **RESOLVED, v8:** the WC16 Demon — continuity name "The Unburied One," true name withheld — is critically wounded, not killed. Dormant WC16–32; secretly influences Seraphine's domination-seeking faction from the shadows without her or her faction leadership's knowledge; presumed (unconfirmed) destroyed at WC40. Keep backstage in Season 1 prose; see `26-mystery-board.md`.
- The Empire of Veyrand is an Empire, not a Kingdom. Isolde is "Isolde Veyrand, princess of the Empire of Veyrand." Never refer to it as "Isolde's Kingdom."
- **RESOLVED, v8:** the Architect's city is renamed "Elena" (plain, no derived stylization) after her death (post-WC35 reconstruction). Motivation layer: informal use had been calling it "the Architect's City" (~WC28–31), which he privately disliked and deflected; the renaming is both memorial and a final refusal of that framing. Do not reintroduce an alternate stylization or drop the nickname motivation without explicit owner instruction.
- World Peoples now include, alongside Human/Eterna/Half-blood/Demon: Beastkin, Dwarf, Sylvan/Elf-adjacent, Undead/Revenant, Giant/Titan-kin.
- `43-ost-reference.md` has no "Season 3" — corrected to "Movie 2" (v8); the saga is Season 1 + Movies 1–4 only.

---

## CURRENT CHARACTER TRAJECTORIES

### The Architect

- Has now spent multiple days building real, ordinary friendship with Elena and Iris beyond their first meeting — a structural deepening of Era 2's opening.
- Continues carrying two independent, serious, unresolved warnings (Teacher, Mother) about untested confidence, entirely undisturbed by the events of this chapter.
- Primary immediate goal: continue training under The Teacher while maintaining the newly deepened friendships with Elena (now traveling) and Iris; next canonical milestones are further deepening toward FRIEND/TRUST state and, eventually, WC16's First Major Loss (must not be rushed).

### Elena

- Deepened from ACQUAINTANCE toward FRIEND across Chapters 7–8. Established as warm, direct, perceptive, teasing, and now shown as reflective and occasionally guarded about her own long life. Has departed the area but signaled clear intent to return.
- Next steps: further deepen the friendship with the Architect and Iris in subsequent chapters, working the relationship state machine toward FRIEND and eventually TRUST, well ahead of the WC23 breakthrough.

### Iris

- Deepened within ACQUAINTANCE (WC15, age 12) through her first on-page indirect caretaking gestures. Still strictly platonic — no romantic/attraction framing before adulthood (~WC21+).

### Seraphine

- Not yet active in the current story period.

### Isolde

- Not yet active in the current story period.

### Son

- Not yet born.

### Mira

- Not yet active.

### The Other Builder

- Not yet active.

### Noah

- Not yet active.

## CURRENT ROMANCE STATE

PRIMARY:
The Architect ↔ Elena — ACQUAINTANCE moving toward FRIEND (WC15, deepened across Chapters 7–8)

SECONDARY ATTRACTIONS:

- Iris — ACQUAINTANCE, strictly platonic (age 12; adult-only attraction begins ~WC21+)
- Seraphine (guilt-driven, permanently refused; not yet active)
- Isolde (political-then-genuine, permanently refused; not yet active)

## ELENA STATUS:

Formally introduced at WC15, per `world_calendar.md` / `02-timeline.md`. Currently at ACQUAINTANCE-moving-toward-FRIEND stage with the Architect; has departed the area after several days, with a stated intent to return.

---

## CURRENT FAN-SERVICE LEVEL

Installment baseline: Season 1, highest of the saga overall.
CURRENT LEVEL: None/minimal — Elena and Iris remain at ACQUAINTANCE/early-FRIEND level; no fanservice framing is appropriate yet.

## Allowed:

N/A yet — relationships are at ACQUAINTANCE/early-FRIEND stage only.

## Avoid:

Any romantic/attraction framing involving Iris before ~WC21. Any premature romantic escalation with Elena beyond ACQUAINTANCE/early-FRIEND.

---

## CURRENT TECHNOLOGY LEVEL

- Early magical infrastructure; household enchanted lighting and simple magical utility systems; village-level enchanted goods such as lantern-golem carts exist and are imperfect/prone to malfunction.
- The Architect has completed original applied research into mana-lit stone longevity — the first seed of his later technology work, though not yet formalized as an invention or shared beyond The Teacher.

## CURRENT MAGIC LEVEL

- Ambient magic and basic enchantment are established.
- The Architect has advanced from single-action spellcraft (warming a stone) to sustained-effect constructs ("khung ý chí") and has demonstrated clear superiority over older, formally-trained Academy students in a controlled test.
- Elena has demonstrated Light-affinity magic used for calming/soothing distress, consistent with the Eterna's Light/Time affinity (`00-story-bible.md`), and has shown she can perceive Mana visually under strong disturbance.

## CURRENT FACTION STATE

- No major faction conflict active.
- The Teacher's former adventuring party is relevant as hidden backstory, not as an active faction.
- A loose, informal "reputation network" among regional Mages continues around the Architect — not an organization, just an emerging social fact.

## CURRENT LOCATION STATE

- City name: resolved as plain "Elena" (post-WC35 rebuild). Pre-WC35, informally "the Architect's City" (disliked, never adopted). Not yet founded — City Project begins WC28.
- A small lake outside the village is newly established as a recurring, non-registry backdrop tied to Iris and Elena's shared childhood.

## CURRENT ARTIFACT STATE

- The Architect's early research notes (mana-lit stone lifespan study) are a non-registry precursor to the "Architect's Notebooks" described generically in `24-artifact-registry.md`; no new registry entry required yet.
- Elena's personal observation notebook is newly established as a minor, non-registry personal object; may recur.

---

## LAST CHAPTER SUMMARY

**Chapter 8 — A Name to Grow Into (WC15):** Over the several days Elena remains in the area following Chapter 7, she and the Architect deepen a genuine, entirely non-romantic friendship — sitting together at the inn steps, walking to a nearby lake, and sharing a final evening meal. Elena reflects on the loneliness of being seen only as history rather than a person, a sentiment the Architect privately recognizes without disclosing his own hidden burden. She deliberately declines to invent a casual nickname for him, framing a real name/title as something to be grown into — a direct thematic seed for the "Architect" title at WC35. Iris shows her first on-page indirect caretaking gestures (sharing food, offering to accompany him on errands, a dry vote of confidence in his character) while remaining strictly platonic. Elena departs the following morning, promising their paths will cross again.

## NEXT CHAPTER INTENT

- The group has now departed for the eastern forest. WC16 — First Major Loss — is the natural next event and should not be delayed further without explicit owner instruction, since the deliberate buildup requested earlier has now been substantially completed across Chapters 6–9.
- Do not reveal the Unburied One's identity or its WC16→WC33–35 connection.
- Preserve Iris's strictly platonic framing (age 12–13) throughout any further Chapter 9-adjacent material.

## CONTINUITY WARNINGS

- Chapter 3's metadata covers WC0–WC8 and overlaps Chapters 1–2; do not interpret it as a single event occurring after Chapter 2.
- Chapter 6's metadata covers WC11–14 as a coverage range; Chapter 7 and Chapter 8 both occur within WC15, with Chapter 8 following directly after Chapter 7.
- Chapter 8 is the current chronological endpoint, still at WC15.
- Do not reveal the WC16 tragedy, the full former-party history, Builder terminology, or the Unburied One early.
- The Architect's Earth-origin knowledge must remain selectively concealed in-world.
- Iris is not a romantic interest during childhood; attraction begins only at adulthood (~WC21+). Her Chapter 7–8 scenes are strictly platonic (age 12).
- Never give The Architect a personal name.
- Elena's introduction and subsequent bonding at WC15 must not be rushed into romance; the relationship state machine (`37-relationship-state-machine.md`) requires FRIEND → TRUST → the WC23 breakthrough before LOVE.

## MEMORY UPDATE RULE

Only record confirmed events from accepted chapters.

Do not store speculation as fact.

When a contradiction is discovered, flag it instead of silently rewriting history.

## CURRENT PROTAGONIST IDENTITY RULE

PERSONAL NAME:
NONE / DO NOT INVENT

IN-WORLD TITLE:
The Architect (earned WC35; distinct from the broader category "Builder")

NARRATIVE IDENTITY:
Reader-projectable first-person protagonist, adult mind from birth (WC0) in an infant/child body.

PHYSICAL SPECIFICITY:
Keep intentionally moderate unless scene requires detail.

VISUAL DEFAULT:
Back / side / silhouette / over-the-shoulder / partially obscured face.

## CURRENT VISUAL STATE

## ACTIVE CHARACTER DESIGNS:

## ACTIVE LOCATION DESIGNS:

## ACTIVE ARTIFACT DESIGNS:

## LAST CANONICAL ILLUSTRATIONS:

## PENDING ILLUSTRATIONS:

## IMAGE CONTINUITY WARNINGS

- Never give the protagonist a personal name.
- Never turn "The Architect" into a civilian name.
- Never accidentally use another character's design for Elena, Iris, Seraphine, or Isolde.
- Never depict Iris with any romantic/attraction framing before she is an adult (~WC21+).
- Keep age (computed via the Aging Rate System), costume, technology, and location consistent with the current WC year.
