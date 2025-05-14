# Cursor Rules

This directory contains the cursor rules that will be copied to generated projects when `include_cursor_rules` is set to `true`.

## Included Rules

| Rule File | Purpose | Auto-Attach | Scope |
|-----------|---------|-------------|-------|
| 010-core-python-style.mdc | PEP 8, Black, typing, f-strings | Always applied | All Python files |
| 020-docstrings.mdc | NumPy-style docstrings | Auto-attach | src/**/*.py |
| 030-tdd-python.mdc | Test-driven development | Auto-attach | src/**/*.py |
| 040-bug-fix-tdd.mdc | Bug fix protocol | Agent request trigger | src/**/*.py |
| 100-pytest-autogen.mdc | Test scaffolding | Agent request trigger | New features |
| 200-domain-specific.mdc | Business rules | Auto-attach | domain/**/*.py |

## How to Update Rules

1. **Edit rules in this directory**: Modify the `.mdc` files directly
2. **Commit changes**: Tag a new version of the template
3. **Apply to existing projects**: 
   - Either regenerate the project with the new template version
   - Or manually copy the updated rules to existing projects

## Single-Repo Model

This template uses the "single-repo" model where cursor rules are:
- Stored directly in the cookiecutter template
- Copied to projects during generation
- Versioned with the template itself

This approach is ideal for:
- Solo developers or small teams
- Rules that change infrequently
- Simple project setups

For teams needing more flexibility with frequent rule updates across many projects, consider the two-repo model with Git submodules.
