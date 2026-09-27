# repo-tasks-gitflow-twin

A test target for [repo-tasks](https://github.com/TheodoreAD/repo-tasks)' `gitflow` tasks in PR
mode. It is not a project, and nothing here is meant to be used.

It exists because `gh pr create` needs a real GitHub remote, which a local bare repo cannot stand in
for, and because `main` and `develop` carry a ruleset with no bypass list. A direct push is
rejected here the way a protected team repo would reject it, including for the owner.

Leftover branches, tags and PRs from earlier runs are expected. The tests derive their starting
state from what is here rather than assuming a clean repo.

`tasks.py` imports `repo_tasks.ns`, so run `inv` from an environment where repo-tasks is installed,
usually repo-tasks' own venv with its working tree installed editable.
