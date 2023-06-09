# 2023-06-08 Falco Core Maintainers (monthly)

## MC

- leogr

## Who joined

- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Melissa Kilby ([@incertum](https://github.com/incertum))
- Jason Dellaluce([@jasondellaluce](https://github.com/jasondellaluce))
- Massimiliano Giovagnoli ([@maxgio92](https://github.com/maxgio92))
- Grzegorz Nosek ([gnosek](https://github.com/gnosek))
- Andrea
- Luca

## Agenda

- [luca] **[Roadmap WG](https://github.com/falcosecurity/falco/blob/master/proposals/20230511-roadmap-management.md#next-steps-and-conclusions)**
    - introduction and scoping
    - to update https://github.com/orgs/falcosecurity/projects/5/views/7

- **Falco 0.36 [Roadmap Planning](https://github.com/falcosecurity/falco/blob/master/proposals/20230511-roadmap-management.md#roadmap-planning)**
    > The onus is on the Core Maintainers to manage the roadmap. In this regard, Core Maintainers meet in planning sessions on the first week of each calendar month.
    > 
    > During these planning sessions, tasks are allocated to the current iteration or postponed to one of the following iterations. The assigned iteration indicates the projected completion date for a particular workstream.
    > 
    > When a session matches with the commencement of an iteration, maintainers convene to assess the planning and prioritize tasks for the iteration. **The first planning session of a release cycle must define top priorities for the related release.**

- [melissa] **Proposals that aim to address action items proposed by our TOC sponsors for graduation:**
    1. Kernel version testing https://github.com/falcosecurity/libs/pull/1131
        - TOC recommended timeline: **May-August 2023**
    2. Rules Maturity and Adoption https://github.com/falcosecurity/rules/pull/76
        - TOC recommended timeline: **May-July 2023**

- [melissa] proposed herself as an approver for rules and falco
    - we also need other approvers

- [jason/luca] **Proposed roadmap items**
  - Deprecate falco-driver-loader
      - https://github.com/falcosecurity/falco/blob/master/proposals/20221129-artifacts-distribution.md#deprecate-falco-driver-loader
  - Container image vulnerability issues (Supply Chain Security)
    - https://github.com/falcosecurity/evolution/issues/261
    - https://github.com/falcosecurity/falco/issues/2489
    - https://github.com/falcosecurity/falco/issues/2181
    - https://github.com/falcosecurity/falco/issues/2580 (conflicting need)
  - Continuing Supply Chain Security topics
    - Signatures & verification for missing artifacts
    - SLSA Provenance Attestations
  - Consolidate end-to-end testing framework for Falco, falcoctl, plugins
    - https://github.com/falcosecurity/testing
    - [melissa] to remove from 0.36 or postpone
    - [andrea] just postpone the enrichment of tests
    - [jason] at least python tests should be replaced
  - K8S Metadata Client refactor and improvements
    - https://github.com/falcosecurity/libs/issues/987
  - DNS parsing improvements (Melissa's & Lorenzo's discussion, adopter's interview feedback)
      - Shopify
      > They would love to see Falco enrich DNS information beyond the existing attempts to resolve DNS through name-resolver.
      - [melissa] to prioritize this
  - Symlink bypass solution through new kernel hook points
    - https://github.com/falcosecurity/falco/issues/2203
    - https://github.com/falcosecurity/libs/issues/1111
    - [melissa] to prioritize this

- [jason] **Already in progress/to be finalized:**
  - Finalize work on plugin framework
    - Plugin SDK C++ to become official and support low-level features (syscall events, thread table access)
    - Logging API: https://github.com/falcosecurity/libs/issues/989
    - Native metrics API: follow-up to Melissa's work on libs  
  - Finalize work on native libs metrics
    - Add Prometheus exporter in Falco
    - Finalize API on libsinsp
  - Various PRs pending in Falco and libs https://github.com/falcosecurity/falco/pulls?q=is%3Aopen+is%3Apr+milestone%3A0.36.0
      - [andrea]  Introduce a coding style for libs
          - https://github.com/falcosecurity/libs/pull/470

- [jason] **Known relevant problems (for the long term):**
  - Solving issues and add features in Falco's rule language:
    - https://github.com/falcosecurity/plugins/issues/206
    - https://github.com/falcosecurity/falco/issues/510
    - https://github.com/falcosecurity/falco/issues/1332
    - https://github.com/falcosecurity/falco/issues/1338
    - https://github.com/falcosecurity/falco/issues/1340
    - https://github.com/falcosecurity/falco/issues/1542
    - https://github.com/falcosecurity/falco/issues/1695
    - https://github.com/falcosecurity/falco/issues/1736
    - https://github.com/falcosecurity/falco/issues/1814
    - https://github.com/falcosecurity/falco/issues/1859
    - https://github.com/falcosecurity/falco/issues/2127
    - https://github.com/falcosecurity/falco/issues/2279
    - https://github.com/falcosecurity/falco/issues/2354
    - https://github.com/falcosecurity/falco/issues/2372
    - https://github.com/falcosecurity/falco/issues/2477
    - https://github.com/falcosecurity/falco/issues/2484
    - https://github.com/falcosecurity/falco/issues/2486
    - https://github.com/falcosecurity/falco/issues/2541
    - [melissa] https://github.com/falcosecurity/falco/issues/2403
  - Inconsistent process hierarchy in thread tables
      - [andreagit97] https://github.com/falcosecurity/libs/issues/1139
      - https://github.com/falcosecurity/libs/issues/1011
      - [melissa] will picky-back on this effort to enhance a few things relevant to enhance usability of the state from a feature perspective
  - [melissa, fededp] 32-bit support
      - https://github.com/falcosecurity/falco/issues/2472
      - https://github.com/falcosecurity/libs/issues/279
      - https://github.com/falcosecurity/libs/issues/1045
  - cgroup v2
      - https://github.com/falcosecurity/libs/pull/1058
      - [andrea] to prioritize this
      - [grzeg] pr is wip but mostly complete
          - testing in progress
  - Stabilization, clean-up, and finalization of libsinsp and libscap code and APIs
      - [melissa] scap refactoring?
      - [grzeg] 3 platform PRs not ready yet
          - on hold until we have a clear picture
          - this should not be a blocker for any release
- [melissa] **Proposed roadmap items**
    - Melissa to propose herself as falco and rules approver
    - [melissa] on-host anomaly detection / advanced behavior analysis
      - Proposal against libs repo to be compiled by Jun 19, 2023 with details and initial explorations. Treat is similarly to how we introduced modern_bpf. Tangential work in the background, not influencing Falco 0.36 at all and hopefully be ready for experimental release for Falco 0.37. Aimed to extend the state engine tangentially, not a plugin, introduce probabilistic data structures and new way of information processing (opt-in even for compilation only similar to gvisor).
      - [jason] why not a plugin?
          - [melissa] we need to discuss
          - [jason] we can revamp the Plugin SDK C++
  - [melissa, jason] finalize metrics feature, see other related items under (already in progress captured by jason)
      - cleanup old stats and/or adopt some of the old currently not used libsinsp metrics for the new metrics framework as well.
  - [melissa, andrea] -> see an item below also check on some state inconsistencies from a feature and usability perspective, picky-back on Andrea's work
  - [melissa] -> Work on LSM hooks and DNS led by Lorenzo and others would really be great.
  - [melissa] -> check with Grezg on cgroup work and check for inconsistencies for some container engines. 
  - [melissa + others] check on officially supported build container for modern bpf and ensure it's easya nd straight forward to compile, create an official new guid for building in containers in general.

- [grzeg] layered approach to improve libs code/API
    - [everyone] ok with introducing the layerd approach first if it does not break anything
    - [grzeg] not a short-term thing, depends on the platform PRs
    - not a priority, this must not be a blocker for any release

## Action items

- [ ] [luca] create a Slack channel for the roadmap WG
- [ ] Roadmap WG to process the output of this call
    - see items with a priority note
