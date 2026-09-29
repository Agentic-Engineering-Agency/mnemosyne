# Agentic: Mnemosyne adoption and extension proposal

Status: discussion draft, 2026-09-29. No extension implementation or hosted service is released by this proposal. This fork is maintained by Agentic Engineering and does not represent an upstream endorsement.

## Objective

Adopt Mnemosyne across multiple agent harnesses, with project boundaries, deliberate sharing and a portable deployment. Reuse upstream capabilities; add code only for demonstrated gaps. Start with an internal pilot before developing an optional paid managed service. Self-hosting remains part of the intended open-source direction.

Upstream owns the storage schema, BEAM lifecycle, extraction and retrieval. Human approval of company documents is outside this memory project. No memory draft-review UI, replacement graph engine, billing or SaaS control plane is needed for the first pilot.

## Discussion packet

- [Validation plan, decisions and diagrams](plan.md)
- [BEAM architecture](https://docs.mnemosyne.site/architecture/beam-overview)
- [Banks](https://docs.mnemosyne.site/memory-systems/memory-banks)
- [Multi-agent use](https://docs.mnemosyne.site/use-cases/multi-agent)
- [Access control](https://docs.mnemosyne.site/security/access-control)
- [Sync](https://docs.mnemosyne.site/operations/sync)
- [Upstream contribution guidelines](../../CONTRIBUTING.md)

## Provenance and maintenance

Initial audited source: `7295b4e23bf435942a4a630be4c43d0c51f182d5`, source package version `4.0.0b3`. The documentation home references v3.15.1; verify behavior against the selected source/package, not the website version alone.

The fork preserves upstream history and MIT license. Documentation added in this directory uses the repository's MIT license. Preserve upstream attribution. Product naming and hosted-service packaging remain future decisions.

```sh
git clone https://github.com/Agentic-Engineering-Agency/mnemosyne.git
cd mnemosyne
git remote add upstream https://github.com/mnemosyne-oss/mnemosyne.git
git fetch upstream
git switch -c validation/native-boundaries 7295b4e23bf435942a4a630be4c43d0c51f182d5
```

Use topic branches and pull requests to this fork. Keep the initial discussion proposal separate from validation/code changes. For updates, fetch upstream, review the release/diff, merge the chosen upstream revision into an update branch, and rerun boundary checks before merging. Avoid force-pushing shared branches. General fixes may be proposed upstream through a separately reviewed PR; no upstream submission is implied by work here.

Internal planning stays in the team's private planning repository and Linear. Do not copy customer memories, credentials, meeting transcripts, internal financial details or private links into this public fork. Use synthetic fixtures and public technical evidence.
