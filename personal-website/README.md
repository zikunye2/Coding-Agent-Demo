# Demo 2: Personal Website with a Coding Agent

## Overview

Use a coding agent to transform your resume into a professional portfolio website — powered by the DevPortfolio Astro template.

**How it works**: The agent reads your resume, updates a single config file (`src/config.ts`), and launches a live preview.

## Files

| File | Description |
|------|-------------|
| `inputs/sample_resume.md` | Sample resume (replace with yours!) |
| `inputs/project1_summary.md` | Project summary from Demo 1 |
| `website/devportfolio-master/` | Astro portfolio template |

## Quick Start

1. Open any coding agent (Claude Code, Cursor, Copilot, Gemini CLI, etc.)
2. Navigate to this folder
3. Paste the prompt below

## Prompt

```
You are working in the personal-website/ folder.

Inputs:
- inputs/sample_resume.md (replace with YOUR resume)
- inputs/project1_summary.md (your churn analysis project summary)

Website template: website/devportfolio-master/

Task:
1. Read the resume and project summary files
2. Update website/devportfolio-master/src/config.ts with:
   - name, title, description from resume
   - aboutMe section summarizing the resume
   - skills array from resume
   - projects array: include the churn prediction project from project1_summary.md
   - experience array from resume work history
   - education array from resume
   - social links (use placeholder URLs if not in resume)
3. Do NOT invent claims, metrics, or outcomes not in the source files
4. Keep descriptions concise and professional
5. Install dependencies and start the dev server so I can preview the site
```

## Personalize It

To use your own information:
1. Replace `inputs/sample_resume.md` with your actual resume (in markdown)
2. Update `inputs/project1_summary.md` with your own project details
3. Run the prompt — the agent does the rest!

## Template Details

The DevPortfolio template uses Astro + Tailwind CSS. All content is configured through a single file: `src/config.ts`. The agent only modifies this one file. See `website/devportfolio-master/CLAUDE.md` for template architecture details.
