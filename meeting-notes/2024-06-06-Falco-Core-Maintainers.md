# 2024-06-06 Falco Core Maintainers (monthly)

## MC

- leogr

## Who Joined

- Melissa Kilby ([@incertum](https://github.com/incertum))
- Mauro Moltrasio ([@molter73](https://github.com/molter73))
- Luca Guerra([LucaGuerra](https://github.com/LucaGuerra))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))

## Agenda

- Falco 0.38.1 (hotfix)
    - https://github.com/falcosecurity/falco/pulls?q=is%3Apr+milestone%3A0.38.1
    - pending:
        - enable plugins metrics https://github.com/falcosecurity/falco/pull/3228
        - workaround for -pk bug https://github.com/falcosecurity/falco/pull/3239
- Entering 0.39 Development iteration
    - Reference: 1.0.0 Roadmap https://falco.org/docs/roadmap/#road-to-falco-1-0-0
        - TODO: we should update the page marking what was already delivered by 0.38
    - Streamlining container images ([issue](https://github.com/falcosecurity/falco/issues/3165)) [in roadmap]
    - Additional outputs in the configuration file ([issue](https://github.com/falcosecurity/falco/issues/3235)) [in roadmap]
    - Performance testing for us maintainers + CNCF Green Reviews Perf Testing
        - dogfooding environment
            - may we use test-infra?
        - Green Review exploring how to benchmarking
    - Transformer and Operator flexibility ("any/all" in lists) [in roadmap] + output fields formatting, e.g. process lineage bash->python->sh
        - leogr will come with a proposal for oneof/anyof/allof
        - bash->python->sh can be addressed by `join()`
            - `join(proc.foo, "->") contains bash->python`
            - mentioned in https://github.com/falcosecurity/libs/pull/1625
    - vpckg for dependency management
        - cmake compatible
        - SBOM
    - Security: signatures for drivers [in roadmap]
        - No secure boot (likely not doable)
    - Fix all pending metrics issues (see [here](https://github.com/falcosecurity/falco/issues/3194)) + discuss metrics needed for existing metrics categories or new categories still needed (e.g. syscalls counters)
        - syscalls counters on the kernelside?
        - Grafana dashboard
        - deprecation of falco-exporter
        - goal for 0.39: to make Metrics stable
    - Expand drivers testing even more
        - complex test in CI?
        - run tests on demand?
    - CRI container engine, further improvements [issue](https://github.com/falcosecurity/libs/issues/1589) (e.g. self healing, more metrics on failures)
    - Ideas/TBD
        - generate inline docs from falco.yaml
        - we may provide a simple builder image for falco
            - https://github.com/falcosecurity/falco/blob/master/.github/workflows/reusable_build_packages.yaml#L55
- How to collect data about the state of used drivers?
    - Is it time to evaluate legacy eBPF maintaince mode?
- [Proposal] Kernel-side filtering https://github.com/falcosecurity/libs/pull/1867/files
    - Give feedback
    - Evaluate
- Skip July and Aug calls?
    - all in favor
