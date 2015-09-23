#What is a Pull Request?
When it comes to managing any scale of project that involves working as a team,
pull requests end up being one of the most potent tools in the team's arsenal
to promote well-formed code.

If a feature branch is the beginning of a new feature, a pull request is its end.

---

A pull request is a fancy way of saying "please consider my code for
inclusion in the stable development branch." The origin of the name comes from
the git command `git request-pull`, which diffs a branch and its parent from a
certain point in time (represented by a commit sha), then dumps the changeset to
stdout.

If a team is using raw git for management (as opposed to GitHub or
GitLab, for example), the changeset would be sent to the team/team lead for
inspection and (hopefully) eventual inclusion into the main codebase.

Thinking about it semantically, a *pull request* is a *request* for someone else
to *pull* your changes into his/her codebase. The "someone else" in this case
may be an open source maintainer, your team members, or your product owner.

