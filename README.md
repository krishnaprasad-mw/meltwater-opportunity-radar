## Current Prototype Files

- **Live prototype / GitHub Pages:** `index.html` — now synced to the latest **V11 Teal** build.
- **Archived latest full build:** `Meltwater_Opportunity_Radar_Prototype_Final_v11_Teal.html`.
- **Video-preview compatible standalone build:** `Opportunity_Radar_Standalone_Video_Compatible.html` — no iframe or hosted-page dependency; external font references and embedded logo blobs removed for safer rendering in restricted preview environments.

# Meltwater Opportunity Radar

> **Hackathon prototype:** an AI-powered opportunity intelligence layer that turns Meltwater signals into prioritized opportunities, recommended actions, and measurable activation workflows.

[Live Prototype](https://krishnaprasad-mw.github.io/meltwater-opportunity-radar/) · [Repository](https://github.com/krishnaprasad-mw/meltwater-opportunity-radar)

---

## 1. What is Opportunity Radar?

Meltwater already helps organizations understand what is happening across media, social, creators, competitors, and emerging AI-driven discovery. **Opportunity Radar** explores the next step:

> **Where can the brand win next, why does the opportunity matter, and what should the team do about it now?**

Instead of stopping at monitoring, dashboards, spikes, or reporting, Opportunity Radar is designed as an intelligence and decision layer that:

1. Connects signals from multiple Meltwater intelligence sources.
2. Detects patterns that may represent a commercial, communications, content, creator, or competitive opportunity.
3. Scores and ranks those opportunities by relevance, urgency, brand fit, evidence, and timing.
4. Explains why the opportunity has been surfaced.
5. Converts the insight into a recommended action plan.
6. Tracks activated opportunities and their early impact.
7. Captures human feedback so the engine can improve over time.

The prototype is intentionally designed to feel like a natural extension of the **Meltwater Suite**, rather than a separate standalone tool.

---

## 2. The problem

Modern communications and marketing teams have access to more intelligence than ever, but they still spend significant time manually connecting signals across different workflows.

A team may separately identify:

- a spike in media coverage,
- a shift in social sentiment,
- a competitor receiving criticism,
- an emerging audience question,
- a creator gaining momentum,
- a gap in generative-AI visibility,
- or an under-served content topic.

The difficult part is not always discovering these signals. The difficult part is answering:

- **Is this actually an opportunity?**
- **How important is it compared with everything else happening?**
- **Why is the engine recommending it?**
- **How quickly do we need to act?**
- **Which channel or play should we use?**
- **What happens after we act?**
- **Did the opportunity create measurable impact?**

Opportunity Radar is intended to reduce that decision gap.

---

## 3. The solution

Opportunity Radar acts as a cross-channel opportunity intelligence engine.

### Conceptual flow

```text
Meltwater Intelligence Signals
        ↓
Signal Fusion
        ↓
Opportunity Detection
        ↓
AI Scoring & Ranking
        ↓
Reasoning + Evidence
        ↓
Prioritized Opportunity
        ↓
Action Plan
        ↓
Activated Opportunity
        ↓
Impact Monitoring
        ↓
Human Feedback / Learning Loop
```

The key shift is from:

**“Here is what is happening.”**

to:

**“Here is where you may have an opportunity, why it matters, how strong it is, and what you can do next.”**

---

## 4. Intelligence inputs

The conceptual Opportunity Radar Engine combines signals from several parts of the Meltwater ecosystem.

### Media Intelligence

Potential inputs include:

- coverage velocity,
- emerging narratives,
- journalist interest,
- topic momentum,
- story saturation,
- share of voice,
- sentiment shifts,
- media gaps,
- competitor coverage changes.

### Social Listening

Potential inputs include:

- conversation growth,
- sentiment movement,
- audience questions,
- engagement velocity,
- topic emergence,
- community reactions,
- unmet needs,
- negative or positive spikes.

### Creator Intelligence

Potential inputs include:

- creator momentum,
- emerging creator clusters,
- engagement growth,
- content format performance,
- category whitespace,
- relevant creator-brand fit.

### Competitive Intelligence

Competitive Intelligence was added as an important expansion layer in the prototype. It can help identify:

- competitor weaknesses,
- negative competitor narratives,
- campaign momentum,
- product or positioning gaps,
- share-of-voice changes,
- competitor launches,
- competitor messaging saturation,
- windows where a brand can respond or differentiate.

### GenAI Lens

GenAI Lens signals can expand the engine beyond traditional media and social intelligence by highlighting:

- AI visibility gaps,
- brand mention frequency,
- share of answer,
- citation/source gaps,
- competitor AI visibility,
- prompt-level demand,
- questions where third-party sources dominate,
- opportunities to improve authoritative brand content.

---

## 5. Opportunity types

The prototype currently supports five primary opportunity types.

### 5.1 Emerging Demand

Detects topics, needs, narratives, or audience interests that are accelerating and may create an early-mover opportunity.

**Example signals:**
- rising social conversations,
- increasing search or AI-question demand,
- growing media attention,
- creator momentum.

**Possible action:** move early with content, messaging, product storytelling, or audience engagement.

---

### 5.2 Competitor Weakness

Identifies moments where a competitor is underperforming, receiving criticism, losing narrative ownership, or leaving a positioning gap.

**Example signals:**
- negative competitor coverage,
- sentiment deterioration,
- messaging gaps,
- product criticism,
- declining share of voice.

**Possible action:** reinforce a differentiated proof point without relying on direct competitor attacks.

---

### 5.3 Creator Opportunity

Identifies creators, formats, communities, or themes where audience engagement is growing but brand participation is still limited.

**Example signals:**
- creator engagement growth,
- emerging expert voices,
- underused creator formats,
- high-performing content patterns.

**Possible action:** activate relevant creators or build a new creator-led content series.

---

### 5.4 PR Opportunity

Surfaces timely earned-media openings based on journalist interest, news cycles, coverage gaps, or emerging public conversations.

**Example signals:**
- journalist activity,
- category news momentum,
- under-covered questions,
- spokesperson relevance,
- event-driven narratives.

**Possible action:** create a rapid-response story package, pitch angle, data story, or spokesperson opportunity.

---

### 5.5 Content Whitespace

Detects areas where audience interest is high but useful, authoritative, or differentiated content is limited.

**Example signals:**
- fragmented coverage,
- repeated audience questions,
- weak owned-content visibility,
- GenAI citation gaps,
- competitor content saturation.

**Possible action:** create an authoritative content hub, explainer, FAQ, evidence page, or category resource.

---

## 6. Opportunity scoring

Every opportunity in the prototype is presented with an **Opportunity Score**.

The production concept could combine dimensions such as:

| Dimension | Purpose |
| --- | --- |
| Signal strength | How strongly is the opportunity appearing across channels? |
| Momentum | Is the signal accelerating or declining? |
| Brand fit | How relevant is the opportunity to the brand? |
| Competitive advantage | Is there a credible gap the brand can exploit? |
| Evidence quality | How many reliable signals support the recommendation? |
| Urgency | How quickly could the window close? |
| Potential reach | How large could the audience or impact be? |
| Actionability | Can the team realistically respond? |

The current prototype uses **simulated opportunity scores** for demonstration. It does not run a production scoring model.

---

## 7. Prototype workflow

The prototype demonstrates the complete journey from discovery to activation.

### Step 1 — Radar

The **Radar** page is the starting point.

It provides:

- brand-level opportunity monitoring,
- live-style signal indicators,
- opportunity ranking,
- opportunity scores,
- opportunity summaries,
- source signal indicators,
- filtering by opportunity type,
- filtering by timeframe.

#### Opportunity Type filter

Users can filter to:

- All Opportunities
- Emerging Demand
- Competitor Weakness
- Creator Opportunity
- PR Opportunity
- Content Whitespace

Selecting a type immediately updates the opportunity panel to show only relevant opportunities.

#### Timeframe filter

The prototype supports:

- **Live**
- **Last 7 days**
- **Last 30 days**

The timeframe changes the analytical context and live-style metrics shown in the Radar.

---

### Step 2 — Opportunity Depth

Clicking an opportunity opens **Opportunity Depth**.

This is designed to answer:

> **Why is this an opportunity?**

The page includes:

- opportunity summary,
- opportunity score,
- urgency,
- brand fit,
- potential reach,
- opportunity window,
- evidence sources,
- key reasons the opportunity was detected,
- recommended play,
- recommended next step.

The purpose is to make AI-generated opportunity recommendations **explainable and reviewable**, rather than presenting only a black-box score.

---

### Step 3 — Human-in-the-loop feedback

A flag control is available at the end of the Opportunity Score area.

Users can give quick feedback through four actions:

#### ✓ Accept
**Relevant opportunity**

The engine correctly identified a useful opportunity.

#### ✎ Refine
**Change assumptions / context**

The opportunity is useful, but the reasoning, framing, classification, or assumptions should be adjusted.

#### ◷ Snooze
**Right idea, wrong timing**

The opportunity is valid but should not be prioritized now.

#### × Dismiss
**Not relevant / weak evidence**

The recommendation is not useful enough for the user.

In the prototype, these responses are stored in browser **LocalStorage**.

In a production system, these signals could become part of a human-in-the-loop learning framework used to:

- evaluate recommendation quality,
- identify false positives,
- adjust ranking,
- personalize opportunity recommendations,
- improve future model training and evaluation.

---

### Step 4 — Action Plan

From Opportunity Depth, the user can convert an opportunity into an **Action Plan**.

The prototype generates a structured plan containing:

- plan name,
- objective,
- owner,
- primary KPI,
- start date,
- end date,
- recommended activities,
- activation steps.

The goal is to reduce the gap between **insight** and **execution**.

Instead of asking users to manually interpret a dashboard and build a plan elsewhere, Opportunity Radar proposes the next actions directly from the detected opportunity.

---

### Step 5 — Activated Opportunities

Once an Action Plan is activated, the workflow moves to **Activated Opportunities**.

This page represents the monitoring layer after an opportunity becomes an active initiative.

It shows:

- active opportunity,
- activation status,
- progress,
- owner,
- primary KPI,
- signal impact,
- next milestone,
- aggregate active-plan metrics,
- early impact indicators.

This creates a closed loop:

```text
Detect → Understand → Decide → Activate → Monitor → Learn
```

---

## 8. Engine Expansion

The **Engine Expansion** sub-tab demonstrates how Opportunity Radar could grow beyond basic media/social signals.

The current concept specifically highlights the combination of:

### GenAI Intelligence

GenAI Lens can provide an additional signal layer for:

- AI visibility,
- prompt demand,
- source/citation gaps,
- competitor recommendation share,
- AI-answer whitespace.

### Competitive Intelligence

Competitive Intelligence can add:

- competitor moves,
- competitor weaknesses,
- positioning gaps,
- campaign momentum,
- share-of-voice changes,
- response windows.

Together, these inputs allow the engine to find opportunities that may not be visible from a single intelligence source.

---

## 9. Multi-brand experience

The prototype includes several preloaded demo brands from different industries:

- **Nike** — apparel / sportswear
- **Tesla** — automotive / EV
- **Netflix** — entertainment / streaming
- **Microsoft** — technology
- **Coca-Cola** — consumer / beverages
- **Boeing** — aerospace

Each brand has:

- its own logo,
- industry context,
- simulated metrics,
- dedicated opportunity set,
- opportunity scores,
- recommended plays,
- evidence sources.

Users can switch between brands directly from the top brand selector.

The prototype also includes an **Add Brand** interaction to demonstrate how additional brand workspaces could be introduced.

---

## 10. Live-style signal simulation

The prototype includes a lightweight live-data simulation to make the experience feel dynamic.

At regular intervals, selected metrics change slightly, including:

- signal volume,
- media velocity,
- social demand,
- creator momentum,
- activated-opportunity progress,
- impact indicators.

This is intended solely for the hackathon demo.

> **Important:** the current prototype is not connected to live Meltwater APIs or production data. The values are simulated and should not be interpreted as actual brand intelligence.

---

## 11. Navigation and Meltwater Suite alignment

Opportunity Radar is positioned as a main Meltwater Suite capability alongside concepts such as:

- Explore
- Monitor
- Analyze
- Engage
- Influence
- GenAI Lens

Within Opportunity Radar, the prototype provides dedicated sub-navigation:

1. **Radar**
2. **Opportunity Depth**
3. **Action Plan**
4. **Activated Opportunities**
5. **Engine Expansion**

The sidebar can be collapsed into a compact icon rail. When collapsed:

- tab icons remain available,
- the main content expands,
- users can restore the full navigation at any time.

The UI uses a Meltwater-inspired visual language with:

- navy navigation,
- teal accents,
- light workspace surfaces,
- compact cards,
- Nunito Sans typography.

---

## 12. Core interactive features

### Brand management
- switch between demo brands,
- display embedded brand logos,
- add a new demo brand.

### Opportunity filtering
- filter by opportunity type,
- filter by timeframe,
- update result counts dynamically.

### Opportunity exploration
- select any opportunity,
- inspect opportunity score,
- review evidence and reasoning,
- view urgency, fit, reach, and timing.

### Human feedback
- Accept,
- Refine,
- Snooze,
- Dismiss,
- save feedback locally.

### Action planning
- generate plan details,
- select owner,
- select KPI,
- edit dates,
- review recommended actions.

### Activation monitoring
- activate plans,
- monitor progress,
- show KPI and signal-impact fields,
- track next milestones.

### Responsive navigation
- collapsible side navigation,
- icon-only collapsed state,
- content expansion when navigation is collapsed.

---

## 13. Technology used in the prototype

The current prototype is deliberately lightweight.

| Technology | Use |
| --- | --- |
| **HTML5** | Application structure |
| **CSS3** | Meltwater-inspired design system, layout, cards, responsive behavior |
| **Vanilla JavaScript** | Navigation, filters, brand switching, action plans, monitoring, feedback |
| **LocalStorage** | Human-feedback history and sidebar state |
| **Nunito Sans** | Prototype typography |
| **Base64-embedded images** | Brand logos inside the single HTML file |
| **GitHub** | Source repository and version hosting |
| **GitHub Pages** | Public prototype hosting |

No frontend framework is required to run the current demo.

---

## 14. What is not implemented yet

The prototype demonstrates the **product experience and workflow**, not a production backend.

The current version does **not** include:

- production Meltwater API integrations,
- live Meltwater customer data,
- authentication or permissions,
- persistent cloud database,
- production opportunity-ranking model,
- LLM inference pipeline,
- real-time event streaming,
- automated competitor entity resolution,
- production monitoring/observability,
- multi-user collaboration,
- backend training pipeline.

These are logical next steps if the concept progresses beyond the hackathon.

---

## 15. Potential production architecture

A production implementation could evolve toward a structure such as:

```text
Meltwater Data Sources
│
├── Media Intelligence
├── Social Listening
├── Creator Intelligence
├── Competitive Intelligence
└── GenAI Lens
        │
        ▼
Signal Normalization + Entity Resolution
        │
        ▼
Cross-Channel Signal Fusion
        │
        ▼
Opportunity Detection
        │
        ├── Trend / anomaly detection
        ├── Competitive gap detection
        ├── Content whitespace detection
        ├── Creator momentum detection
        └── GenAI visibility gap detection
        │
        ▼
Opportunity Ranking & Scoring
        │
        ▼
LLM Reasoning / Evidence Explanation
        │
        ▼
Opportunity Radar UI
        │
        ├── Human feedback
        ├── Action plan
        └── Activation
        │
        ▼
Monitoring + Impact Measurement
        │
        ▼
Feedback / Evaluation / Model Improvement
```

Potential production technologies could include TypeScript/React for the frontend, backend services, Meltwater APIs/data services, Snowflake or equivalent analytical storage, search/vector retrieval, event pipelines, ML ranking models, and LLM orchestration. These are **future implementation options**, not technologies currently used by this prototype.

---

## 16. Human-in-the-loop learning concept

Human feedback is an important part of the Opportunity Radar concept because an opportunity can be technically detectable while still being contextually wrong for a specific brand or team.

A future feedback dataset could contain:

```text
Brand
Opportunity
Opportunity Type
Opportunity Score
Evidence
User Outcome
    ├── Accept
    ├── Refine
    ├── Snooze
    └── Dismiss
Timestamp
Subsequent Action
Observed Impact
```

Over time, this could support:

- ranking evaluation,
- recommendation precision,
- personalization,
- opportunity-type calibration,
- better timing recommendations,
- model retraining,
- quality benchmarking.

---

## 17. Business value

Opportunity Radar is designed to help teams move from intelligence to action more quickly.

### For PR and Communications
- identify earned-media openings earlier,
- find unanswered narratives,
- detect competitor vulnerabilities,
- prioritize spokesperson opportunities.

### For Marketing
- find emerging audience demand,
- identify content whitespace,
- connect intelligence to campaigns,
- prioritize growth opportunities.

### For Social and Creator teams
- detect creator momentum,
- identify relevant communities,
- find emerging content formats,
- activate before themes become saturated.

### For Executives
- reduce information overload,
- show the highest-priority opportunities,
- connect intelligence with action and impact.

### For Meltwater
The concept could create a stronger connective layer across multiple Meltwater capabilities by turning separate intelligence signals into a unified opportunity workflow.

---

## 18. Why this is different from another dashboard

Opportunity Radar is not intended to simply add more charts.

The key product principles are:

### Prioritization
Surface the opportunities that matter most rather than every possible signal.

### Explainability
Show why an opportunity was detected and which evidence supports it.

### Actionability
Recommend a practical next action instead of ending with insight.

### Timing
Make the opportunity window and urgency visible.

### Cross-channel intelligence
Combine signals that may be weak individually but powerful together.

### Closed-loop measurement
Continue the workflow after activation.

### Human learning
Allow users to correct the engine and improve future recommendations.

---

## 19. Prototype data disclaimer

All brand opportunities, scores, metrics, signals, reach estimates, progress values, and impact indicators in this prototype are **simulated demonstration data**.

The prototype is designed to demonstrate:

- user experience,
- interaction patterns,
- product concept,
- opportunity workflow,
- engine logic at a conceptual level.

It should **not** be treated as a source of actual intelligence about the brands included in the demo.

---

## 20. Running the prototype locally

Clone the repository:

```bash
git clone https://github.com/krishnaprasad-mw/meltwater-opportunity-radar.git
```

Open the project directory and launch:

```text
index.html
```

The prototype is self-contained and can run directly in a modern browser.

Because Nunito Sans is loaded through Google Fonts, internet access is useful for the intended typography. The rest of the demo logic and embedded brand images are contained in the HTML.

---

## 21. Live prototype

The GitHub Pages deployment is available at:

**https://krishnaprasad-mw.github.io/meltwater-opportunity-radar/**

---

## 22. Repository structure

```text
meltwater-opportunity-radar/
│
├── index.html     # Complete interactive prototype
└── README.md      # Project documentation
```

The prototype intentionally remains a single HTML deliverable so it is easy to share, host, demo, and iterate during the hackathon.

---

## 23. Suggested next steps

If the concept moves forward, the next stages could be:

1. Connect a limited set of real Meltwater signals.
2. Define a formal opportunity taxonomy.
3. Build transparent scoring criteria.
4. Create a historical opportunity evaluation dataset.
5. Test ranking quality with internal experts.
6. Add production LLM reasoning and evidence grounding.
7. Add user/team personalization.
8. Connect Action Plans with downstream Meltwater workflows.
9. Define impact-attribution metrics.
10. Use human feedback to continuously evaluate and improve recommendations.

---

## 24. Project vision

**Opportunity Radar aims to turn Meltwater from a place where teams understand what is happening into a place where they can also understand where to act next.**

The long-term vision is a cross-suite intelligence layer that continuously answers:

> **What is the opportunity? Why does it matter? What should we do? How quickly should we act? And did it work?**

---

### Hackathon prototype

Built as an interactive concept to demonstrate the end-to-end Opportunity Radar workflow inside a Meltwater-inspired product experience.
