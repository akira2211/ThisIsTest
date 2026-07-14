# Prompt: Build H1 2026 Achievement HTML Report (CEO Edition)

You are building **one standalone, executive-grade HTML report** for the
**H1 2026 achievements of SHRC VD S/W Engineering Development**.

Audience: **CEO, top executives, department leaders**. The first screen must be
understandable by a non-engineer in 10 seconds. Deep technical evidence stays
available but collapsed.

---

## Step 0 — Use the html-skills plugin (MANDATORY)

The `html-skills` plugin (from `f-labs-io/agent-html-skills`) is installed.
Before writing any HTML:

1. List the available skills from the plugin and read the SKILL.md of every
   skill relevant to this task. Expected candidates:
   - the **structured document / report / dashboard** skill (executive
     documents with metric cards, charts, collapsible references) — this is
     the PRIMARY skill for this report
   - **html-svg-diagrams** — for the 4-team value-chain diagram and any
     architecture flow you redraw
   - the **deck** skill only if I later ask for a slide version (do NOT
     produce a deck now)
2. Follow the plugin's **HTML output foundation** rules exactly (typography,
   spacing, contrast, no innerHTML with variables, `<foreignObject>` for SVG
   labels, visible last-updated timestamp in the footer, descriptive
   filename).
3. Do NOT use the interactive/submit-button skills. This report is
   read-only; no round-trip needed.
4. Charts must render locally with no external CDN. If the skill provides a
   chart component, use it; otherwise inline SVG.

Output file name: `h1-2026-sw-engineering-achievement-report.html`
(saved next to this prompt, sibling of `assets/`).

---

## Step 1 — Read the sources

1. Read the achievement source document(s) in this folder.
2. Scan the `./assets/` folder. Build an internal list of every image file
   name. These are screenshots/diagrams from my monthly report slides
   (architecture diagrams, latency charts, flow diagrams, kernel-porting
   illustrations, operation charts).
3. If a section of the report would clearly benefit from an image but no
   matching file exists in `assets/`, add a visible placeholder card that
   says `IMAGE NEEDED: <what>` and list all such requests at the end of your
   reply to me. Never invent or generate a fake image.

### Source hygiene rules

- Do not invent any number, result, or benefit.
- The May 2026 section is duplicated in the source — count it ONCE.
- Treat monthly counts as monthly values unless the source says cumulative.
- If a half-year total cannot be safely computed, show the monthly trend
  instead and label it "monthly".
- Distinguish clearly: Completed / In Progress / Routine operation / Planned.

---

## Step 2 — Core executive story

One organization, one story, four layers:

> Four specialized teams jointly provide end-to-end TV software readiness —
> from kernel and memory foundations, through visual experience and system
> integration quality, to application certification and global release.

Value chain (render as an SVG diagram using html-svg-diagrams, not ASCII):

```
TizenLite → OpenGL → System S/W Verification → App Operation
(Platform    (Visual     (Integration quality &      (App ecosystem &
foundation)  experience)  product readiness)          release assurance)
```

Each stage protects the next stage. Say so on the diagram.

---

## Step 3 — Teams and strategic pillars

| Team | Executive role | Pillar |
|---|---|---|
| TizenLite | Memory management, kernel allocators (CMA/GCMA/ZRAM), Linux 6.12 migration, boot & SAM performance | **Pillar 1: Platform Stability & Performance** |
| OpenGL | Lifestyle/ambient apps, screen savers, brush & blur effects, graphics API quality | **Pillar 2: Differentiated Visual Experience** |
| System S/W Verification | BM framework, chipset/model bring-up, automation infrastructure (VTS-BM, BTS, Hurdle), AI-assisted verification | **Pillar 3: Product Readiness & Verification Transformation** |
| App Operation | App certification, SP-Review, release governance, compatibility, partner support | **Pillar 4: Application Ecosystem & Release Assurance** |

Every achievement is tagged with: team, pillar, status, and 1–3 impact
categories from: Product readiness · Quality & risk reduction · Performance &
resource efficiency · Automation & productivity · Technology capability ·
Ecosystem & partner support.

### Achievement classification (3 levels)

- **A. Strategic achievements** → full cards (6–8 only, org-wide). Strong
  candidates: Linux 6.12 kernel/memory migration; GCMA 6–22x latency
  improvement over CMA; SAM score improvements (reclaimd/fastboot); BM
  Scenario Intelligence Generator; VTS-BM / BTS infrastructure expansion; PC
  Timing multi-target automation; X24UL/X26UL bring-up (SOC issues detected
  early); automated PPTX/report generation via LLM; app-verification
  automation.
- **B. Operational performance** → KPI cards / trend charts (KONA DF handled,
  Jira resolved, apps certified/released, SP-Reviews, App Admin, partner Q&A).
  Do not present routine volume as strategic achievement.
- **C. Work in progress** → smaller roadmap/progress section (CMA Pinner tool,
  Scenario Generator Phase 2, feasibility studies). Never at the same visual
  level as completed outcomes.

---

## Step 4 — Page structure

1. **Hero** — title, period, one-sentence summary, value-chain SVG.
   - Title: *H1 2026 SHRC Software Engineering Achievement Report*
   - Subtitle: *End-to-End TV Software Readiness: From Platform Foundation to Global Application Release*
2. **Executive summary** — ≤150 words: what was delivered, why it matters,
   risk reduced, productivity gained.
3. **Executive KPI dashboard** — 8–12 verified KPIs across the 4 teams.
   Label each value: exact/approx, monthly/cumulative.
4. **Strategic pillar overview** — 4 cards (purpose, owner, top wins, key
   metric, H2 priority).
5. **Top organization achievements** — 6–8 detail cards, each with:
   Executive summary · Context · Challenge · Action · Result · Business
   impact · Metrics · Status · Team/Pillar · expandable Technical details ·
   **supporting image from assets (see Step 5)**.
6. **Cross-team impact matrix** — business objectives × 4 teams,
   qualitative High/Medium/Low, only where supported by the source.
7. **Monthly trend section** — secondary view; line charts for trends, bars
   for volume. Do NOT make the monthly timeline the main structure.
8. **H2 2026 priorities** — 5–7 items, separated into Committed /
   In-progress / Proposed. Never claim planned work as done.
9. **Technical appendix** — collapsed by default: acronym glossary, full
   activity lists, metric definitions, data-quality notes (including the
   May-duplication handling).

---

## Step 5 — Image usage rules (assets/)

These images are evidence. Use them to make achievement cards credible, not
as decoration.

1. Reference by **relative path** `assets/<filename>`; never base64-embed,
   never hotlink external images.
2. Every image gets a `figure` with a short **caption** and meaningful `alt`
   text (executive language, not filename).
3. Images inside achievement cards default to a compact thumbnail
   (max-height ~280px, object-fit contain, subtle border) with
   **click-to-enlarge** (a simple CSS/JS lightbox, no library).
4. Screenshots of slides may contain Korean UI chrome, rulers, or camera
   glare — crop visually via CSS (container + overflow hidden) is acceptable;
   do not stretch or distort.
5. Expected image-to-section mapping (match by filename/content; adjust to
   the real names you find in `assets/`):

| Content of image | Place in |
|---|---|
| GCMA introduction / architecture diagram, GCMA vs CMA latency charts (4–96MB) | Pillar 1 → GCMA achievement card |
| Kernel module porting for Linux 6.12 (CMA_ZONE & mem_logger illustration) | Pillar 1 → Linux 6.12 migration card |
| Blue Mountain PC Timing multi-target topology (NVIDIA/AMD PC, splitters, TVs) | Pillar 3 → PC Timing automation card |
| VTS-BM Server / Full Test Setup system overview | Pillar 3 → verification infrastructure card |
| BM Scenario Intelligence Generator architecture (N8N UI, orchestration agent) | Pillar 3 → AI-assisted verification card |
| PPTX Generation Flow Diagram (Web UI → Backend → LLM → Layout & PPTX) | Pillar 3 → automation productivity card |
| App Operation monthly bar/line charts | Redraw as native chart from the table data if numbers are legible; keep the screenshot only in the appendix as evidence |
| Plan & Schedule timeline (Design → PR Support) | Pillar 3 card or H2 roadmap section |

6. Prefer **redrawing data charts natively** (SVG) when the underlying
   numbers are available in the source tables; use the screenshot as
   collapsed evidence. Use the screenshot directly when it is an
   architecture/topology diagram.
7. Remove or avoid anything marked Confidential footer in a way that
   dominates the layout — the report itself is internal, but crop the slide
   chrome where possible.

---

## Step 6 — Language & tone

- Clear professional English; fix grammar from the source; keep technical
  names exact (GCMA, ZRAM, VTS-BM, KONA DF...).
- Define every acronym on first use + glossary tooltip.
- Executive sections: outcome first, no jargon. Technical wording goes in
  expandable details. Example transformation:
  - Source: "Completed backport SWAP-related components for Linux 6.12 (ZRAM, ZSmalloc, ZSTD)"
  - Executive: "Advanced Linux 6.12 platform readiness by migrating the
    critical memory components required for next-generation TV products."
- No marketing language, no invented cost savings, no exaggeration.

---

## Step 7 — Visual & interaction requirements

- Premium corporate style: white / dark navy / deep blue / light gray, one
  subtle accent. No playful gradients.
- Sticky top navigation; filters by team, pillar, status; expandable cards;
  acronym tooltips; back-to-top; print-friendly CSS (print = executive view,
  appendix expanded optional).
- Responsive desktop/tablet; accessible (WCAG AA contrast, keyboard focus,
  status conveyed by label not color alone).
- Single HTML file, embedded CSS/JS, zero external dependencies, opens
  directly in a browser. Images stay as relative-path files in `assets/`.

---

## Final checklist (verify before finishing)

- [ ] Relevant html-skills SKILL.md files were read and followed
- [ ] Four teams presented as ONE organization; report opens with business impact
- [ ] Strategic vs operational vs in-progress clearly separated
- [ ] May 2026 counted once; no invented or uncertain totals shown as exact
- [ ] Every assets image referenced by relative path with caption + alt text
- [ ] Missing-image requests listed back to me
- [ ] All acronyms explained; first screen CEO-readable
- [ ] File opens standalone in a browser; print layout verified
