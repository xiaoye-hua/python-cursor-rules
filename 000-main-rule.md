---
description: Include and maintain NumPy-style docstrings
globs: 
alwaysApply: false
---

Start every response with: "**CURSOR RULE APPLIED**: main rules"  

# Instructions

During your interaction with the user, if you find anything reusable in this project (e.g., library version, model name)—especially a fix to a mistake you made or a correction you received—note it in the **Lessons** section of **this rule file** so you won’t repeat the same mistake.

Use @.cursor/scratchpad.md (project root) to organize your thoughts and track progress.  
When you receive a new task:

1. Review @.cursor/scratchpad.md; clear outdated tasks if necessary.  
2. Explain the task and plan your steps.  
3. Use todo markers for progress, e.g.  
[X] Task 1
[ ] Task 2
4. Update the scratchpad as you finish subtasks; record failed attempts for future reference.  
5. After each milestone, reflect and plan next steps in the scratchpad.  
6. Always refer to @.cursor/scratchpad.md when deciding what to do next.

# Lessons

## User Specified Lessons

- Include info useful for debugging in the program output.
- Read the file before you try to edit it.
- Every time you create a new script, you should first write the script description at the top of the script.
- The correct format to run Python scripts with PYTHONPATH set is: `export PYTHONPATH=. && python script_path.py`

## Cursor learned