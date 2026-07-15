# Prompt: Build "AX — AI Utilization & GrowHive" HTML Report

You are building **one standalone, executive-grade HTML report** covering the
**AX (AI Transformation) activities of VD SW Group, H1 2026**: AI utilization,
AI Best Practice awards, AX-supported projects, and the GrowHive adoption
program.

Audience: **top leaders / CEO**. Executive language first; technical and
per-project detail stays in expandable sections.

---

## Step 0 — Use the html-skills plugin (MANDATORY)

The `html-skills` plugin (from `f-labs-io/agent-html-skills`) is installed.
Before writing any HTML:

1. List the plugin's skills and read the SKILL.md of every relevant one:
   - the **structured document / report / dashboard** skill — PRIMARY skill
   - **html-svg-diagrams** — for the GrowHive milestone timeline and the
     AI Best Practice monthly timeline (redraw natively, do not screenshot)
2. Follow the plugin's **HTML output foundation** rules (typography, spacing,
   WCAG AA contrast, no innerHTML from variables, `<foreignObject>` for SVG
   labels, footer timestamp, descriptive filename).
3. No interactive/submit skills — this is a read-only report.
4. All charts render locally (skill components or inline SVG). No CDN.

Output file: `ax-ai-utilization-report.html` (sibling of the `AX/` folder).

---

## Step 1 — Read the sources

1. Read the source notes file (this project's general write-up).
2. Read the **`AX/` folder (exclude `AX/assets/`)** for schedule details of
   the two AX-supported projects; summarize into a project timeline showing
   progress, number of functions delivered, and milestones.
3. Scan `AX/assets/` and map every image (see Step 6).
4. If an image referenced in the notes is missing from `AX/assets/`, insert a
   visible `IMAGE NEEDED: <name>` placeholder and list all such requests back
   to me. Never invent an image or a number.

---

## Step 2 — Page 1: AI Utilization

Layout: two columns (left content, right images stacked top/bottom).

**Left — narrative:**
- Program started March 2026: all developers encouraged to use **Cline-SR**,
  reinforced by real activities — VD SW Group's monthly **Best Practice
  Reward & Sharing** to boost AI utilization.
- Cline-SR = AI-based coding assistant enabling agent-based coding:
  code analysis & generation; defect fixing & structural improvement
  (refactoring); analyzing code + specification and improving algorithms.
- **Headline KPI (make this a big stat pair):** adoption grew from
  **129/170 users (~76%) in March → 100% of engineers in June** (Cline-SR
  used in daily work). Render as a progress/adoption visual, not plain text.
- **AI Best Practice (monthly):** identify & promote best practices of AI in
  SW development; enhance efficiency/productivity; foster an AI work culture.
- **Milestone timeline (Mar→Jun), render as a small native chart:**
  March 2 projects · April 5 · May 3 · June 1 (11 awarded projects total).

**Right — images:** `AX/assets/AI_Utilization_1.png` (top),
`AX/assets/AI_Utilization_2.png` (bottom). Cline images
`AX/assets/Cline_SR_1.png` and `AX/assets/Cline_SR_2.png` go with the
Cline-SR block (thumbnail + click-to-enlarge).

---

## Step 3 — Page 2: AI Best Practice (interactive)

Requirement from me, implement exactly:

> Show a **table of awarded projects by month**. Clicking a row expands (or
> opens a detail panel) showing the project introduction, benefit, and image
> if available.

- Table columns: Month · Project · One-line summary · Category (e.g., Coding
  assistant, Document automation, Test automation, Ops automation, Knowledge
  management) · Has image?
- Expandable detail per project uses the introductions from the source notes
  (rewrite into clean professional English; keep facts, do not exaggerate):
  - **March:** E-Paper Application AI function PoC (AI content creation +
    AI Handwritten Converter for Flip screens) — image
    `AX/assets/E-Paper Application AI function PoC.png`; AI Document
    Automatic Creating Tool (SEHC Chatbot → Kona API → Samsung Gauss AI →
    auto-creates eCODE issues) — image
    `AX/assets/AI document automatic creating tool.png`.
  - **April:** Cline Kit (61 skills / 8 rules / 5 workflows, Web UI or CLI);
    AI-Powered SAM Analysis Report with Gauss (analysis time from hours to
    minutes, structured HTML reports with troubleshooting guidance);
    Screen Extractor (OCR of OSD to Excel, 33 Flip languages, screen or
    webcam capture); Asset Management System (LLM invoice extraction replaces
    email-based MRO purchasing, intranet sync); Monitor AI Cline Skills
    (LEMON 2026 monitor firmware — automation, code quality, PLM-integrated
    defect resolution).
  - **May:** Release Automation Tool (end-to-end TV Plugin release: version
    bump, Git, CI/CD monitoring, APK signing, Galaxy deployment, docs);
    PM Onboard AI Assistant (self-service onboarding Q&A, reduces mentor
    load, Confluence quick search); AI-Powered Carry-in Document Creation via
    Cline Skills (Cline orchestrates Knox Portal/Intranet APIs; avoids
    storage-charge overruns from the 4-day vendor window; outputs CIT/
    Carry-in Excels).
  - **June:** Decision Manager (GraphRAG over Samsung chat/email exports,
    local ONNX embeddings + GaussO Think; decision lookup from 30–60 min to
    <30 sec, cited and second-pass-verified answers).
- Keep quantified benefits visible (hours→minutes, 30–60 min→<30 sec,
  76%→100%) — these are the executive hooks.

---

## Step 4 — Page 3: AX Activity

**Supported projects (2), each as a Background / Solution / Key benefit card:**
1. **Plan Balancing Agent (VD SCM)** — manual Excel SOP planning for THE WALL,
   decisions relying on individual experience → data-transformation
   automation + AI decision support → reduced manual processing time,
   optimized resources, absorbs higher workload without proportional effort.
2. **Training Management Agent (HR Training P)** — manual cross-department
   training-data collection and hour calculation → automated collection +
   AI agent that generates reports with insight → learning-path suggestions
   and SEHC KPI training-hour assurance.

**Project schedule:** build a timeline (native SVG) from the `AX/` folder
files showing each project's progress, functions delivered, and milestones.
Mark clearly what is completed vs in progress as of today.

**Other activities — talkshows (compact cards):**
- *Samsung Agent Builder* — introduction to SEHC colleagues; how to apply
  Agent Builder to enhance work efficiency.
- *Cline SR Kit* — toolkit with 32+ skills; developed and shared to grow
  AI-agent capability.
- Images: `AX/assets/AX_Talk_1.png`, `AX/assets/AX_Talk_2.png`.

---

## Step 5 — Page 4: GrowHive Activity

GrowHive is an **online self-study system to boost employee skills**. Frame
its benefits around the three program goals (started March 2026):
- **Productivity Growth** — project-based training and skill mapping improve
  performance.
- **Collaborative Support** — an environment where all members can
  collaborate and learn from each other.
- **Agility & Resilience** — ability to redeploy people as strategy changes
  or uncertainty demands.

Add a short benefit paragraph in executive language: continuous, self-paced
upskilling; visible skill maps for managers; training aligned to real
projects rather than generic courses.

**Milestone & progress — redraw natively (html-svg-diagrams). The reference
image is `AX/assets/Grow_hive.png`; its content is already extracted below —
use these facts, and consult the image only for layout inspiration:**

Adoption phases:
| Phase | Scope | Period | Status |
|---|---|---|---|
| Project Research | Strategy alignment & first introduction | Q4 2025 | ✅ Completed |
| Project Planning | Define objectives & orientation | Q1 2026 | ✅ Completed |
| Pilot & Full Rollout Plan | Prepare for official deployment | Q2 2026 | 🔄 In progress — **we are here** |
| Production Launching | Launch the official system for all users | Q3 2026 | Planned |

Detailed execution milestones (week numbers of 2026):
| Week | Milestone | Status |
|---|---|---|
| W11 | Linux server request | ✅ Done |
| W19 | Environment ready | ✅ Done |
| W22 | Server set-up & troubleshooting | 🔄 Current position ("we are here") |
| W24 | Pre-deployment | Planned |
| W26 | Completion (ready for production phase) | Planned |

Show a progress indicator (e.g., 3 of 5 execution milestones reached; phase
2.5 of 4). Do not claim Production Launching as done — it is Q3 2026 planned.
You may include the original `Grow_hive.png` as collapsed evidence
("source slide") under the redrawn timeline.

---

## Step 6 — Image rules (AX/assets/)

- Reference by relative path `AX/assets/<filename>` (mind the space-containing
  filenames — URL-encode or quote correctly). Never base64, never external.
- Every image: `figure` + caption + meaningful alt text.
- Thumbnails max-height ~280px, click-to-enlarge lightbox (no library).
- Screenshots with slide chrome/glare: crop via CSS container, don't distort.
- Redraw data/timeline charts natively; screenshots are evidence, collapsed.

---

## Step 7 — Language, tone, design

- Clean professional English; correct source grammar; keep product names
  exact (Cline-SR, Gauss, GaussO Think, Kona, eCODE, Knox, GrowHive).
- Define internal acronyms on first use (AX, SOP, MRO, OSD, SAM, PLM, SCM,
  CIT, SEHC, VD) + glossary in a collapsed appendix.
- Outcome-first executive phrasing; no invented savings or percentages;
  only the numbers present in the sources.
- Style: premium corporate — white / dark navy / deep blue / light gray, one
  accent (the GrowHive section may echo the purple of its branding, subtly).
- Sticky nav across the 4 pages/sections; filters where useful (month filter
  on the Best Practice table); print-friendly; responsive; accessible.
- Single HTML file, embedded CSS/JS, opens directly in a browser.

---

## Final checklist

- [ ] Relevant html-skills SKILL.md files read and followed
- [ ] Page 2 table is clickable with per-project detail + image
- [ ] Cline-SR adoption 76%→100% shown as a headline visual
- [ ] GrowHive timeline redrawn natively with the exact phases/weeks above,
      "we are here" at W22 / Q2 2026, nothing planned shown as done
- [ ] AX folder schedule summarized into a project-progress timeline
- [ ] All images relative-path with caption + alt; missing images reported
- [ ] Acronyms explained; first screen CEO-readable; prints cleanly
