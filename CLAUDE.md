# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains documentation for a vision document project focused on the C- and D-clusters of the HBO Bedrijfskunde (Business Administration) program. The project aims to develop a comprehensive vision document that defines the educational philosophy and design principles for year 2 of the program.

**Project Name:** Visie C- en D-cluster HBO Bedrijfskunde (Vision for C- and D-clusters HBO Business Administration)

## Document Structure

### Key Documents

1. **starting-doc.md** - Main project proposal document that outlines:
   - The rationale for developing a vision for C- and D-clusters
   - Two core questions: WHY (unique contribution) and HOW (design principles)
   - C-cluster: Transition from propedeuse to AD-level (5 learning outcomes)
   - D-cluster: Internship phase (4 days practice + 1 study day)
   - Project approach in 4 phases: deepening, vision development, validation, and follow-up

2. **eindkwalificaties-prop-ad.md** - Competency framework defining learning outcomes (LUKs):
   - LUK1: Analyzing and diagnosing business issues
   - LUK2: (Re)designing business processes with focus on value creation
   - LUK3: Guiding business change processes
   - LUK4: Evaluating process and results
   - LUK5: Developing as a business professional
   - Each LUK shows progression across three levels: Propedeuse, AD-niveau, Bachelor-niveau

## Tools and Technology

**Quarto** is installed for document creation and rendering:

- Version: 1.6.40
- Use `quarto preview <file.qmd>` to preview documents
- Use `quarto render <file.qmd>` to render documents

## Context and Domain

**Educational Level:**

- Propedeuse: First year, foundational level
- AD-niveau: Associate Degree level (between propedeuse and bachelor)
- Bachelor-niveau: Full bachelor degree level

**Focus Areas:**

- The C-cluster covers 5 learning outcomes (LUK1-5) representing the complete business administration action cycle
- The D-cluster is an internship with research component
- Key themes: competency development, work-integrated learning, professional identity formation

**Important Concepts:**

- Bedrijfskundige handelingscyclus: Business administration action cycle (analyze → design → guide → evaluate)
- Four business domains: strategy, operations, information management, organizational behavior
- Meervoudige waarden: Multiple values (social, environmental, economic)
- Moreel kompas: Moral compass

## Document Development Workflow

When working on vision documents:

1. Consider the progression from propedeuse → AD-niveau → Bachelor-niveau
2. Maintain focus on the WHY (contribution to professional development) and HOW (design principles)
3. Ensure alignment with the 5 learning outcomes (LUKs)
4. Consider practical implementation aspects (teaching methods, assessment, internship structure)

## Content Creation Protocol

**CRITICAL:** When the user requests content creation for a specific section or chapter, follow this mandatory workflow:

### STRICT OUTLINE ADHERENCE

**Rule 1: NEVER add new sections**
- The document structure is FIXED in `startmateriaal/vision-document-outline.md`
- NEVER create new hoofdstukken (##) or major sections (###)
- ONLY add content within existing outline sections
- If content doesn't fit in existing structure, discuss with user first

**Rule 2: ALL questions MUST remain visible**
- Every question from the outline MUST stay in the Quarto document
- Questions are NEVER replaced by content
- Content is added UNDER the questions, not instead of them
- Format:
  ```markdown
  #### [Exact question from outline]

  [Content answering the question]

  **Status:** ✅ Beantwoord | ⏸️ Gedeeltelijk beantwoord | ⏳ Nog open
  **Nog uit te werken:** [Specific aspects still missing]
  ```

**Rule 3: Explicit status tracking**
- ✅ **Beantwoord**: Question fully addressed with sources
- ⏸️ **Gedeeltelijk beantwoord**: Question partly answered, explicitly state what's missing
- ⏳ **Nog open**: `[Uitwerking volgt]` placeholder

**Rule 4: Traceability**
- Each piece of content must clearly indicate which question(s) it answers
- Use cross-references to related sections explicitly
- Cite sources for all factual content

### Step 1: Identify Questions from Outline
ALWAYS start by identifying which questions from `startmateriaal/vision-document-outline.md` are relevant to the requested content section.

### Step 2: Present Questions
Return the complete set of questions from the outline that need to be addressed. Present them clearly to the user for confirmation.

### Step 3: Structure Content Under Questions
For each question from the outline:
- Keep the question visible as a heading
- Add content that addresses the question below it
- Add status indicator
- Explicitly state what remains to be done (if applicable)

### Example Workflow:

**User request:** "Create content for section 2.1 (LUK1)"

**Response:**
1. First, check `startmateriaal/vision-document-outline.md` section 2.1:
   - Questions listed: "Hoe ontwikkelt de student van 'toepassen' naar 'selecteren'?"
   - Sub-topics: Stakeholder-bewustzijn, Theoretische onderbouwing, Complexiteit

2. Present these to the user for confirmation

3. Structure content WITHIN existing outline:
   ```markdown
   #### LUK1: Analyseren en diagnosticeren

   ##### Kernvraag: Hoe ontwikkelt de student van 'toepassen' naar 'selecteren'?

   **Stakeholder-bewustzijn: van vooral intern naar intern én extern**

   [Content addressing stakeholder awareness development]

   **Status:** ⏸️ Gedeeltelijk beantwoord
   **Nog uit te werken:** Concrete voorbeelden van hoe studenten leren externe stakeholders te identificeren

   **Theoretische onderbouwing: van aangereikte modellen naar zelf selecteren relevante theorieën**

   [Content addressing theory selection]

   **Status:** ⏳ Nog open
   ```

### Common Mistakes to AVOID:

❌ Adding new sections like "## De onderzoeksleerlijn" → NOT in outline
❌ Replacing questions with content
❌ Removing `[Uitwerking volgt]` without adding content
❌ Creating subsections not mentioned in outline
❌ Losing track of what questions remain unanswered

✅ Add content under existing questions
✅ Keep all questions visible
✅ Mark status explicitly
✅ State what's still needed

This ensures perfect alignment with `startmateriaal/vision-document-outline.md` and maintains traceability.

## Language

All documentation is in Dutch. When generating or editing content, use Dutch language and maintain professional academic tone appropriate for higher education policy documents.
