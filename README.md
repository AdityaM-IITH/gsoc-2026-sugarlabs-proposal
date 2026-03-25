# GSoC 2026 Proposal -- Music Blocks Maintenance

**Organization:** Sugar Labs
**Project:** Music Blocks Maintenance
**Mentors:** Walter Bender, Om Santosh Suneri
**Length:** 150 hours (Medium, 12 weeks)

---

## About Me

- **Name:** Aditya Mishra
- **GitHub:** [AdityaM-IITH](https://github.com/AdityaM-IITH)
- **Matrix:** @AdityaM-IITH:matrix.org
- **Email:** adityamishra13r@gmail.com
- **Institution:** IIT Hyderabad
- **Program:** B.Tech, Electrical Engineering (1st year)
- **Time Zone:** IST (UTC +05:30)

---

## Proposal

👉 [View Full Proposal (PDF)](./GSoC-Proposal.pdf)

---

## Summary

Music Blocks v3 is actively maintained while v4 is in development. The
codebase has accumulated dependency debt and the architecture has grown
monolithic in places -- both of which make changes risky without a solid
test safety net. Over the past several weeks I built out Jest unit tests
and a Cypress E2E suite to provide that safety net. The GSoC project uses
it to do the harder work: systematic dependency upgrades and targeted
modularization of large files like `activity.js` and `blocks.js`.

---

## Pre-GSoC Contributions

### Merged

| PR | Description |
|----|-------------|
| [#6138](https://github.com/sugarlabs/musicblocks/pull/6138) | Cypress E2E refactor: removed hard waits, added `waitForAppReady` |
| [#6043](https://github.com/sugarlabs/musicblocks/pull/6043) | boundary.js: image onload callback coverage |
| [#6021](https://github.com/sugarlabs/musicblocks/pull/6021) | IntervalsBlocks.js unit tests |
| [#6004](https://github.com/sugarlabs/musicblocks/pull/6004) | turtledefs Music Blocks mode unit tests |
| [#6001](https://github.com/sugarlabs/musicblocks/pull/6001) | JSInterface validateArgs unit tests |
| [#5977](https://github.com/sugarlabs/musicblocks/pull/5977) | p5-sound-adapter: 0% → 100% coverage |
| [#5924](https://github.com/sugarlabs/musicblocks/pull/5924) | Fix blockList reference in setMasterVolume |
| [#5907](https://github.com/sugarlabs/musicblocks/pull/5907) | Turtle class unit tests |

### Open (Awaiting Review)

| PR | Description | Coverage |
|----|-------------|----------|
| [#6357](https://github.com/sugarlabs/musicblocks/pull/6357) | PenBlocksAPI.js | 94.28% → 100% |
| [#6356](https://github.com/sugarlabs/musicblocks/pull/6356) | export.js (58 tests) | 86.61% → 100% |
| [#6284](https://github.com/sugarlabs/musicblocks/pull/6284) | performanceTracker.js (22 tests) | 0% → 88% |
| [#6262](https://github.com/sugarlabs/musicblocks/pull/6262) | Dependency updates: cypress, i18next, jest-environment-jsdom, sass | -- |
| [#6143](https://github.com/sugarlabs/musicblocks/pull/6143) | Cypress: Block Palette interaction tests (19/19) | -- |
| [#6114](https://github.com/sugarlabs/musicblocks/pull/6114) | tempo.js | 92.89% → 100% |
| [#6108](https://github.com/sugarlabs/musicblocks/pull/6108) | planetInterface.js | 91.85% → 100% |
| [#6099](https://github.com/sugarlabs/musicblocks/pull/6099) | MediaBlocks.js | 90.82% → 99.51% |
| [#6083](https://github.com/sugarlabs/musicblocks/pull/6083) | ToneBlocks.js | 93.85% → 96.11% |
| [#6082](https://github.com/sugarlabs/musicblocks/pull/6082) | MeterBlocks.js | 94.38% → 98.59% |
| [#6048](https://github.com/sugarlabs/musicblocks/pull/6048) | EnsembleBlocks.js | 93.88% → 98.21% |
| [#6047](https://github.com/sugarlabs/musicblocks/pull/6047) | BoxesBlocks.js | → 100% |
| [#6046](https://github.com/sugarlabs/musicblocks/pull/6046) | status.js | 98.24% → 100% |
| [#6042](https://github.com/sugarlabs/musicblocks/pull/6042) | pitchslider.js | 99.02% → 100% |
| [#6041](https://github.com/sugarlabs/musicblocks/pull/6041) | OrnamentBlocks.js | 92% → 100% |
| [#6028](https://github.com/sugarlabs/musicblocks/pull/6028) | activity-context.js | 0% → 88.88% |
| [#6026](https://github.com/sugarlabs/musicblocks/pull/6026) | minify.js | 0% → 100% |

---

## Feedback

I would appreciate feedback from mentors on:
- Scope and feasibility of the modularization targets
- Timeline -- specifically whether the dependency work is correctly sized for weeks 1-4
- Any areas I have missed or should prioritize differently
```
