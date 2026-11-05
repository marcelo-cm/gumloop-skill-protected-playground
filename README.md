# Protected skill sync playground

Synthetic skills for testing Gumloop saves against a protected GitHub branch.
This public repository contains no customer data or credentials.

## Connect in Gumloop

- Repository: `marcelo-cm/gumloop-skill-protected-playground`
- Branch: `main`
- Source folder: `skills`

The repository contains two valid skills: `protected-release-summary` and
`protected-support-triage`. These names differ from the unprotected playground
so both repositories can be connected to the same Gumloop organization.
Importing the repository root also finds only these two skills.

## Branch protection

Changes to `main` must go through a pull request. The rule also applies to the
repository owner. Direct pushes, force pushes, and branch deletion are blocked.
No approval or CI check is required to merge a pull request.

Use this repository to test what Gumloop shows when a save targets a protected
branch. Check both GitHub and Gumloop after the save attempt.

For a permitted change, create a branch, edit a skill, and open a pull request.
Merge it only when ready to test the resulting GitHub-to-Gumloop sync.

## Example tasks

Ask Agent X to use `protected-release-summary` with the sample changes, or ask
it to use `protected-support-triage` for this synthetic report:

> User A can open the dashboard, but exporting a report fails. Other users can
> export reports. The issue started after User A changed teams.
