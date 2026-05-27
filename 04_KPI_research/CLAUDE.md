# Project Context
In this project, I want to have an agent, that will be able to crawl for recent KPIs and OKRs among the FSI C-level positions. This agent will research only one position at a time, and will be focused only on a specific geography. Besides current KPIs and OKRs (maximum 2 years old), I want to also see a projection for next 1,3 and 5 years based on strong conference posts, articles and researches

# About Me
I am a business, process and IT consultant in a major consultancy (outside of big 4)
I have a business background, I do understand technology and IT concepts, I am close to data and processes.
I prefer clear, jargon-free output.

# Rules
Always ask clarifying questions before starting a complex task
Always ask in case of uncertanies or conflicts in the inputs
Show your plan and steps before executing
Save all output files to the output folder

# Project Structure
- workflows/ - Workflow instruction files (plain English recipes the agent follows)
- output/ - Finished deliverables (reports, drafts, analysis)
- resources/ - References docs and templates

# Git workflow
After every meaningful change — new feature, bug fix, refactor — commit and push to `origin/main` (https://github.com/lukaskulhavy/POC_UML). Never batch unrelated changes. This keeps a clean history and ensures work is never lost.

Commit message format:
- Subject line: short imperative summary (e.g. `Fix win detection for draw state`)
- Body (optional): explain *why*, not just *what*
- Always append: `Co-Authored-By: Claude`

Push immediately after each commit so GitHub always reflects the latest state.