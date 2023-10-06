# 2023-10-05 Falco Core Maintainers (monthly)

## MC

Melissa Kilby ([@incertum](https://github.com/incertum))

## Who Joined

- Melissa Kilby ([@incertum](https://github.com/incertum))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Massimiliano Giovagnoli ([@maxio92](https://github.com/maxgio92))
- Federico Di Pierro [@fededp](https://github.com/fededp)
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Luca Guerra ([@LucaGuerra](https://github.com/LucaGuerra))

## Highlights

- CNCF Licesing issues:
    - https://github.com/cncf/foundation/issues/645
    - https://github.com/cncf/foundation/issues/629
    - CNCF is going to evaluate them in Oct

## Agenda


Notes:

- Discuss CNCF TAG Environmental Sustainability, Green Review WG
  - https://github.com/cncf/tag-env-sustainability/issues/183#issuecomment-1704313320
  - https://github.com/cncf/tag-env-sustainability/issues/183#issuecomment-1742310582
  - https://github.com/cncf/tag-env-sustainability/issues/182#issuecomment-1743250546 adjust our kernel-testing Ansible setup for Green Review WG setup (still empty, see https://github.com/cncf-tags/green-reviews-tooling)
  - Discuss: Do we need a new repo for all this on Falco side? Similar to the kernel version testing?
  - Context: This is a high-visibility, high-priority issue for the CNCF ecosystem, Falco users, and Falco itself. Performance overhead is a top concern, even before considering other capabilities.
  - Proposed timeline for e2e v1 January 2024: Need to budget accordingly.
  - Related: https://github.com/falcosecurity/libs/issues/1347 Enhanced libs stats / metrics, related to tracking down current and possible future memleak issues
  - Related: Container engine testing https://github.com/falcosecurity/libs/issues/1298
  - Summary of guidance we will provide:
    - Clarify how project's binaries are intended to be run? On the bare-metal host, in simple VMs or Kubernetes where for example daemonset deployment for Falco can be an option 
    - Propose configuration options
- Discuss high priority Falco 0.37 tasks
    - k8s client -> top priority for Falco 0.37
      - https://github.com/falcosecurity/libs/issues/987 
      - it should faster than container runtime, because the api server is queried before the first syscall is run
      - currently -k parses every message (JSON) from the api server and even needs jq extension which we confidentally identify as huge overhead
      - in the future have k8s client and container engine as plugins and have them both read/write to a shared container/pod state table
  - ia32 support
      - https://github.com/falcosecurity/libs/pull/1196
  - finalizing metrics and Green Review CI, see above (@incertum extend metrics and postpone libsinsp interface refactor later @jasondellaluce)
  - libsinsp cleanups?
      - mesos client
      - old k8s client (remove once we have new one Falco 0.37)
      - udig
  - falcoctl as driver loader (in flight @LucaGuerra)
      - https://github.com/falcosecurity/falcoctl/issues/327
  - Create formal deprecation policies document https://github.com/falcosecurity/.github/issues/115
- Discuss tasks that span Falco 0.38 and beyond
  - e.g. when will LSM hooks become a reality? -> open* syscalls and symlinks for open* syscalls as primary use case (replace syscalls open* in that case)
  - Work on DNS?
  - Other kernel signals we need more urgently?
  - New issue to facilitate a discussion https://github.com/falcosecurity/falco/issues/2857
- Discuss Deprecations and additional necessary cleanups
  - Falco 0.37 https://github.com/falcosecurity/falco/issues/2763
    - Consider to deprecate exceptions? They are not user-friendly right now -> No, make them better instead and incorporate other expression language issues into this workstream @jasondellaluce https://github.com/falcosecurity/falco/issues/2858)
  - Falco 0.38 https://github.com/falcosecurity/falco/issues/2840
- Falco rules maturity framework and configs:
  - -t/-T etc move to falco.yaml https://github.com/falcosecurity/falco/issues/2717
  - Consolidated new approach to allow rules overrides or partial overrides https://github.com/falcosecurity/falco/issues/1340, https://github.com/falcosecurity/falco/pull/2671 
      - [leogr] I would like to see this in 0.37
      - [incertum] @jasondellaluce will do it
