# 2023-12-14 Falco Core Maintainers (monthly)

## MC
- leogr

## Who Joined

- Melissa Kilby ([@incertum](https://github.com/incertum))
- Massimiliano Giovagnoli ([@maxgio92](https://github.com/maxgio92))
- Andrea Terzolo ([@Andreagit97](https://github.com/Andreagit97))
- Grzeg
- Luca

## Highlights

## Agenda

- **[URGENT]** `libelf` license exception request follow-up from CNCF 
    - Their **question**:
        - *Is it technically possible for Falco to instead dynamically link to libelf, so that the libelf library remains separable from Falco at runtime?*
    - Proposed **answer**:
        - Yes, it is technically feasible and already possible if users build Falco from the source.
        - However, Falco dynamically linked to libelf may have compatibility issues and create more burdens for adopters. For these reasons, we currently distribute Falco artifacts with libelf statically linked. Disallowing us to distribute Falco statically linked to libelf will have the following effects:
             - Users that intend to install Falco on the host will be forced to install libelf by themselves.
             - Compatibility issues may arise with different versions of libelf
             - We currently distribute different flavors of the Falco binary, one is based on MUSL and completely statically linked. We will find ourselves forced to interrupt the distribution of this flavor.
         - Question for the Legal Committee: Would it be acceptable to distribute both dynamically and statically linked binaries so users can choose which to use? AFAIK this fully aligns with LGPL requirements.
     - **Agree?**
         - leo agrres
         - andrea agrees
         - luca agrees
         - melissa agrees
         - max agrees
         - Gzreg agrees
- Deprecate/Archive https://github.com/falcosecurity/kilt
    - 2 out of 3 maintainer inactive for more than 1 year
    - no supported use cases
    - **Agree?**
        - everybody agrees
- Create new repo [cncf-green-review-testing](https://github.com/falcosecurity/evolution/issues/345)
    - **Agree?**
        - everybody agrees
- Canceling the Jan 4th meeting
   - **Agree?**
       - Melissa agrees
       - Andrea agrees
       - Luca agrees
       - Max agrees
       - Grzeg agrees
- `libs` 0.14.0 release for Falco 0.37.0, no libs 0.15.0 release for Falco -> discuss outstanding PRs
    - https://github.com/falcosecurity/libs/pull/1575
    - https://github.com/falcosecurity/libs/pull/1561 (under evaluation)
        - we may tag it as experimental
- New k8s plugin status update
    - https://github.com/falcosecurity/plugins/pull/378
- Discuss oustanding tasks for Falco 0.37.0 (including docs updates and ensuring all items we want to deliver are on track)
    - Luca working on https://github.com/falcosecurity/falco/issues/1340
    - Mike will help with documentation for new features
        - He will be release manager shadow
        - Luca will work with him
- Schedule PR reviews for PRs or issues that have not been given priority:
  - Discuss general sustainable path forward for massive servers (21+ Million events/s)
    - https://github.com/falcosecurity/libs/issues/1376 (Allow loading tracepoints other than the ones needed by Falco). Kindly asking core maintainers to stay open minded and support iterative progress.
    - https://github.com/falcosecurity/libs/issues/1557 (Introduce conditional kernel-side event filtering) Related to driver modernization above.
    - https://github.com/falcosecurity/falco/issues/2960 ([DISCUSSION] New base_syscalls.exclude_enter_exit_set config)
    - https://github.com/falcosecurity/libs/pull/1375 (wip: feature(scap): allow custom tracepoints on ebpf probe)
  - https://github.com/falcosecurity/falco/pull/2413 (new: driver selection in falco.yaml) in general check in on status and future of driver loader
  - https://github.com/falcosecurity/falco/pull/2655 (docs(proposals): introduce on host anomaly detection framework)
  - https://github.com/falcosecurity/libs/pull/1452 (new(driver): kmod configure system)
  - https://github.com/falcosecurity/libs/pull/1393 (Silence missing BPF program error)
- IMPORTANT: we need criteria for prioritization
    - For example, Falco vs. libs use cases
    - How to plan design decision?
SKIPPED:
- libs coding style: https://github.com/falcosecurity/libs/issues/381, https://github.com/falcosecurity/libs/pull/470
- Discuss falco and metrics output sinks: https://github.com/falcosecurity/libs/issues/1463#issuecomment-1809354692 [if time permits] 
