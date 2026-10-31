# Organization profile review

Review date: 2026-10-31. Scope: tuprel/.github only. No organization settings,
main-project branches, migration PRs, database objects or logo assets changed.

## Previous experience

The public profile used a different tagline, a plain heading, three navigation
links and no badges or workflow. It explained the toolkit accurately, but did
not reflect the visual hierarchy of the main project or provide direct CLI/API
entry points. The organization displayed two repositories under Popular
repositories, rather than a curated Pinned section.

## Proposed experience

Centered TUPREL hero, approved tagline, three primary links and six badges in
three pairs. Reuse the existing four workflow assets directly from main-project
commit addc7275ec85fbb7c2634e3494b45688a0848401: desktop/mobile and Light/Dark.
No new graphics, copied binary assets or replacement logo. Pinning asset URLs to
a verified commit prevents an unrelated asset edit changing this proposal.

Seven short sections explain the product, practical benefits, workflow,
repository, onboarding, documentation/examples and participation. All links to
the main project are absolute. Availability matches main: offline creation,
read-only status and library preview/plans, without migration execution.

The organization overview intentionally links to compiled Java examples in the
main project instead of repeating a query fragment and its imports here. No
executable code, new installation commands or simulated terminal output is added.

## Organization settings: owner proposal

These are proposals for separate review, not configuration changes made by this PR.
Repository admin permission was confirmed; organization-owner permission was not
assumed from repository access.

| Setting | Observed | Proposed |
|---|---|---|
| Public name | Tuprel | TUPREL, matching the approved README identity |
| Description | Modern relational data toolkit for Java. | Schema-first Java toolkit for typed PostgreSQL access. |
| Website | Not set | https://github.com/tuprel/tuprel/blob/main/docs/README.md |
| Featured repositories | Popular repositories lists tuprel and .github | Pin tuprel first; keep .github as configuration, not a second product |
| Logo | Existing blue/teal avatar | Preserve the current avatar; no new logo or re-upload |
| Public email/social | Not set | Leave unset until an owner supplies a maintained contact; use Issues and Security links |
| Community | No public members shown | Members may choose public visibility individually; do not expose membership automatically |

Owner steps after approving the profile:

1. Merge this PR through the normal review process to publish profile/README.md.
2. Open https://github.com/organizations/tuprel/settings/profile as an organization
   owner. Set the approved public name, description and website above, then save.
   Leave avatar, email and social fields unchanged unless separately approved.
3. On https://github.com/tuprel, use Customize your pins (when signed in as an
   authorized organization member) and select tuprel/tuprel as the first pin.
   GitHub may require pins to be enabled/customized before this control appears.
4. Review the published overview in both themes and on a narrow screen. The
   branch-file preview does not reproduce the organization header/sidebar.

No separate website, support email, chat service or other product is invented.

## Validation

- 31 unique absolute resource URLs returned HTTP 200, including six badge images,
  both workflow destinations, documentation and all four pinned SVG variants.
- Main-project fragment destinations reuse the verified compatibility and local
  PostgreSQL setup anchors. Badge workflow links explicitly select main.
- Existing launcher --version and --help executed successfully from this checkout,
  without credentials or database access. No root/playground builds were needed
  for this Markdown-only change; no Java examples were added.
- Git diff whitespace check passed. This repository has no Actions workflows;
  absence of checks is not reported as CI approval. Main-project badges show
  main-project state, not validation of this profile PR.
- Rendered GitHub previews and limitations are recorded in the PR description.
  Dark-mode assets existing in source do not constitute a verified Dark preview.

## Review links

- Profile source: ../profile/README.md
- Main documentation: https://github.com/tuprel/tuprel/blob/main/docs/README.md
- Current public organization: https://github.com/tuprel
