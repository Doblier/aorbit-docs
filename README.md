# AORBIT Documentation

Official documentation for **AORBIT™** — the Autonomous Enterprise Intelligence Suite by [Doblier](https://doblier.io).

**Live site:** https://docs.doblier.io

## How this repo works

Docs-as-code, published by Mintlify. `main` **is** the live site: merge to `main` = published.

1. Create a branch and edit/add `.mdx` files.
2. Preview locally: `npx mint dev` → http://localhost:3000
3. Open a pull request. The folder owner (see `.github/CODEOWNERS`) reviews.
4. Merge → Mintlify deploys automatically.

New pages must be added to `docs.json` navigation to appear on the site.

## Repository layout

```
docs.json        Site config & navigation (Mintlify)
index.mdx        Documentation home
platform/        Cross-product docs: architecture, security, release policy
orca/            ORCA — IT Operations & AIOps (AORBIT Intelligence)
```

## Documentation ownership

| Area | Owner | Review cadence |
|---|---|---|
| `platform/architecture`, `orca/architecture` | _architect_ | per release |
| `orca/operations`, `orca/readiness`, `orca/deployment` | _SRE lead_ | per release |
| `platform/security` | _security owner_ | quarterly |
| `platform/release`, `orca/release-notes` | _release owner_ | per release |

## Ground rules

- **No client-identifying data.** Client names, logos, environments, and engagement material never enter this repo.
- **No secrets.** No credentials, tokens, internal hostnames, or IPs — use `example.com` style placeholders.
- **Honest statuses.** Module availability is stated exactly as licensed: GA / Pilot / Gated / Roadmap. Nothing rounded up.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the style guide and [SECURITY.md](SECURITY.md) for vulnerability reporting.

---
© 2026 Doblier Inc. DOBLIER™ and AORBIT™ are trademarks of Doblier Inc. See [LICENSE.md](LICENSE.md).
