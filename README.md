# HireMind

### Evidence-first hiring, built around the employer's workflow.

HireMind brings job criteria, résumé comparison, candidate applications and interview evidence into one hiring workspace. The goal: show the evidence behind a recommendation, make uncertainty visible, and leave hiring decisions with people.

**[Explore the live product](https://hiremind-evidence-first.sharmaaishu84.chatgpt.site/)** · **[Download the full source](HireMind-source.zip)**

## What's included

- Employer and candidate workspaces with email-code authentication.
- Job posts, weighted criteria, multi-résumé comparison and source-linked explanations.
- Résumé/profile intake, job discovery and application tracking.
- Recruiter CRM, talent search, saved searches and team permissions.
- Interview scheduling, calendar export, live-call implementation, transcript import and structured scorecards.
- Matching benchmarks, analytics and export/integration endpoints.

## Source package

`HireMind-source.zip` contains **223 files**: the application, API routes, matching and parsing logic, database schema/migrations, assets, automated tests and documentation. Extract it to get the project root and full setup README. The source is packaged as a ZIP in this repository; it is not yet a file-by-file Git checkout.

Production candidate data, credentials, runtime storage and old Git history are excluded. Supabase and hosting identifiers have been replaced with placeholders; configure your own services before running authenticated workflows.

## Stack

TypeScript · React 19 · Tailwind CSS 4 · Vinext/Vite · Cloudflare Workers · D1/SQLite · Drizzle · R2 · Supabase Auth · WebRTC

Supabase provides authentication; D1 stores application data. This is not a static GitHub Pages site.

## Matching philosophy

The matcher distinguishes demonstrated work, claims, missing evidence, stated gaps and conflicting statements. Relevant work with a different tool can be surfaced for human review without treating the tools as equivalent or inflating the score.

The current approach is deterministic, with curated skill aliases and six bounded English responsibility families. Scores are heuristics, not probabilities of job success. There is no independently verified accuracy figure or claim of superiority over another vendor.

## Development status

The upstream v9 snapshot passed 174 automated tests, TypeScript checking and a production build on 25 September 2026. That is development verification, not full signed-in production end-to-end testing. Email delivery and live calls depend on external-service configuration. The exported source has not been separately tested against a new backend.

See the full README and `docs/` inside the source archive for setup, matching limitations and roadmap details. Roadmap items are not promises of verified production behavior.

## Security and licensing

Do not include candidate documents or credentials in public issues. See [SECURITY.md](SECURITY.md).

No open-source license has been selected. Public visibility does not itself grant a general reuse or redistribution license. Dependencies retain their respective licenses.
