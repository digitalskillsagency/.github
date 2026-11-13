# .github Repository Guide

This repository provides shared GitHub configuration for all repositories in the **digitalskillsagency** organisation.

## What This Repository Does

GitHub automatically applies files from this repository across all org repositories that do not define their own equivalent files.

## Structure

| Path | Purpose |
|---|---|
| `workflow-templates/` | Reusable workflow templates shown in the Actions tab of org repos |
| `ISSUE_TEMPLATE/` | Default issue templates applied org-wide |
| `PULL_REQUEST_TEMPLATE/` | Default PR description template |
| `DISCUSSION_TEMPLATE/` | Default discussion category templates |
| `.github/workflows/` | Workflows that run within **this** repository only |

## Scope and Precedence

- Files here apply only when a repository does **not** define its own equivalent.
- Repository-level files always take precedence over these org defaults.
- Workflow templates are not auto-applied; they appear as starter options in the Actions UI.

## Maintenance

- Changes to templates take effect immediately for new issues/PRs opened after the commit.
- Workflow template changes apply when a contributor next selects the template.
- Keep templates minimal — prescribe structure, do not over-specify content.

## References

- [GitHub: Creating a default community health file](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- [GitHub: Sharing workflows with your organisation](https://docs.github.com/en/actions/using-workflows/sharing-workflows-secrets-and-runners-with-your-organization)
