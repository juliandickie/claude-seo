# Syncing this fork with upstream

Run this whenever you want to pull upstream improvements.

1. git fetch upstream

2. git checkout main, then git merge upstream/main

3. The merge should be clean. pro-marketing is additive and never conflicts. If a tracked file conflicts, an upstream file was edited against the rule. See CUSTOMIZATIONS.md.

4. python3 -m pytest tests/ -q

5. Run one demo build end to end (agency sub-project 1) and confirm the site is still good.

6. Update the pinned commit in CUSTOMIZATIONS.md, then commit.
