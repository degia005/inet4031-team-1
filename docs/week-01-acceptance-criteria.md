# Week 1 Acceptance Criteria

Sprint 1, Week 1 (Setup & Team Formation). A deliverable is done when every box below is checked and QA has signed off in `docs/qa-report-1.md`.

## Team and documentation
- [ ] `README.md` at repo root has the team name, team number, full roster, and the Google Doc link (accessible to everyone at the University of Minnesota)
- [ ] `team-charter.md` has: Team Name, Team Number, Full Roster, Sprint 1 role assignments, one-sentence role descriptions, 7-Sprint Rotation Schedule (every member holds Scrum Master, System Admin, and QA at least once), Communication Norms, three Operating Agreements, Container Baseline
- [ ] All teammates added as collaborators with Write access
- [ ] GitHub Project board linked to the repo with Backlog / In Progress / In Review / Done columns and Sprint 1 tickets opened

## Environment
- [ ] Every team member has run `whoami` and `hostname` inside the shared team container (screenshots in the Google Doc)
- [ ] Container baseline recorded (OS, disk space, installed vs. missing tools, `docker info`) in `docs/week-01-environment-log.md` and in the Container Baseline section of `team-charter.md`
- [ ] `df -h` and `docker system df` output recorded under "Week 1 Storage Baseline" in the Google Doc

## Ansible
- [ ] `ansible/inventory` targets localhost with `ansible_connection=local`
- [ ] `ansible/site.yml` contains the "Baseline environment setup" play using the dnf module
- [ ] First playbook run shows `failed=0` and `unreachable=0`
- [ ] Second playbook run shows `changed=0` (screenshot in the Google Doc)

## Validation
- [ ] `ls -1` at repo root shows README.md, ansible, docs, scripts, team-charter.md, week-1 through week-9
- [ ] `./scripts/check-week1.sh` passes with zero failures
- [ ] Google Doc contains the Sprint 1 Reflections section with the Part 2 and Part 3 discussion answers
- [ ] QA sign-off completed in `docs/qa-report-1.md`
