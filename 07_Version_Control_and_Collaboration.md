# 07. Version Control & Collaboration (Git, GitHub)

---

## What is Version Control?

Version control is a system for recording changes to files or codebases over time so that specific versions can be recalled later. It enables collaboration, tracking, and recovery from mistakes.

---

## Types of Version Control

- **Local:** Changes tracked on a single machine.
- **Centralized (CVCS):** All changes tracked on a central server (e.g., SVN).
- **Distributed (DVCS):** Every user has a full copy of the repository (e.g., Git).

---

## Why Version Control Matters

- **Collaboration:** Multiple people can work on the same project.
- **History:** Track who changed what, when, and why.
- **Recovery:** Roll back to earlier versions if needed.
- **Branching:** Experiment without affecting main codebase.
- **Auditing:** Compliance and accountability.

---

## Git Basics

- **Repository:** Directory tracked by Git.
- **Commit:** Snapshot of staged changes.
- **Branch:** Isolated line of development.
- **Merge:** Combine branches together.
- **Clone, Pull, Push:** Copy, fetch, and send data to/from remotes.

---

## Common Git Commands

```bash
git init
git clone <repo-url>
git status
git add <file>
git commit -m "message"
git push
git pull
git branch
git checkout <branch>
git merge <branch>
git log
git revert <commit>
git rebase <branch>
```

---

## GitHub for Collaboration

- **Pull Requests (PRs):** Propose, discuss, and merge code.
- **Issues:** Track bugs, feature requests, and tasks.
- **Reviews:** Provide and receive feedback before merging.
- **Actions:** Automate tests, builds, and deployments (CI/CD).
- **Wiki & Projects:** Documentation and project tracking.

---

## Git Workflow Best Practices

- Use feature branches for new features.
- Commit frequently with clear messages.
- Pull/rebase often to stay up to date.
- Use PRs and require reviews before merging.
- Tag releases and use semantic versioning.

---

## Handling Merge Conflicts

- Occur when changes in different branches conflict.
- Use `git status` and `git diff` to investigate.
- Manually resolve in code, then add, commit, and continue.

---

## Advanced Collaboration

- **Forking:** Contribute to open source projects.
- **Blame:** See who last modified each line.
- **Squash Merges:** Combine multiple commits into one.
- **Protected Branches:** Restrict force-push and require status checks.

---

## Tools

- **GitHub Desktop, GitKraken:** GUIs for Git.
- **GitLab, Bitbucket:** Alternatives to GitHub.
- **Jira, Trello:** Issue and project tracking integration.

---

## Interview Questions

1. How do you resolve a merge conflict?
2. What is the difference between merging and rebasing?
3. How would you recover from accidentally deleting a branch?
4. What are the benefits of using pull requests?
5. How do you ensure code quality in a collaborative project?

---

## References

- [Git Documentation](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com/)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)

---

## Exercises

1. Create a git repository, make several commits, and view the log.
2. Simulate a merge conflict and resolve it.
3. Open a pull request and perform a code review.
4. Experiment with branching and rebasing in a test project.
5. Set up GitHub Actions for automated testing.

---

## Summary

Version control and collaboration are fundamental to modern software engineering. Mastering Git, GitHub, and associated workflows is essential for teamwork, quality, and productivity.

---
