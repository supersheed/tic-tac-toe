# Research Workflow

You are executing a deep research task on the following topic: **$ARGUMENTS**

## Step 1 — Clarify Before Researching

Before doing any research, ask the user these questions in a single message:

1. **Scope** — How broad or narrow? (overview vs. deep dive into a specific aspect)
2. **Audience** — Who is this for? (technical experts, general audience, executives, personal reference)
3. **Specific angles** — Any particular questions, subtopics, or perspectives to prioritize?
4. **Depth** — How much detail? (quick ~500 words / standard ~1000 words / comprehensive ~2000+ words)
5. **Format** — Any sections to include or exclude? (e.g., add FAQ, skip executive summary)

If $ARGUMENTS is blank, first ask what topic to research.

Wait for the user's answers before continuing.

---

## Step 2 — Plan

Based on answers, briefly outline:
- Research approach and angles to cover
- Report structure
- Estimated number of sources

Then proceed immediately to Step 3.

---

## Step 3 — Research

Use WebSearch and WebFetch to gather information:
- Run 3–5 targeted searches covering different angles
- Fetch full content from the most relevant, credible sources
- Prioritize recent and authoritative sources
- Note publication dates

---

## Step 4 — Write the Report

Structure:
- **Title:** Research Report: [Topic]
- **Date:** [today's date]
- **Audience:** [from clarification]
- **Executive Summary** — 3–5 bullet points of most important findings
- **Background** — Brief context
- **Key Findings** — Main insights organized by theme, using bullet points and subheadings
- **Deep Dive** — Detailed analysis of specific angles the user requested
- **Implications** — Why this matters; what to watch for
- **Sources** — Numbered list with title, URL, and date accessed

---

## Step 5 — Save the Report

Save to: `output/<slugified-topic>-report.md`
- Slugify: lowercase, replace spaces and special characters with hyphens
- Example: "AI in Healthcare 2025" → `output/ai-in-healthcare-2025-report.md`

---

## Step 6 — Close Out

Provide:
- **Summary:** 2–3 sentences on what was researched and delivered
- **Feedback:** Notes on source quality, gaps, or caveats
- **Score:** Rate research quality and completeness out of 10 with brief justification
