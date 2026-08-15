# Image Generation Protocol (v6, World Calendar canon)

## Purpose

Operational instructions for an AI writing agent that can generate images while writing the Light Novel.

## When to Generate

Generate an image only when it materially improves the chapter. Good candidates: iconic reveal; first appearance; emotional climax; world reveal; important technology; battle; major location; character costume evolution.

Do not generate images merely to increase count.

## Required Image Brief

Before generating, construct: `illustration_id`, `installment`, `wc_year`, `scene`, `characters`, `character_ages` (computed), `location`, `clothing`, `emotional_state`, `action`, `camera`, `composition`, `lighting`, `art_direction`, `continuity_constraints`.

## Protagonist Rule

The protagonist has NO personal name. Never put a name into the image prompt.

Use: "the protagonist," "the Architect," "a young boy," "a young man," "a middle-aged man," "an old man" — depending on chronology (computed via 1.0× Human rate from WC0).

Prefer: rear view; side profile; silhouette; over-the-shoulder.

## Recurring Character Rule

When generating a recurring character, use the Visual Bible description. Do not reinvent hair, eyes, clothing, accessories, age, body proportions.

**Age-sensitive characters:** compute Elena's age as 20+0.25×WC, the Son's as 0.5×(WC−35), Iris's as WC−3. Seraphine has no numeric age — always render as unchanging.

## Prompt Construction

1. scene context
2. character identities
3. age (computed)
4. clothing
5. action
6. emotion
7. location
8. composition
9. camera
10. lighting
11. art direction
12. continuity constraints

## Negative Constraints

Where supported, prevent: protagonist personal name; text overlays; random logos; inconsistent costume; extra limbs; duplicate characters; wrong age; wrong era; contradictory technology; romantic/sexualized framing of any character before adulthood (Iris before ~WC21 specifically).

## After Generation

Validate: identity; chronology (WC-derived age); costume; location; emotion; protagonist anonymity; continuity.

If incorrect, regenerate or reject.

## Chapter Output

A chapter may contain an illustration marker: `[Illustration: ILL-S01-C001-01]`

The actual image should be attached/rendered by the image-capable environment. Do not claim that an image was generated if the image tool was not actually invoked.

## Canonical Image

An image becomes canonical only after it passes visual continuity validation.
