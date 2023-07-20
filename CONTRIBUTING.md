# Contributing to AORBIT Documentation

## Who can contribute

- **Doblier team:** branch → PR → CODEOWNERS review → merge (publishes to docs.doblier.io).
- **External readers:** we welcome issues for errors, gaps, or unclear sections. PRs for typo-level fixes are accepted; substantive external PRs will be discussed in an issue first.

## Workflow

1. Branch from `main` (`docs/<topic>` naming, e.g. `docs/orca-sizing-tiers`).
2. Edit or add `.mdx` files. New pages must be registered in `docs.json` navigation.
3. Preview: `npx mint dev`
4. Open a PR and complete the checklist in the PR template.
5. Owner review → merge → live.

## Style guide

- **Audience:** enterprise architects, SREs, security and compliance reviewers. Write precisely; no marketing language in technical docs.
- **Voice:** direct, present tense, second person for instructions ("Run…", "Verify…").
- **Statuses:** always one of GA / Pilot / Gated / Roadmap, matching the current license map. Never overstate availability.
- **Numbers:** performance and recovery figures must be *measured* values with their source (e.g., chaos experiment) — never vendor claims restated as ours.
- **Placeholders:** `example.com`, `<CUSTOMER_ID>`, `10.0.0.0/24`-style documentation ranges only.
- **Diagrams:** Mermaid in fenced code blocks, so diagrams are reviewed and versioned like text.
- **Callouts:** use Mintlify components — `<Note>`, `<Warning>`, `<Info>`, `<Tip>`.

## Hard rules (PR blockers)

- No client names, logos, or client-attributable data.
- No credentials, tokens, license keys, internal hostnames, or real IPs.
- No roadmap commitments beyond what is published on doblier.io.

## Versioning

Docs are versioned per product release. Release notes live in `orca/release-notes/`; the technology-stack page is updated in the same PR as any release that changes component versions.
