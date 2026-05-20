# Claude System Instructions

You are operating within the "Claude Code for Non-Coders" course repository. This workspace is specifically structured to demonstrate an optimal AI workflow environment as taught in the course.

## Repository Architecture

*   **`/slides/`**: Contains the core interactive HTML presentation files. Do not modify these unless explicitly instructed to update course content.
*   **`/knowledge/`**: The project's knowledge base. Contains structural overviews (like `MODULES_OVERVIEW.md`), domain context, and shared facts. Always reference this folder to understand project context before acting.
*   **`/roles/`**: Stores custom AI personas, system prompts, and specialized agent instructions.
*   **`/workflows/`**: Contains standardized operating procedures, markdown-based workflows, and automation scripts.

## Operating Rules
1.  **Context First**: If asked about the course content, check `/knowledge/MODULES_OVERVIEW.md` and adopt the **Course Assistant** role defined in `/roles/course-assistant.md`.
2.  **Workflow Execution**: Use the standardized procedures in `/workflows/` to handle routine requests like generating study guides or quizzes.
3.  **Structural Integrity**: Maintain this directory structure. Any new documentation should go to `/knowledge/`, new processes to `/workflows/`, and new personas to `/roles/`.
4.  **Readability**: Always write clear, markdown-formatted outputs when creating new files for non-coders.
5.  **Slide Change Logging**: After any modification to a file in `/slides/`, append a compact one-line entry to `/MEMORY.md` using this format:
    `[YYYY-MM-DD] <filename> — <brief description of what changed>`