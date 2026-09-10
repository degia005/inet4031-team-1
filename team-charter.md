# Team Charter - Sprint 1

## Team Identity

**Team Name:** Team 5

**Team Number:** 5

**Full Roster:**

| Name | Email | GitHub | Role (Sprint 1) |
|------|-------|--------|-----------------|
| Dane DeGiacomo | degia005@umn.edu | degia005 | Scrum Master |
| Santiago Caldas Quiroga | calda034@umn.edu | calda034 | System Admin |
| Nazariah Makpo | makpo002@umn.edu | makpo002-cpu | |
| Neshy Waakuwa | waaku001@umn.edu | neshylia17 | |
| Reina Ganter | gante031@umn.edu | | |
| Shanna Nunez | nunez192@umn.edu | nunez192 | |

## Role One-Sentence Descriptions

- **Scrum Master:** Runs the sprint board and standups, opens the tickets for each week, keeps track of who is blocked, and writes the retrospective at the end of the sprint.
- **System Admin:** Owns the shared container and the Ansible playbook, leads the infrastructure steps in each lab, and keeps the environment log and runbooks up to date.
- **QA:** Runs every validation check and the check script, fills out the QA report, and is the last sign-off before anything gets submitted.
- **Developer:** Writes the config files and manifests for the week, follows the lab steps, and opens pull requests for the work so someone else can review it.

## 7-Sprint Rotation Schedule

Every team member must hold Scrum Master, System Admin, and QA at least once across the seven sprints. Fill in this table using what you jotted down in your Google Docs:

```
Sprint 1: Scrum Master = Dane, System Admin = Santiago, QA = ___, Developers = ___
Sprint 2: Scrum Master = ___, System Admin = ___, QA = ___, Developers = ___
Sprint 3: Scrum Master = ___, System Admin = ___, QA = ___, Developers = ___
Sprint 4: Scrum Master = ___, System Admin = ___, QA = ___, Developers = ___
Sprint 5: Scrum Master = ___, System Admin = ___, QA = ___, Developers = ___
Sprint 6: Scrum Master = ___, System Admin = ___, QA = ___, Developers = ___
Sprint 7: Scrum Master = ___, System Admin = ___, QA = ___, Developers = ___
```

## Three Team Operating Agreements

1. **Playbook changes:** All changes to `ansible/` go through a reviewed pull request, and only the System Admin runs `ansible-playbook` against the shared container after the merge. Nobody applies an unmerged playbook to the container.

2. **Merge conflicts:** Whoever opened the later pull request pulls `main`, resolves the conflict on their branch, and pings the other author in chat before merging. We do not force push to `main`.

3. **When the container acts up:** Stop, post what you were doing and what you saw in the chat, and do not try to fix it alone. The System Admin leads the troubleshooting, and anything fixed by hand gets written into `docs/week-01-environment-log.md` and folded back into the playbook so the fix is reproducible.

## Communication Norms

- **Where we talk:** [team chat / channel]
- **Merges and breakage:** [how we notify each other]
- **Response time:** [normal / when someone is blocked]
- **PR reviews:** [who reviews and how fast]

## Container Baseline

Filled in by the System Admin during Part 3. Full command output lives in `docs/week-01-environment-log.md`.

| Item | Value |
|------|-------|
| Access method | [SSH / docker exec] |
| OS and version | [from `cat /etc/os-release`] |
| Disk space available on / | [from `df -h`] |
| docker | [installed / missing] |
| git | [installed / missing] |
| python3 | [installed / missing] |
| curl | [installed / missing] |
| ansible | [installed / missing] |
| Docker daemon | [from `docker info`: server version, storage driver] |
