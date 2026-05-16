# GitHub Automation

## What is automated

For a new project, one command can now:

1. initialize `git`;
2. create `main`;
3. create a new GitHub repository;
4. push the project to `origin/main`;
5. install a safe branch workflow;
6. create a stable tag for rollback.

## Command

Run from the project root:

```bash
/Users/dzavidgabibov/Documents/Codex/scripts/codex_bootstrap_github_project.sh repo-name public
```

or:

```bash
/Users/dzavidgabibov/Documents/Codex/scripts/codex_bootstrap_github_project.sh repo-name private
```

## After bootstrap

For every change:

```bash
./scripts/start-change.sh task-name
```

This creates:

- a working branch;
- a snapshot tag for rollback.

`main` remains the stable version.

## What is still not automatic

The machine does not decide on its own when to create a new project or what repository name you want.

You still need to give one clear start command, for example:

`Create a new landing page project, bootstrap GitHub repo, keep main stable, and do all changes through work branches.`
