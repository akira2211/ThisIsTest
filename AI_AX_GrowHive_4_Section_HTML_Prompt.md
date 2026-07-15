# Prompt: Create a Single-File Interactive HTML Presentation

## Goal

Create one standalone HTML file that behaves like an interactive PowerPoint presentation.

The HTML must contain exactly four primary full-screen sections:

1. AI Utilization
2. AI Best Practice
3. AX Activity
4. GrowHive Activity

Users must be able to move between sections like slides.

Navigation methods:

- Previous / Next buttons
- Keyboard Left / Right arrows
- Keyboard Page Up / Page Down
- Mouse wheel
- Touch swipe on mobile or tablet
- Clickable section indicators
- Optional clickable table of contents

Do not create four separate HTML pages.

Do not create a long scrolling website.

Create one HTML document with four slide-like sections.

---

# Audience

The report is designed for:

- CEO
- Top executives
- Department leaders
- Technical leaders

The first view of every section must communicate the main message clearly without requiring the viewer to read technical details.

---

# Main Executive Story

Use the following central message:

> The organization is progressing from AI tool adoption to practical AI transformation by combining daily engineering usage, reusable best practices, cross-functional AX projects, and continuous workforce development through GrowHive.

The four sections represent one connected journey:

```text
AI Utilization
      ↓
AI Best Practice
      ↓
AX Activity
      ↓
GrowHive
```

Interpretation:

- AI Utilization builds adoption.
- AI Best Practice turns usage into reusable solutions.
- AX Activity applies AI to real business and operational problems.
- GrowHive develops sustainable skills and workforce capability.

---

# Global Presentation Behavior

## Slide Layout

Each primary section must:

- Fill the browser viewport
- Use `min-height: 100vh`
- Fit key content within one screen on a standard presentation display
- Allow an internal detail panel or modal for extra information
- Avoid forcing the audience to scroll through long text
- Use concise executive summaries
- Use expandable cards for detailed information

## Slide Navigation

Add fixed navigation controls:

- Previous button
- Next button
- Current slide number
- Four clickable navigation dots
- Section title indicator
- Home or overview button

Example:

```text
← Previous      2 / 4      Next →
```

Navigation dots:

```text
●  ○  ○  ○
```

The active section must be clearly highlighted.

## Transitions

Use smooth, professional transitions:

- Horizontal slide movement
- Fade and subtle scale
- Duration between 400 and 700 milliseconds
- No playful or distracting animation
- Avoid excessive parallax

## Keyboard Controls

Support:

- ArrowRight: next section
- ArrowLeft: previous section
- PageDown: next section
- PageUp: previous section
- Home: first section
- End: last section
- Escape: close modal or detail panel

## Touch Controls

Support horizontal swipe:

- Swipe left: next section
- Swipe right: previous section

## Mouse Wheel

A deliberate wheel gesture may move to the next or previous section.

Prevent multiple section jumps from one wheel action by applying a short navigation lock.

## Progress Indicator

Show a thin progress bar at the bottom or top.

Example:

- Section 1: 25%
- Section 2: 50%
- Section 3: 75%
- Section 4: 100%

---

# Visual Direction

Use a premium corporate technology-presentation style.

## Design Characteristics

- Executive
- Modern
- Clean
- Innovative
- High readability
- Strong visual hierarchy
- Suitable for large-screen presentation
- Responsive for desktop and tablet
- Print-friendly where possible

## Color System

Use a coherent palette:

- Dark navy
- Deep blue
- Purple
- Teal accent
- White
- Light gray

Suggested section accents:

- AI Utilization: Blue
- AI Best Practice: Purple
- AX Activity: Teal
- GrowHive: Violet

Avoid excessive gradients.

## Typography

Use:

- Large section titles
- Large KPI numbers
- Short supporting text
- Clear subtitles
- Compact detail cards
- Strong contrast

Use system-safe fonts or embedded web-safe fonts.

---

# Section 1 — AI Utilization

## Section Objective

Show how AI adoption progressed from initial usage to full engineering participation.

## Main Headline

> From AI Tool Introduction to Daily Engineering Practice

## Executive Summary

Use a concise message:

> Starting in March 2026, the organization encouraged engineers to apply Cline-SR in real development work. Adoption grew from 129 of 170 users, approximately 76%, to full participation by June. Monthly AI Best Practice activities reinforced adoption by rewarding practical solutions and sharing reusable knowledge.

## KPI Cards

Show:

- March adoption: 129 / 170 users
- March adoption rate: approximately 76%
- June adoption rate: 100%
- Best Practice projects: 11
- Program period: March to June 2026

Do not invent April or May adoption percentages.

## Cline-SR Introduction

Describe Cline-SR as an AI-based coding assistant.

Capabilities:

- Code analysis
- Code generation
- Agent-based coding
- Defect analysis
- Refactoring
- Structural improvement
- Specification analysis
- Algorithm improvement

## Images

Use:

- `AX/assets/Cline_SR_1.png`
- `AX/assets/Cline_SR_2.png`
- `AX/assets/AI_Utilization_1.png`
- `AX/assets/AI_Utilization_2.png`

Recommended arrangement:

- Left side: executive text and KPI cards
- Right side: image gallery or stacked screenshots

Allow image zoom in a modal.

## Adoption Visualization

Create:

- March donut chart: 76%
- June progress ring or progress bar: 100%
- Simple March-to-June timeline

Do not invent intermediate values.

## AI Best Practice Monthly Trend

Data:

- March: 2 projects
- April: 5 projects
- May: 3 projects
- June: 1 project

Display:

- Compact bar chart
- Total: 11 projects
- Monthly reward and sharing mechanism

## Process Diagram

```text
Real Engineering Problem
        ↓
AI-Based Solution
        ↓
Internal Demonstration
        ↓
Best Practice Review
        ↓
Reward and Sharing
        ↓
Reuse Across Teams
```

## Final Message

> AI adoption has progressed from optional tool usage to an organization-wide engineering practice supported by measurable participation and practical reuse.

---

# Section 2 — AI Best Practice

## Section Objective

Present the monthly AI Best Practice portfolio in an interactive and visually compact format.

Do not show all details at once.

The main slide should show:

- Monthly tabs
- Project cards
- Project count
- Category filters
- Click-to-open details

## Portfolio Summary

Show:

- March: 2 projects
- April: 5 projects
- May: 3 projects
- June: 1 project
- Total: 11 projects

## Interaction

Use month tabs:

```text
March | April | May | June
```

When a month is selected, show its project cards.

When a project card is clicked, open a modal or side drawer containing:

- Introduction
- Background
- Problem
- Solution
- Workflow
- Benefits
- Metrics
- Image
- Status
- Category

## March Projects

### E-Paper Application AI Function PoC

Category:

- Generative AI
- Content Creation
- User Experience

Summary:

AI-powered handwritten-content conversion and content generation for Flip or e-paper use cases.

Capabilities:

- Text to image
- Voice to image
- Image to image
- Handwriting recognition
- Translation
- Digital-content conversion

Introduction:

> AI Handwritten Converter transforms handwritten content on Flip screens into clear digital text using AI-powered recognition and translation, making information easier to read, share, and preserve.

Image:

- `AX/assets/E-Paper Application AI function PoC.png`

Benefits:

- Better readability
- Easier content reuse
- Faster digital conversion
- Improved collaboration

### AI Document Automatic Creation Tool

Category:

- Workflow Automation
- Defect Management
- LLM Integration

Introduction:

> A developer enters a defect ID through the SEHC Chatbot. The backend collects Kona and PLM information, Samsung Gauss analyzes the data, and the system creates a structured issue automatically in eCODE.

Workflow:

```text
Defect ID
    ↓
SEHC Chatbot
    ↓
Kona and PLM Data Collection
    ↓
Samsung Gauss Analysis
    ↓
Structured Summary
    ↓
Automatic eCODE Creation
```

Benefits:

- Reduced manual documentation
- Better consistency
- Faster defect handling
- Improved data accuracy

Image:

- `AX/assets/AI document automatic creating tool.png`

## April Projects

### Cline Kit

Category:

- Developer Productivity
- Reusable AI Assets
- Engineering Standardization

Metrics:

- 61 skills
- 8 rules
- 5 workflows

Introduction:

> A modular kit-management system for Cline containing reusable rules, skills, workflows, and hooks, installable through Web UI or CLI.

Benefits:

- Faster AI onboarding
- Reusable engineering knowledge
- Standardized development workflows
- Easier sharing across teams

### AI-Powered SAM Analysis Report with Gauss

Category:

- Technical Analysis
- Troubleshooting
- Automated Reporting

Problem:

- SAM reports are difficult to read
- Root-cause analysis requires significant time
- Report quality varies by reviewer

Solution:

> Gauss AI analyzes SAM reports and creates structured HTML reports with error interpretation, root-cause guidance, and troubleshooting recommendations.

Verified benefit:

- Analysis time reduced from several hours to minutes

Other benefits:

- Consistent report format
- Clearer guidance
- Step-by-step recommendations

Do not claim accuracy improvement unless verified.

### Screen Extractor

Category:

- OCR
- Test Automation
- Multilingual Verification

Background:

- Testers manually compare OSD text with multilingual Excel data
- Many languages make checking difficult
- Manual comparison is slow

Solution:

> Capture the PC screen or TV display through a webcam, recognize displayed text, highlight detected regions, and export selected content to Excel.

Capabilities:

- PC screen capture
- Webcam capture
- OCR detection
- Highlight boxes
- Excel export
- Support for 33 Flip languages
- Easy language extension

Benefits:

- Faster multilingual verification
- Less manual comparison
- Better consistency

### Asset Management System

Category:

- Business Process Automation
- Asset Governance
- LLM Data Extraction

Introduction:

> A centralized asset-management platform replacing manual email-based MRO purchasing. An LLM extracts invoice information, triggers workflows, and synchronizes with the intranet for asset tracking.

Benefits:

- Reduced manual processing
- Better asset and cost visibility
- Faster requests
- Improved governance

### Monitor AI Cline Skills

Category:

- Embedded Development
- AI Engineering Assistant
- Defect Resolution

Introduction:

> An AI-assisted development framework for the Samsung LEMON 2026 Display Monitor project.

Purposes:

- Automate routine tasks
- Improve code quality
- Accelerate defect resolution
- Integrate with PLM
- Standardize workflows
- Improve developer productivity

## May Projects

### Release Automation Tool

Category:

- CI/CD Automation
- Release Engineering
- Developer Productivity

Scope:

- Version update
- Git operations
- CI/CD monitoring
- APK signing
- Galaxy deployment
- Release documentation

Benefits:

- Fewer manual steps
- Reduced release errors
- Faster release execution
- Better consistency

### PM Onboard AI Assistant

Category:

- Knowledge Assistant
- Employee Onboarding
- Self-Service Support

Introduction:

> An AI assistant helping new employees understand company processes, setup guides, onboarding information, and team knowledge.

Benefits:

- Faster onboarding
- Reduced mentor workload
- Fewer repetitive questions
- Easier Confluence search
- Better self-service support

### AI-Powered Carry-in Document Creation via Cline Skills

Category:

- Process Automation
- Document Generation
- Logistics Support

Background:

- Vendors provide four days of free storage
- Delayed document preparation may create extra cost
- The process depends on email, invoices, and portals

Solution:

> Cline acts as an orchestrator, collects carry-in emails, processes text or image invoices, calls Knox and intranet APIs, and generates CIT and Carry-In Excel files.

Benefits:

- Faster preparation
- Reduced manual coordination
- Lower delay risk
- Better consistency

Do not claim actual cost savings without evidence.

## June Project

### Decision Manager

Category:

- GraphRAG
- Knowledge Management
- Decision Intelligence

Background:

- Important decisions in chat and email are difficult to retrieve
- Manual search takes 30 to 60 minutes
- Source provenance is difficult to verify

Solution:

> A desktop application indexing Samsung chat and email exports and answering natural-language questions using GraphRAG, a local ONNX embedding model, and Samsung GaussO Think.

Capabilities:

- Index `.mht` and `.eml`
- Extract people, topics, and decisions
- Build a knowledge graph
- Natural-language query
- Source citations
- Secondary AI verification

Verified impact:

- Decision lookup reduced from 30–60 minutes to less than 30 seconds
- Answers cite exact sources, participants, and timestamps

## Filters

Support:

- Month
- Category
- Business function
- PoC / Completed / Ongoing
- With image / Without image

## Main Slide Layout

Recommended:

- Top: monthly summary and project count
- Left: month tabs and category filter
- Center: project-card grid
- Right or modal: selected project details

---

# Section 3 — AX Activity

## Section Objective

Show how AI and automation capabilities are applied to real business operations outside normal software development.

## Main Headline

> Extending AI Capability into Business Operations

## Executive Summary

> AX activities apply AI agents, automation, and data transformation to real departmental problems. The current focus includes SCM planning and HR training management, supported by knowledge-sharing activities that help more teams adopt AI effectively.

## KPI Cards

Show:

- Major supported projects: 2
- Knowledge-sharing talkshows: 2
- Main business areas: SCM and HR Training
- Main technology pattern: Automation plus AI Agent

## Project 1 — Plan Balancing Agent

Business area:

- VD SCM

Background:

- SOP plans for THE WALL are manually adjusted in Excel
- Decisions depend heavily on individual experience
- Manual analysis is time-consuming

Solution:

> Create an AI-assisted planning solution that automates data transformation and provides decision support for plan balancing.

Capabilities:

- Excel data collection
- Data transformation
- Plan comparison
- AI recommendations
- Resource-balancing support
- Scenario analysis
- Report generation

Benefits:

- Reduced manual planning
- Better consistency
- More scalable workload handling
- Improved resource allocation
- Lower dependence on individual experience

Do not invent exact time savings.

## Project 2 — Training Management Agent

Business area:

- HR Training

Background:

- Training data is manually collected across departments
- Preprocessing and training-hour calculation are time-consuming
- Managers need clearer insight

Solution:

> Build an automated collection and management system with an AI agent that summarizes results, tracks KPI progress, and recommends learning paths.

Capabilities:

- Department data collection
- Data preprocessing
- Training-hour calculation
- AI-generated summary
- KPI tracking
- Learning-path recommendation
- Manager dashboard

Benefits:

- Reduced manual reporting
- Better training visibility
- Faster KPI monitoring
- More useful learning recommendations

## Timeline

Read schedule information from files under the `AX` folder.

Exclude the `assets` folder when reading schedule documents.

Create one compact visual timeline per project.

Suggested phases:

```text
Discovery
   ↓
Requirement Analysis
   ↓
Data Integration
   ↓
Agent Development
   ↓
Validation
   ↓
Pilot
   ↓
Deployment
```

For each project show, when supported by source data:

- Planned functions
- Completed functions
- In-progress functions
- Upcoming functions
- Current phase
- Major milestones

Do not calculate percentages without a verified task count.

## Knowledge-Sharing Talkshows

### Samsung Agent Builder

Purpose:

- Introduce Samsung Agent Builder
- Demonstrate practical applications
- Explain how AI agents improve efficiency
- Encourage wider adoption

### Cline-SR Kit

Purpose:

- Introduce reusable Cline-SR skills
- Share development assets
- Improve agent capability
- Promote reuse

Use the value of more than 32 skills only in this talkshow context.

Do not merge it with the separate Cline Kit value of 61 skills unless the source confirms they are the same version.

Images:

- `AX/assets/AX_Talk_1.png`
- `AX/assets/AX_Talk_2.png`

## AX Process Diagram

```text
Business Problem
      ↓
Data Collection
      ↓
Automation
      ↓
AI Agent
      ↓
Decision Support
      ↓
Operational Improvement
```

## Main Slide Layout

Recommended:

- Left: project selector
- Center: selected project's problem, solution, and benefits
- Bottom: project timeline
- Right: talkshow image gallery
- Details shown through modal or expandable drawer

## Final Message

> AX activities demonstrate how engineering capability can improve planning, training, and other operational processes across the organization.

---

# Section 4 — GrowHive Activity

## Section Objective

Present GrowHive as a strategic workforce-capability platform.

Do not present it only as an online learning website.

Use the supplied image:

- `AX/assets/Grow_hive.png`

Use the image as a schedule reference, but redesign it into a modern interactive roadmap.

## Main Headline

> Building a Future-Ready Engineering Workforce

## Executive Summary

> GrowHive is an online self-learning and workforce capability platform designed to improve engineering skills, strengthen collaboration, accelerate onboarding, and increase organizational agility.

## Strategic Benefit Cards

### Productivity Growth

Description:

Project-based training, structured learning paths, and skill mapping help engineers build practical capability and improve performance.

Potential outcomes:

- Faster skill development
- Reduced learning curve
- Better project readiness
- Stronger technical capability
- Improved onboarding

### Collaborative Support

Description:

Create an environment where members learn together, share knowledge, exchange best practices, and reuse internal expertise.

Potential outcomes:

- Better knowledge sharing
- Stronger collaboration
- Reusable learning assets
- Cross-team support
- Community learning

### Agility and Resilience

Description:

Improve the organization's ability to redeploy employees, respond to strategic changes, adopt new technology, and manage uncertainty.

Potential outcomes:

- Faster skill redeployment
- Better technology adaptation
- Future-ready workforce
- Reduced capability gaps
- Stronger organizational resilience

## GrowHive Roadmap

Create an interactive horizontal roadmap.

### Phase 1 — Project Research

Period:

- Q4 2025

Activities:

- Strategy alignment
- First introduction
- User research
- Initial concept definition

Status:

- Completed

### Phase 2 — Project Planning

Period:

- Q1 2026

Activities:

- Define objectives
- Define orientation
- Plan system structure
- Prepare infrastructure
- Define learning and skill model

Status:

- Completed

### Phase 3 — Pilot and Full Rollout Plan

Period:

- Q2 2026

Activities:

- Prepare official deployment
- Validate the environment
- Conduct pilot activities
- Resolve infrastructure issues
- Prepare users and content

Status:

- Current phase

Highlight:

> We are here

### Phase 4 — Production Launch

Period:

- Q3 2026

Activities:

- Launch the official system
- Enable organization-wide usage
- Monitor adoption
- Improve learning content and operation

Status:

- Upcoming

## Milestones

### Week 11

- Linux Server Request
- Status: Completed

### Week 19

- Environment Ready
- Status: Completed

### Week 22

- Server Setup and Troubleshooting
- Status: Current

### Week 24

- Pre-deployment
- Status: Upcoming

### Week 26

- Completion
- Status: Upcoming

## Progress Cards

Show:

- Current phase: Pilot and Rollout Preparation
- Current milestone: Server Setup and Troubleshooting
- Completed milestones: 2
- Current milestones: 1
- Upcoming milestones: 2
- Target launch: Q3 2026
- Platform type: Online Self-Learning

Do not show an overall percentage unless supported by verified task data.

## Capability Map

```text
GrowHive
   ├── Learning Paths
   ├── Skill Mapping
   ├── Project-Based Training
   ├── Self-Learning Content
   ├── Knowledge Sharing
   ├── Progress Tracking
   ├── Community Collaboration
   └── Workforce Readiness
```

## User Journey

```text
Engineer Joins
      ↓
Skill Assessment
      ↓
Recommended Learning Path
      ↓
Self-Learning
      ↓
Project-Based Practice
      ↓
Progress Review
      ↓
Knowledge Sharing
      ↓
Capability Growth
```

## Recommended Future Features

Show these only as proposed or planned unless confirmed as implemented:

- Skill profiles
- Role-based learning paths
- Project-based curriculum
- AI learning recommendations
- Progress dashboard
- Peer learning
- Mentor support
- Best Practice library
- Badge or certification system
- Manager capability dashboard
- Learning analytics
- Internal content search

Clearly label each feature as:

- Existing
- Planned
- Recommended

## Main Slide Layout

Recommended:

- Top left: GrowHive title and executive summary
- Top right: strategic benefit cards
- Center: interactive roadmap
- Bottom: capability map and milestone progress
- Detail drawer: user journey and future features

## Final Message

> GrowHive is more than a learning platform. It is a strategic capability system that helps the organization build skills, share knowledge, redeploy talent, and prepare engineers for future technology and business needs.

---

# Optional Overview Menu

Before entering Section 1, an optional lightweight menu may appear.

It must not count as a fifth primary slide.

Menu content:

- AI Utilization
- AI Best Practice
- AX Activity
- GrowHive

When the user selects an item, jump directly to that section.

The menu can be opened at any time through a small home button.

---

# Detail Handling

The four main sections must stay presentation-friendly.

Move long content into:

- Modal dialogs
- Slide-in drawers
- Expandable cards
- Tooltips
- Image lightboxes

Do not overload the main screen.

---

# Image Rules

Use these paths:

## AI Utilization

- `AX/assets/Cline_SR_1.png`
- `AX/assets/Cline_SR_2.png`
- `AX/assets/AI_Utilization_1.png`
- `AX/assets/AI_Utilization_2.png`

## AI Best Practice

- `AX/assets/E-Paper Application AI function PoC.png`
- `AX/assets/AI document automatic creating tool.png`

## AX Activity

- `AX/assets/AX_Talk_1.png`
- `AX/assets/AX_Talk_2.png`

## GrowHive

- `AX/assets/Grow_hive.png`

Rules:

- Preserve aspect ratio
- Do not stretch
- Add captions
- Use rounded containers
- Add image zoom
- Show a graceful placeholder when missing

---

# Data Accuracy Rules

1. Do not invent metrics.
2. Preserve verified values exactly.
3. Distinguish exact and approximate values.
4. Do not invent intermediate monthly adoption values.
5. Do not calculate progress percentages without verified task counts.
6. Do not combine metrics from different toolkit versions.
7. Clearly label PoC, pilot, ongoing, planned, and completed work.
8. Do not claim cost savings without evidence.
9. Do not claim accuracy improvement without evidence.
10. Correct grammar while preserving the original meaning.

---

# Technical Output Requirements

Generate:

1. One standalone HTML file
2. Four full-screen primary sections
3. Embedded CSS
4. Embedded JavaScript
5. No external runtime dependency
6. Responsive presentation layout
7. Keyboard navigation
8. Mouse-wheel navigation
9. Touch-swipe navigation
10. Previous and Next buttons
11. Navigation dots
12. Section progress indicator
13. Modal or drawer details
14. Accessible semantic HTML
15. Keyboard-accessible interactions
16. Print-friendly fallback
17. Graceful missing-image handling

The HTML must open directly in a browser.

---

# HTML Anything Guidance

Use the selected HTML Anything skill as the primary visual and implementation standard.

Follow the selected skill's:

- Typography
- Layout system
- Spacing
- Card design
- Chart style
- Visual hierarchy
- Interaction patterns
- Responsive behavior

Do not create a generic Bootstrap dashboard.

Do not create four separate pages.

Do not create a long scrolling report.

Implement a single HTML presentation with four navigable sections.

---

# Final Quality Checklist

Before finishing, verify:

- There is only one HTML file.
- There are exactly four primary sections.
- Navigation behaves like a PowerPoint presentation.
- The four sections tell one transformation story.
- Section 1 shows AI adoption.
- Section 2 includes all 11 Best Practice projects.
- Section 3 explains both AX projects and talkshows.
- Section 4 presents GrowHive as a capability platform.
- GrowHive milestones match the supplied image.
- The current GrowHive milestone is highlighted.
- No metric is invented.
- Long details are hidden in modals or drawers.
- The first view of every section is understandable to a CEO.
- The presentation works with keyboard, mouse, and touch.
