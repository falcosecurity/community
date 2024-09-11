# 2024-09-05 Falco Core Maintainers (monthly)

## MC

- Luca Guerra

## Who Joined

- leogr ([@leogr](https://github.com/leogr))
- LucaGuerra ([@LucaGuerra](https://github.com/LucaGuerra))
- Mauro Moltrasio ([@molter73](https://github.com/Molter73))
- Aldo Lacuku ([@alacuku(https://github.com/alacuku)])
- Federico Di Pierro ([@fededp](https://github.com/fededp))
- Grzegorz Nosek ([@gnosek](https://github.com/gnosek))
- Samuel Gaist ([@sgaist](https://github.com/sgaist))
- Thomas Labarussias([@Issif](https://github.com/Issif))

## Agenda

- Falco 0.39 release updates (new features below)
    - Release manager: Aldo Lacuku
- New options
    - https://github.com/falcosecurity/falco/pull/3308 "append_output"
    - https://github.com/falcosecurity/falco/pull/3310 -o x={object}
    - JSON modifying options [to-do]
- Docker images: https://github.com/falcosecurity/falco/issues/3165
    - [FedeDP, leogr] most likely to be postponed to 0.40.0
- falco.yaml validation
- Metrics improvements: https://github.com/falcosecurity/falco/issues/3309
    - [leo] let's keep those incubating and later stable
    - [Grzeg] should be enter and exits be an aggregate?
        - Yes
- Libs 0.18.0
    - basename() transformer
    - regex operator
    - proc.{stdin,stdout,stderr}.{name,type} https://github.com/falcosecurity/libs/pull/1916
    - `dirfd` and `fs.*` improvements: https://github.com/falcosecurity/libs/pull/1993
    - linux 6.11 support
    - dynamic snaplen improvements -> https://github.com/falcosecurity/libs/pull/2006, https://github.com/falcosecurity/libs/pull/2035
    - new fields proc.is_exe_lower_layer, fd.is_upper_layer and fd.is_lower_layer https://github.com/falcosecurity/libs/pull/1936
- Status of high-level goals (as per our [1.0 roadmap](https://falco.org/docs/roadmap/) )

| Area | Goal | Status |
| -------- | -------- | -------- |
| **Engine**     | adoption and depreciation policies     | a bit late     |
|      | Streamlining falco.yaml structure     | not started     |
|      | CLI args consolidation and standardization     | in progress     |
|      | Advanced metrics support     | In a good shape, stable tenatively for 0.40     |
| **Syntax**     | language inconsistencies arising from our commitment to backward compatibility     | a bit late     |
|     | new constructs     | in progress     |
| **Drivers**     | Make the modern eBPF probe the default driver     | Done in 0.38     |
| **Distribution**     | Packages consolidation     | not started     |
|      | Publish signatures for drivers and all packages    | partially done     |
|      | Make the Falco default image a "no-driver"/"distroless" image    | in progress, tentatively for 0.40     |
|      | supply chain security best practices    | unsure, need review     |
| **Documentation**     | Better documentation around our feature adoption and deprecation policies     | not started     |
|      | Improve troubleshooting guide    | unsure, need review     |
|      | Enhance guidance on operationalizing and responding to Falco alerts based on adopters' feedback    | not started    |
|      | Revamp and enhance documentation for non-Kubernetes use cases (i.e. Falco installed on a Linux host)    | in progress    |
| **Integrations**     | Improve stability in the container runtime integration    | tenatively for 0.40     |
|      | Provide deeper access from the Plugin Framework to the Falco stream of events to make Falco more modular and easier to extend    | in progress     |
- [proposal] Falco 1.0 release schedule
    - Release 0.39 (2024 sept) and 0.40 (2025 jan) as usual
    - Release 1.0:
        - WHAT: same feature set of 0.40 + [Breaking changes for 1.0](https://github.com/falcosecurity/falco/issues/3038)
        - WHEN: one-off release close to KubeconEU 2025 (April), then we will continue with the usual release schedule (ie. 1.1 in May, 1.2 in Sept, etc...)
    - Notes:
        - this is a tenatively release schedule, we can postpone it if not ready in time
        - no annoncement until the 1.0 is in a good shape
