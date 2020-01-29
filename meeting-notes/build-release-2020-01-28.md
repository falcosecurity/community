# Build/Release Infrastructure Call

[More Information](https://github.com/falcosecurity/community)

## 2020-Jan-28


### MC

- Lorenzo Fontana ([@fntlnz](https://github.com/fntlnz))

### Who joined

- Kris Nova ([@kris-nova](https://github.com/kris-nova))
- Leonardo Di Donato ([@leodido](https://github.com/leodido))
- Marky Jackson ([@markyjackson-taulia])(https://github.com/markyjackson-taulia)
- Pierre Lacerte ([@ephemeral](https://github.com/ephemeral))
- Néstor Salceda ([@nestorsalceda](https://github.com/nestorsalceda))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Zachary Estrella ([@zestrells](https://github.com/zestrells))
- Suresh Palemoni ([@sureshpalemoni] https://github.com/sureshpalemoni)

### This week highlights

- News, shoutouts, updates

### Agenda

- [Nova] Welcome, and reminder that we need to start small
- [Nova] Make a decision if we want to keep doing prebuilt probes for everyone or we prefer to build a more stable local build experience
- [Lore] Discussion/decision on eBPF
    - How do we build/support kernel modules and eBPF probe?
    - Problem: Missing probes and modules in S3, unable to build locally (missing kernel headers)
    - Problem: Unable to build every permutation of OS/Arch/Kernel and support them
    - Problem: Building locally is complicated and undocumented
    - There is some work done with running a VM to help wih the build
    - [Lore/Nova] Proposal to start a new project/API/service to consume /proc/config.gz and system info to build modules and probes as needed
    - [Nova] Please can we get better at probe/module nomenclature
    - [Nova] Do we have Falco and Falcoctl help out with user experience with this new service?
    - See the [slack thread](https://sysdig.slack.com/archives/C19S3J21F/p1579805707105600&thread_ts=1579805005.101500&cid=C19S3J21F) for more information.
    - [Nova] Open issue/proposal
- [Nova] Discussion about init containers for Falco
    - See issue [#1019](https://github.com/falcosecurity/falco/issues/1019)
    - See [slack with @mstemm](https://sysdig.slack.com/archives/C19S3J21F/p1579808765119300?thread_ts=1579808342.116100&cid=C19S3J21F)
- [Leo] Bring the build/release process completely in the open
    - Current process described [**here**](https://hackmd.io/QH08H-6QQnuebvYuPO8bTw)
    - Initial proposal for an "open" build/release process in [issue 726](https://github.com/falcosecurity/falco/issues/726)
        - What we need:
        - Signing (GPG) probes and packages
        - DEB/RPM repositories
        - Probe's service
- [Nova] Issue with hosting BPF Probes
    - See issue [#1021](https://github.com/falcosecurity/falco/issues/1021)
- [Lore] APT/RPM packages hosting
    - One of the missing pieces for release automation
- [Lore] Push docker images for maintainer's PRs and for our branches
    - Makes testing easier
    - Useful point for release automation
- [Lore] dev branch to become master branch
    - [Leo] explaination in issue [726](https://github.com/falcosecurity/falco/issues/726#issuecomment-535621850)
    - [Leo] Announce to the mailing list what is going to happen, when, and how
- [Leo] CNCF.CI is already being worked on
    - https://github.com/crosscloudci/falco-configuration
    - [Leo] Ask via the mailing list what are the next steps to put Falco on cncf.ci
- [Leo] Do we really want/need to pay for CircleCI plan?
    - Docker layer caching needs "performance" plan
- [Nova] Notify folks we have a build/release channel


### Closing

**Recording**: [Play](https://www.youtube.com/watch?v=HUR_HWJZ7yc)
**MC Next Call**: Kris Nóva