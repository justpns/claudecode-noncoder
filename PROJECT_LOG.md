# Project Evolution & Engineering Log

This log records the structural and functional milestones achieved during the development of the "Claude Code for Non-Coders" repository. It serves as a permanent record of the "AI System" architecture implemented here.

---

## [2026-05-11] Architecture & System Implementation

### 1. Repository Restructuring
*   **Action**: Reorganized the project from a flat file structure into a "Standard AI Workflow" hierarchy.
*   **Directories Established**:
    *   `/slides/`: Hosting the interactive HTML presentation modules.
    *   `/knowledge/`: Dedicated knowledge base for persistent context.
    *   `/roles/`: Repository for specialized AI persona definitions.
    *   `/workflows/`: Repository for Markdown-based Standard Operating Procedures (SOPs).
*   **Rationale**: To align the project's physical structure with the "System vs. Chat" curriculum taught in the modules.

### 2. Knowledge Base Development
*   **`knowledge/MODULES_OVERVIEW.md`**: Created a centralized reference for module objectives and key themes (Cold Start Problem, Inconsistency, Tiered Systems).
*   **`knowledge/STYLING_GUIDE.md`**: Formalized the design system (Bebas Neue/Barlow fonts, hex-code palettes) to maintain visual consistency across all modules.

### 3. System Instructions & Persona
*   **`CLAUDE.md`**: Implemented root-level system instructions that enforce the repository's structural rules and the "Course Assistant" persona for all future AI sessions.
*   **`roles/course-assistant.md`**: Defined a specialized AI persona focused on educational clarity and adherence to the slide content (Anti-Hallucination).

### 4. Workflow Automation
*   **`workflows/generate-study-guide.md`**: Created an automated SOP that allows the AI to analyze module content and generate structured study guides and quizzes on demand.

### 5. Curriculum & UX Enhancements
*   **Module 01 Reversion**: Reverted `module01-slides-final-v2.html` to the state of `module01-slides-final-v2_1.html`.
    *   **Restoration**: Restored the original v2_1 visual design and content structure.
    *   **Continuity**: Manually added the "next →" link to Module 02 at the end of the deck to preserve the course loop.
*   **Module 01: Claude Ecosystem Clarification (Archived)**: (Note: The interactive Surfaces slide from the previous refactor was removed during the reversion to v2_1).
*   **Cross-Module Navigation**: Implemented bidirectional links (Next/Previous) between all four slide modules, creating a continuous learning loop.
*   **CIPHER Soft Demo (Enhanced)**: Expanded the interactive simulation in **Module 02**.
    *   **Deliverables Visualization**: Added an "Asset Grid" showing ready-to-review files (Email, PDF, DOCX).
    *   **Feedback Loop**: Implemented a "Human-in-the-Loop" step simulating critical feedback and automated refinement.
    *   **Final Delivery**: Added a success state showing asset synchronization and mission completion.
    *   **Deliverables Showcase**: Created a dedicated slide to visualize the end products (`EMAIL_DRAFT.md`, `STRATEGY.pdf`, `BUDGET.docx`) with high-fidelity mock previews.
    *   **Architecture**: Reinforced the "Two Decisions" principle (Approve/Refine) through visual UI elements.
*   **Cross-Module Standardization & Refactor**: Audited and refactored all 4 HTML modules for functional parity.
    *   **Navigation Engine**: Implemented a unified `handleNext()` logic across all files to handle both slide transitions and internal interactive steps.
    *   **Event Handling**: Standardized Keyboard (Arrows/Space), Global Click-to-Advance, and Touch gestures across the entire course.
    *   **Layout Synchronization**: Ensured all slides reside within identical `.deck > .slide` containers with synchronized CSS animations and variable sets.

---

## [2026-05-11] Curriculum Expansion & Visual Identity (Phase 2)

### 1. Pedagogical Gap Fixes
*   **Gap 01: Context Hierarchy (Module 01)**: Inserted a new slide (`S04`) distinguishing between *Transient Memory* (Chat) and *Persistent Memory* (Workspace Files). Includes a visual "Brain Memory Zones" SVG.
*   **Gap 02: Terminal Control Room (Module 02)**: Added an empathy-focused reframe slide (`S02`) that contrasts "The Messy Desk" (Browser chaos) with "Mission Control" (Terminal centralized cockpit).
*   **Gap 03: System Evolution Model (Module 04)**: Implemented a maturity model slide (`S11`) that maps a student's journey from a Solo Operator (Day 1) to a Full Team/CIPHER architecture (Year 1).

### 2. Signature Visual Language (Hero SVGs)
Standardized the visual narrative across all modules by implementing high-fidelity "Hero SVGs" on every title slide:
*   **M01: The Hamster Wheel (Enhanced)**: Added "New Chat" nodes and curved `textPath` typography to emphasize repetitive failure.
*   **M02: The Blueprint**: Created an architectural floor plan of the workspace folders.
*   **M03: The Engine**: Visualized the workflow pipeline as an interlocked mechanical engine (Scout → Forge → Shade → Proxy).
*   **M04: The Factory**: Demonstrated industrial scaling with three parallel engine lines feeding into a central knowledge base.

### 3. System Integrity & Maintenance
*   **Slide Count Synchronization**: Updated all hardcoded slide counters and internal interactive demo indices (M01=13, M02=16, M03=15, M04=13).
*   **Standardization Maintenance**: Verified that all new slides adhere to the unified `handleNext()` navigation engine and CSS variable standards.

---

## [2026-05-13] Curriculum Expansion & Evolution Model

### 1. Pedagogical Evolution
*   **Evolution Path (Module 01)**: Inserted a new slide mapping the industry shift from **Single Prompting** (Stage 1) to **Workflows** (Stage 2) and finally to **Agents** (Stage 3).
*   **Context**: Based on the evolution model described by Thariq Shihipar (Anthropic). This slide serves as the bridge between identifying "gaps" in chat AI and introducing the "system" solution.
*   **Visuals**: Implemented a vertical evolution SVG model showing the progression of autonomous agency.
*   **Sub-Agent Context Management (Module 02)**: Added a slide ("CONTEXT FILLS UP. SUB-AGENTS DON'T.") explaining how sub-agents protect the main agent's context window. Included Thariq Shihipar's quote on context management.
*   **Agent Verification (Module 04)**: Inserted a new slide ("3 QUESTIONS. BEFORE YOU BUILD.") outlining the three core pillars of agent readiness: Context, Action, and Verification.

### 2. System Integrity
*   **Slide Count Synchronization**: Updated Module 01 slide counter to 13 (Total), Module 02 slide counter to 17 (Total), and Module 04 slide counter to 14 (Total).
*   **Navigation**: Verified the new slides integrate seamlessly into the global advancement logic.

---
**Engineering Standard**: Every curriculum update must include both a conceptual bridge (why it matters) and a visual anchor (how it's remembered).
