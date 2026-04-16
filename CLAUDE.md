# Hidden Grammar: The English Pragmatics Learning Hub for Autistic Individuals

## Project overview

This is a comprehensive, research-grounded learning hub that teaches English pragmatics to autistic individuals. It is built on the **double empathy problem** (Milton 2012): communication breakdowns between autistic and non-autistic people are bidirectional mismatches, not unilateral autistic deficits. Every page in this hub is framed accordingly.

The hub treats pragmatic learning as acquiring a second communicative dialect, not remediating a broken faculty. It is neurodiversity-affirming, research-first, and honest about evidence quality.

## Directory structure

```
content/
  introductions/          4 Tier 1 entry-point pages (narrative + deep dive format)
  categories/             27 category directories, each containing:
    NN-topic/
      topic.md            Main category page
      research/           Research files (theory, autism, practical, etc.)
  manipulation-hub/       40-page Pragmatic Manipulation and Self-Protection sub-hub
    overview.md           Category summary
    framework/            5 framing pages (safety assessment, crisis resources, etc.)
    patterns/             15 manipulation pattern pages (gaslighting, DARVO, etc.)
    strategies/           10 protection strategy pages
    contexts/             10 context-specific pages (workplace, intimate partner, etc.)
    research/             3 foundational research + 3 category-level research files

references/
  citations-index.md      Annotated master citations index (982 entries, independently verified)
  annotation-findings.md  Running log from Stage 3.5 annotation pass
  raw-annotations/        JSON annotation data (12 slice outputs + canonical inventory)

planning/
  phase-2-plan.md         Phase 2 master plan (Stages 1-10)
  hub-research.md         Original Phase 1 research document
  gap-audit.md            Stage 2 gap audit deliverable
  manipulation-build-plan.md  Sub-hub build plan and status
  page-template.md        Narrative + Deep Dive content template
  validation/             Research validation chunk logs
```

## Content design rules

All reader-facing pages use the **Narrative + Deep Dive** template (see `planning/page-template.md`):

1. **Two-part structure**: flowing narrative (no headers beyond page title) followed by `## Deep Dive` with structured subsections.
2. **Narrative = 40-60% of page**. Carries the full argument including load-bearing caveats.
3. **No clinical labels** ("Key Takeaways," "Core Message"). Trust the narrative.
4. **Minimize em-dashes**: 1-2 per page maximum. Replace with commas, colons, periods, semicolons. Em-dashes signal AI-generated content.
5. **Explicit logical connectives** ("because," "this means," "the consequence is") for autistic reader accessibility.
6. **Every load-bearing caveat in the narrative**. Deep Dive expands but does not introduce caveats.
7. **Evidence by description in narrative** ("Crompton's diffusion-chain experiments"), formal citations in Deep Dive.

Reference implementation: `content/introductions/double-empathy-problem.md`

When rewriting pages, always run a validation agent to diff old vs. new and confirm no claims, citations, or caveats were lost.

## Citation handling

The annotated citations index (`references/citations-index.md`) contains 982 independently verified entries. Every citation was checked not just for existence but for claim-support: does the source actually support the claim the hub uses it for?

### Known citation gotchas

- **Rozenkrantz 2021** "A mechanistic link between prior information and autism" is a CONFABULATED title. The real paper is "Enhanced Rationality in Autism Spectrum Disorder" (TiCS 25(8):685-696). Citable for "reduced cognitive biases" but NOT for "attenuated priors."
- **For attenuated priors**, cite **Pellicano & Burr (2012)** "When the world becomes 'too real'" (TiCS 16:504-510).
- **Williams, Wharton & Jagoe (2021)** is in *Frontiers in Psychology* 12:616664, NOT *J Pragmatics*.
- **PMC4764348** is de Marchena & Eigsti (2015/2016), not Hyter 2017 or Nadig 2009.
- **Carney/Cuddy/Yap (2010) power posing** carries replication baggage. Prefer Hall/Coats/LeBeau (2005) for "posture signals status."
- **Binns & Oram Cardy (2019)** DOI resolves to *Review Journal of ASD*, not *Autism & Developmental Language Impairments*.

## Evidence quality labels

The hub uses five evidence tiers:
- `[VALIDATED]` — replicated, peer-reviewed
- `[PRELIMINARY]` — single study, peer-reviewed
- `[EXTRAPOLATED]` — inferred from adjacent evidence
- `[COMMUNITY KNOWLEDGE]` — widely reported in autistic community, limited formal study
- `[CONTESTED]` — active scientific disagreement

## Section 12 forbidden claims

The manipulation sub-hub's trauma-frameworks research file identifies claims that must NOT be presented as fact:
- Triune brain model (MacLean), polyvagal theory literalism (Porges), "body keeps the score" as literal mechanism, recovered memory therapy, universal post-traumatic growth, "time heals all wounds," forgiveness-as-requirement, pop-gaslighting (clinical term misuse), "narcissistic abuse" as clinical diagnosis, "boundaries" as slogan without operational definition.

## Research-only repository

All content in this repo is research and drafts. No webpage generation happens here. The eventual interactive learning platform will be built separately, consuming this research as source material.
