# Replacing the stock photos with generated ones

Two photos on the site are generic stock. Generate replacements (ChatGPT image / DALL·E, or any
image model), save them with **exactly these filenames** over the existing files, and the site
picks them up with no code change.

| File | Where it shows | Size to generate | How it is cropped on the page |
|---|---|---|---|
| `photos/hero-care.jpg` | Top of the page, the big photo card | **1600 × 1067 (3:2)** or larger | Tall card, roughly 5:6 — keep the subject in the **middle 60%** |
| `photos/about-clinician.jpg` | "Who we are" section, left photo | **1600 × 1067 (3:2)** or larger | Nearly square, about 5:4.6 — keep the subject centred |

Save as JPG, quality 85–90. Under 400 KB each is ideal (the site loads with no internet dependency,
so file size is the only cost).

## Rules that keep the site honest and PHI-safe

- **No faces, or faces soft-focus / turned away.** A generated "clinician" with a clear face reads
  as a real Lavida provider. Hands, shoulders, backs, silhouettes are all fine.
- **No visible wound, dressing removed, or clinical detail.** Suggest care, do not show injury.
- **No text anywhere in the image** — no name tags, badges, signage, screens with words, logos.
  Generated text comes out garbled and a fake badge looks like a fake credential.
- **No recognisable facility.** A generic, warm room — not a specific building.
- Photographic, not illustrated. Ask for "photograph", a real lens, natural light.

## Palette to match the site

Warm cream, soft sage green, terracotta accents, navy for depth. Morning light. Avoid cold blue
hospital tones — the whole point of the brand is *care at the bedside, not a hospital*.

## Prompts (paste as-is, then adjust)

**hero-care.jpg — "brought to the bedside"**

> Editorial photograph, 3:2 landscape. A clinician's gloved hands gently holding an elderly
> resident's hand at the bedside of a skilled nursing facility room. Soft morning window light,
> warm cream and sage tones with a small terracotta accent (a blanket edge). Shallow depth of field,
> 50mm lens, calm and dignified. No faces visible, no text, no logos, no badges, no visible wounds
> or dressings. Photorealistic, natural skin texture, not stylised.

**about-clinician.jpg — "a partner your nurses can reach"**

> Editorial photograph, 3:2 landscape. A wound-care clinician in a sage-green scrub top and a
> facility nurse standing together at a nurses' station in a nursing home hallway, reviewing
> something on a tablet, shown from the shoulders down or with faces turned away and out of focus.
> Warm natural light, cream walls, wood accents. Shallow depth of field. No readable text on the
> tablet or walls, no name badges, no logos. Photorealistic.

**Optional third — for a future section**

> Editorial photograph, 3:2. A clinician's supply bag and a folded sage blanket on a chair by a
> sunlit nursing-home window, terracotta cushion, no people, no text. Calm still life, warm light.

## After saving

Open the site and check the top card and the "Who we are" photo. If a subject is cut off, the crop
notes in the table say which part of the image needs to hold it.
