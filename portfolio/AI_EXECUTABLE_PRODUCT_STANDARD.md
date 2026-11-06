# MCP standard for AI-executable product specifications
Draft 2026-11-06. Applies to proposed changes after review; repository-specific stricter security requirements prevail.

## Required documents (or explicit equivalent links)
1. `README.md`: product identity, repository boundaries, safe local startup and documentation index.
2. `AGENTS.md`: AI entry point, canonical instructions, approved branches, security/approval policy, build/test checks, handover reporting.
3. `PRD.md` or `docs/PRD.md`: users, jobs-to-be-done, functional and non-functional requirements, explicit exclusions, dependencies, interface/data contracts, acceptance criteria, staged delivery and versioned scope.
4. `PROJECT_STATUS.md`: evidence date, branch, commit, current DEV deployment build (if independently verified), tested modules, known defects, unverified reports, next work.
5. `ROADMAP.md` or `docs/IMPLEMENTATION_PLAN.md`: approved milestones, dependencies, and definition of done.
6. `docs/DECISIONS.md` or existing decision log: question, options, recommendation, consequence, owner and decision date; **unresolved is not approval**.
7. GitHub issues: small deliverables traceable to requirement IDs; state and acceptance tests. No duplicate backlog disconnected from PRD.
8. `docs/DEPLOYMENT.md` or equivalent: exact environment branches, secrets (names not values), release and rollback, safe DEV test and authorisations.

## Requirement record template
- ID; title; statement of user-visible behaviour
- Product owner and source (confirmed/speculative/proposed)
- Priority and release target (approved or unapproved)
- Preconditions and dependencies
- Input/output, permissions, errors and edge cases
- Acceptance criteria in observable Given/When/Then form
- Automated tests and manual verification
- Code/PR/commit and DEV build evidence
- State: proposed / approved / implemented / tested / DEV verified / released / blocked / deferred
- Relevant unresolved design decision IDs

## Evidence and status requirements
'Implemented' means functionality exists at a specified commit; 'tested' means actual test run and result recorded; 'DEV verified' means service/build identity, date and smoke-test evidence recorded. A test count alone does not prove acceptance, and a published README alone does not prove deployment. Record conflicting information with both source dates.

## Agent workflow
- Inspect repo, current branches, CI, issues/PRs, code, tests and deployed DEV before changing an existing spec.
- Construct a requirements coverage matrix and prioritised, dependency-aware issues. Work through approved items independently.
- Work in reviewable branches and PRs. Keep project documents synchronised with verified changes; preserve earlier approved requirements.
- If product behaviour is unclear, create decision entry with alternatives and recommendation; continue on unblocked work.
- Verify test, database migration safety and DEV smoke tests. Deployment only where existing explicit process permits it.
- **Never** infer authority to spend money, alter credentials, bypass STOP/pause/Gate Zero, merge without review, change DNS, or release to STAGE/LIVE.

## Agent completion report
Product/repo; requirement IDs completed; commits/PRs; test commands and real output; deployment target and verified build; data changes and rollback; decisions required from Peter; unresolved blockers; next eligible tasks.

## Portfolio certification
Classify separately:
- **Documented**: source and scope mapped.
- **AI-preparable**: agent can inventory/test/design and raise PRs without ambiguity.
- **AI-implementable**: approved acceptance criteria and dependency/access prerequisites exist.
- **DEV-release-ready**: test/release/rollback and environment evidence are proven.
- **LIVE-release-ready**: explicit production approval, pre-release verification and rollback, independent of DEV acceptance.

This is a checklist, not an automatic certification. A repo must be reviewed against evidence before its state advances.
