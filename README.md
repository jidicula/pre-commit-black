# pre-commit-black
Minimal example of Black pre-commit hook failing to respect pyproject.toml exclude rule.

The `main` branch uses black 20.8b2. The `master-black` branch uses black's `master` branch.

# To run
1. `poetry install`
2. `poetry shell`
3. `pre-commit install`
4. Add a trailing newline to `ignored/ostensibly_ignored.py`.
5. Run `black check .` to verify that project files pass.
5. Stage the change and attempt to commit.
