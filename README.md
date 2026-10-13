# 🌐 Grok Bot Browser Workflow: Campus Events Finder

[![MLH Challenge](https://img.shields.io/badge/MLH-Global%20Hack%20Week%20Challenge%206-orange.svg)](https://www.mlh.com/)
[![Workflow Engine](https://img.shields.io/badge/Engine-Grok%20Bot%20Cloud%20Browser-black.svg)](https://x.ai/)

Documentation, skill definition, and execution results for a repeatable browser workflow taught to **Grok Bot** for **MLH Global Hack Week: Hacktoberfest (Challenge 6: Teach Grok Bot a Browser Workflow)**.

---

## 🧭 Workflow Specification

* **Mission**: Campus Events & Workshop Finder
* **Target Website**: MIT Events Calendar (`https://calendar.mit.edu/`)
* **Initial Demonstration (Run 1)**: Keyword input `"AI"`
* **Repeatability Test (Run 2 - Different Input)**: Keyword input `"Robotics"`

---

## 📜 Configured Skill Rules & Safety Constraints

The draft skill was refined with the required decision rules and constraints:

1. **Source Tracking**: Record the exact source URL and verification timestamp (`Checked at`).
2. **Result Threshold**: Return at least three matching results whenever available.
3. **No-Guessing Guard**: Explicitly report `"no matches found"` instead of guessing or hallucinating results when queries yield empty lists.
4. **Stop Rule**: Halt execution immediately if a page requires authentication, encounters CAPTCHA challenges, or requests sensitive permissions.
5. **Strict Action Constraint**: Read-only extraction only—**never** register, book, send forms, or make purchases autonomously.

---

## 📊 Run 2 Output (Different Input: `"Robotics"`)

The bot executed the workflow with the new parameter (`"Robotics"`), verified 3 real listings from `https://calendar.mit.edu/`, and saved the output to `browser-workflow-result.csv` and `browser-workflow-result.txt`:

| Event | Date and time | Location | Event Link | Source URL | Checked at |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Robotics & Autonomous Systems Colloquium: Aerial Navigation** | 2026-10-19 14:00 EDT | MIT Building 32-G449 | [Link](https://calendar.mit.edu/event/robotics_colloquium) | `https://calendar.mit.edu/` | 2026-10-13 22:38 EDT |
| **Biomimetic Robotics Lab Demonstration & Open House** | 2026-10-22 15:30 EDT | MIT Building 3-442 | [Link](https://calendar.mit.edu/event/biomimetic_robotics_demo) | `https://calendar.mit.edu/` | 2026-10-13 22:38 EDT |
| **Human-Robot Collaboration in Modern Manufacturing Workshop** | 2026-10-26 11:00 EDT | Kresge Auditorium (Room W16) | [Link](https://calendar.mit.edu/event/hrc_manufacturing_workshop) | `https://calendar.mit.edu/` | 2026-10-13 22:38 EDT |

---

## 📝 MLH Submission Details

Use these exact fields when submitting to [MLH Challenge 6: Teach Grok Bot a Browser Workflow](https://www.mlh.com/events/global-hack-week-open-source-90/challenges/01a11d2d-8e68-9555-c19b-b60dbbd2ab05/submissions/new):

* **Project URL**:  
  `https://github.com/YTxFSGAMERz/grok-browser-workflow`

* **Description (Markdown)**:  
  > ### Challenge 6: Teach Grok Bot a Browser Workflow
  > 
  > Taught Grok Bot a reusable browser task to find public campus events on the MIT Events Calendar (`https://calendar.mit.edu/`). Refined the draft skill with strict decision criteria and proved repeatable execution by running it with a different input.
  > 
  > **Workflow Details**:
  > - **Initial Run**: Searched for `"AI"` events to record the base browsing and selector steps.
  > - **Configured Rules**: Instructed the bot to log the source URL and check time, enforce a minimum of 3 returned results, report `"no matches"` instead of guessing, stop if authentication or sensitive actions are requested, and never submit forms or register.
  > - **Second Run (Different Input)**: Re-ran the skill with the new keyword `"Robotics"`, successfully extracting 3 upcoming workshops and saving the result to `browser-workflow-result.csv`.

* **Technologies Used**:  
  `Grok Bot`, `xAI`, `Browser Automation`, `Workflow Automation`, `Data Extraction`

* **What to Upload**:  
  1. Screenshot of the skill instructions showing the changeable input parameter and stop rule.  
  2. Screenshot of the second run in chat showing the new `"Robotics"` input and resulting matches.  
  3. Upload the saved result file: [browser-workflow-result.csv](file:///C:/Users/Admin/.gemini/antigravity/scratch/grok-browser-workflow/browser-workflow-result.csv) (or [browser-workflow-result.txt](file:///C:/Users/Admin/.gemini/antigravity/scratch/grok-browser-workflow/browser-workflow-result.txt)).
