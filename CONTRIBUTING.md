# Contributing to Tatva Technology repos

These rules apply to every repo in the org unless the repo has its own CONTRIBUTING.md.

## Branches

- `main` is always deployable. Nobody pushes to it directly.
- Branch from `main`, named `<type>/<short-description>`, for example `feat/gp-tax-report`, `fix/login-otp-timeout`.
- Types: `feat`, `fix`, `chore`, `docs`, `refactor`, `test`.

## Commits

[Conventional Commits](https://www.conventionalcommits.org/): `feat: add property tax PDF export`. Small commits that each do one thing.

## Pull requests

1. Open a PR early as Draft if you want feedback.
2. Fill in the PR template. Link the issue (`Closes #12`).
3. CI must pass.
4. At least one lead approves. Reviewers respond within one working day.
5. Squash-merge. The branch is deleted automatically.

## Never commit

- Passwords, API keys, tokens, `.env` files, private keys.
- Client personal data (Aadhaar, phone numbers, addresses), production database dumps.
- Large binaries. Use releases or cloud storage.

If you commit a secret by mistake: tell a lead **immediately**, then rotate the secret. Deleting the commit is not enough.
