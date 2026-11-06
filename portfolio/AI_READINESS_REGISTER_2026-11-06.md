# MCP software portfolio: repository and AI-readiness register
Date: 2026-11-06
Status: **audit working draft**. GitHub repository existence has been checked; runtime, latest branches, tests and deployments have NOT been comprehensively audited. Do not conflate a repository with a working product.

## Operating standard
Every active or planned software project needs a named owner, canonical repo and branch, product purpose, user workflows, in-scope/out-of-scope requirements, acceptance tests, implementation evidence, deployment targets and commands, dependency contracts, security/backup rules, current backlog, decision log and status with an evidence date. An `AGENTS.md` must point agents to those sources. Record proposed work separately from approved work. Make no stage/live changes without Peter's permission; DEV work remains subject to existing security/Workshop controls.

## Verified MCP-Creative-Labs repository inventory (43)
### Current/recent core products, tools and platform
- `storyforge-v2`: StoryForge v2 editorial intake, workflow and publishing; v1 live cutover remains distinct.
- `magforge`: magazine production/CTM; stale default-branch docs to reconcile with reported 548 tests and DEV.
- `cinemadata-v2`: new catalogue/import; stale planning docs versus reported 0.4.1 DEV.
- `IndexForge`: approved-only magazine archive extraction and indexing.
- `cineennyd-poc`, `cineennyd-dcp-worker-poc`, `cineennyd-ui`: one CineEnnyd product across multiple repos; AWS MP4-to-DCP and DCP conversion require defined contracts and cost approval.
- `mcp-audio`: audio/podcast workflow; POC versus laptop episodes/Podbean needs reconciliation.
- `mcp-mail`: multi-account mail triage planning, Gmail read-only first, Zoho/Yahoo/AWKE proposed.
- `mcp-travel`: closure-aware journey decision assistant, not sat nav.
- `worth-a-look`: discoveries, events and Worth a Detour ranking.
- `command_centre`: current ProjectBoard implementation; existing docs mention repository renaming, not proof completed. Check whether Notion changes the product's role.
- `project_dashboard`: local repository/status auditor, not ProjectBoard or live monitor.
- `mcp-account-management`: shared account-control library, not cross-product shared authentication.
- `mcp-ui-design-system`: common interface design guidelines.
- `MCP-clip`: editorial browser clip/publishing utility.
- `mcpwebsite`, `mcp`, `homepage`: different public/technical sites; confirm ownership of new cinematic WordPress theme and actual deployment target.
- `MCP-ai`, `MCP-mcp`: related AI information and mcp.guru entry-point concepts, boundary and routing to resolve.
- `mcp-estate-review`: estate audit/tooling; classify owner and deliverables.
- `tunnicliffe`: provisional HOLD pending handover and ownership; no discretionary development.

### Legacy, adjacent, experimental or status-to-decide repositories
- `StoryForge`, `StoryForge-Cursor`, `CTNewsBuilderApp`: predecessor/editorial variants; verify archive or migration provenance.
- `cinemadata`: v1 live reference; do not overwrite while v2 pending.
- `PromptForge`, `promptforge-new`: determine canonical prompt-management product and duplication.
- `VideoForge`, `YouTubeGrabber`: media tooling, scope and owner to confirm.
- `creativelabs`, `docs`, `Old`: organisational/reference/legacy, not automatically deployable products.
- `ctcprojectforge`: CTC management concept, distinct governance.
- `cinemajobs`: cinema employment portal concept, ownership and business requirements open.
- `solarmeter`, `solarmeter-python`, `merrifieldsolardata`: solar data tools, classify active/legacy.
- `HouseBuying`, `driver_hours`: personal utility, classify support.
- `-mcp-dispatcher-sandbox`, `-mcp-dispatcher-authority`: operational/security infrastructure; do not change without governance review.

## Projects or initiatives mentioned but repository not established in this organisation
These may live in another owner, share a repository or be planned only. **Do not create repos automatically** until canonical ownership is established.
- MCP Workshop / agent controller / Hermes DEV pilot / Telegram integration: known work in `knighp01/mcp-agent-infra` and related infra, outside this organisation inventory; preserve Gate Zero.
- MCP | SoftwareBoard: potentially part of `project_dashboard`; product boundary needs confirmation.
- MCP | CineFix: intended product, exact canonical repo not verified.
- TrainingForge / cinema training tools / Introduction to Cinema: planned, scope and repo not verified.
- MCP Knowledge Hub / chat indexing: planned; access, privacy and retention design needed.
- MCP Vault / CTC Projection Handbook: content archives/products; decide whether they require dedicated software repos.
- MCP newsletter automation, press-release newsdesk, Mailchimp/WordPress publishing and n8n automation: cross-product workflows, not necessarily standalone repositories. Source of truth and job ownership needed.
- AWS transcode/orchestration: three-repository deployment plan and expense controls need explicit repo mapping.
- WordPress cinematic theme and migration: verify current branch/repository, staging data fidelity and cutover controls.
- MCP AI/Command Centre/ProjectBoard/Notion: evaluate adoption before duplicating tools.

## Evidence gaps that need attention first
1. Compare latest main/dev commits, tests and deployed DEV builds for MagForge, CinemaData v2, StoryForge v2 and IndexForge, because some canonical status files are stale.
2. Establish canonical code/site relationship for public WordPress rebuild, legacy WordPress and MCP's static site repos.
3. Choose authoritative project management: existing ProjectBoard versus Notion, and whether SoftwareBoard stays a technical monitor.
4. Confirm CineEnnyd three-repo interface, AWS lifecycle, source rights, naming/re-encode requirements, testing and cost gates.
5. Confirm operational owner and success criterion for MCP Audio, newsroom/newsletters and mail automation.
6. Keep Tunnicliffe on hold pending responsible handover; determine retention and access obligations.
7. Audit all remaining legacy/concept repos before treating them as active development targets.

## Standard handover procedure for agents
1. Read `AGENTS.md`, PRD, status, architecture, decisions, backlog, tests, deployment and existing PRs.
2. Produce evidence matrix: approved requirement / implemented / tested / DEV deployed / outstanding / blocked / proposed, with commit and environment identifiers.
3. Identify missing acceptance criteria, propose options and ask Peter only on material product decisions.
4. Implement only approved scope in reviewable branches. Update truthful documentation and issue status.
5. Run tests and document actual results. Deploy to DEV only where explicitly within existing controls, never infer approval for STAGE/LIVE.
6. Record decisions in GitHub so future coding agents need no inaccessible chat memory.

## Review state
This register is an initial inventory and classification, **not certification that every project is AI-ready**. Handover documents and draft PRs in individual repos are preparatory. Existing PRDs and status files still require reconciliation with current code and product-owner decisions.
