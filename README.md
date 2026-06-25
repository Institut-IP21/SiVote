<div align="center">

# SiVote

**Open-source secret-ballot voting for organizations — understandable, auditable, no blockchain.**

The home of the SiVote platform: an internet voting system built for **private, democratic
organizations** (associations, cooperatives, unions, parties). Self-host it with no GUI, or use the
hosted GUI at [eGlasovanje.si](https://eglasovanje.si). Built by the non-profit [IP21](https://ip21.si).

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

</div>

---

## Why SiVote

- **Secret** — voters vote with random, single-use codes; there is no stored link between a voter and
  their vote.
- **Verifiable** — every voter receives the full anonymized list of submitted ballots and can check,
  with their own code, that their vote was recorded and the tally is correct. Because each voter holds
  their own copy, a falsified result can't be shown selectively — no cryptography degree required.
- **Understandable** — no blockchain, no exotic cryptography. Transparency through simplicity.
- **Secrecy that scales** — three [security levels](https://eglasovanje.si/nivoji-varnosti), from
  fully platform-run to a setup where your electoral commission distributes codes and proxies vote
  submission so the platform never sees the voter at all.
- **A complete, dependable solution** — create ballots, verify voters, collect votes, publish results,
  add your logo (revolutionary, we know). Production software with a support organization behind it,
  not an experiment.

> **Not for state elections — on principle.** The authors are opponents of e-voting for governmental
> elections: there it adds critical risks and no real benefit. SiVote is for private organizations
> where remote secret voting genuinely helps.

## The repositories

| Repo | Role |
| --- | --- |
| [SiVoteEngine](https://github.com/Institut-IP21/SiVoteEngine) | Core: ballots, single-use voting codes, vote collection, results. |
| [SiVoteSender](https://github.com/Institut-IP21/SiVoteSender) | Voter lists, email invitations, verification, delivery tracking. |
| [SiVoteHomeSender](https://github.com/Institut-IP21/SiVoteHomeSender) | Standalone CLI for an electoral commission to distribute invites from its own machine (Level 2/3). |

The graphical web app at eGlasovanje.si is a separate, proprietary product built on top of these.

## How it works

The Engine generates one random code per voter; the Sender — or, at Level 2/3, your commission via
SiVoteHomeSender — emails each voter their code and a ballot link. Voters cast in a browser on any
device. When voting closes, the Engine tallies the result and every voter is emailed the full
anonymized ballot list to independently verify their vote and the count.

## Run it yourself

Self-host with just the Engine + Sender (no GUI) and operate it via the `evote:*` artisan CLI — see the
Engine's [self-hosting guide](https://github.com/Institut-IP21/SiVoteEngine/blob/master/docs/SELF_HOSTING.md)
and [security & secrecy model](https://github.com/Institut-IP21/SiVoteEngine/blob/master/docs/SECURITY_MODEL.md).
Or skip the ops and use the hosted GUI at [eGlasovanje.si](https://eglasovanje.si) (free for smaller
organizations).

## License & support

MIT (see each component repository). _eGlasovanje_ is a trademark of [IP21](https://ip21.si). Questions
or support: **info@ip21.si**. We've published articles explaining the model in depth at
[eglasovanje.si/vsi-clanki](https://eglasovanje.si/vsi-clanki).
