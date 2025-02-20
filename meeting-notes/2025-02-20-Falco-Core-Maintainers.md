# 2025-02-20 Falco Core Maintainers (monthly)

## MC

- Leonardo Grasso

## Who Joined

- leogr ([@leogr](https://github.com/leogr))
- Luca Guerra ([@LucaGuerra](https://github.com/LucaGuerra))
- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Grzegorz Nosek ([@gnosek](https://github.com/gnosek))
- Mauro Moltrasio ([@molter73](https://github.com/molter73))

## Agenda

- Main projects for 0.41
    - [aldo] [K8s operator](https://github.com/alacuku/falco-operator/)
        - First release, around 0.41, as experimental!
    - [FedeDP] [Reimplement containers metadata support as a plugin](https://github.com/falcosecurity/falco/issues/3403)
- [leogr] Status of high-level goals (as per our [1.0 roadmap](https://falco.org/docs/roadmap/) )

| Area | Goal | Status |
| -------- | -------- | -------- |
| **Engine**     | adoption and depreciation policies     | delayed     |
|      | Streamlining falco.yaml structure     | in progress     |
|      | CLI args consolidation and standardization     | done     |
|      | Advanced metrics support     |   stable   |
| **Syntax**     | language inconsistencies arising from our commitment to backward compatibility     | on hold     |
|     | new constructs     | acceptable, but we can do more     |
| **Drivers**     | Make the modern eBPF probe the default driver     | Done in 0.38     |
| **Distribution**     | Packages consolidation     | not started     |
|      | Publish signatures for drivers and all packages    | in progress     |
|      | Make the Falco default image a "no-driver"/"distroless" image    | Done in 0.40     |
|      | supply chain security best practices    | unsure, need review     |
| **Documentation**     | Better documentation around our feature adoption and deprecation policies     | not started     |
|      | Improve troubleshooting guide    | unsure, need review     |
|      | Enhance guidance on operationalizing and responding to Falco alerts based on adopters' feedback    | not started    |
|      | Revamp and enhance documentation for non-Kubernetes use cases (i.e. Falco installed on a Linux host)    | done    |
| **Integrations**     | Improve stability in the container runtime integration    | in progress, see container runtime as a plugin above     |
|      | Provide deeper access from the Plugin Framework to the Falco stream of events to make Falco more modular and easier to extend    | done, but enhancement may be needed      |
- Falco 1.0 release schedule
    - Delayed due to capacity constraints
    - Current plan: just declare 1.0 when all points above are achieved
    - libs 1.0 is unrelated to Falco 1.0, but Falco 1.0 deprecation policy may affect libs development
- [luca] Upcoming Kubecon (London)
    - Talks
        - [Project Lightning Talk: Detect and Respond to Threats in Your Cloud Infrastructure With Falco](https://kccnceu2025.sched.com/event/1tcw6/project-lightning-talk-detect-and-respond-to-threats-in-your-cloud-infrastructure-with-falco-luca-guerra-maintainer)
        - [In the Eye of Falco: Transforming Your View of Linux Kernel Security](https://kccnceu2025.sched.com/event/1tczs/in-the-eye-of-falco-transforming-your-view-of-linux-kernel-security-luca-guerra-jason-dellaluce-aldo-lacuku-leonardo-grasso-sysdig-aurelie-vache-ovhcloud)
    - Project Update Video
        - We are sending a request for KubeconNA (Atlanta), since with new rules we can have 1 slot per year
