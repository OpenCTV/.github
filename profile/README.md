<picture>
  <source media="(prefers-color-scheme: dark)" srcset="openctv-lockup-white.svg">
  <img alt="OpenCTV" src="openctv-lockup-light.svg" height="48">
</picture>

**Find the first place a CTV ad transaction stops agreeing with itself.**

One streaming ad break passes through an ad server, a stitcher, a manifest, a player and a stack of beacons, and each keeps its own record. OpenCTV lines those records up as one transaction, finds the earliest point where they diverge, and explains what that costs in delivery, measurement and billing.

### Components, in shipping order

| Repo | Status | What it does |
| --- | --- | --- |
| `divergence-library` | In progress | How CTV ad transactions go wrong, plus the shared schemas |
| `hls-manifest-diff` | Next | Compare two HLS manifests by meaning, not text |
| `stream-fixtures` | Planned | Reproducible broken streams, each tied to a library entry |
| `cuechain` | Planned | One ad break signal, followed across every cue |
| `openctv` | Planned | One command, one report, one evidence chain |

Releases ship when they install clean, the quickstart works and the tests pass. There are no dates on the roadmap.

[openctv.org](https://openctv.org) · hello@openctv.org

Maintained by [Prashant Chaudhary](https://prashantchaudhary.com). Sister project: [ReachPost](https://reachpost.org). Apache-2.0 for code, CC-BY-4.0 for the library, schemas and fixtures. Not affiliated with any standards organization.
