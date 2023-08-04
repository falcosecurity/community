# 2023-08-03 Falco Core Maintainers (monthly)

## MC

- leogr

## Who Joined

- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Luca Guerra ([@LucaGuerra](https://github.com/LucaGuerra))
- Melissa Kilby ([@incertum](https://github.com/incertum))
- Massimiliano Giovagnoli ([@maxgio92](https://github.com/maxgio92))
- Grzegorz Nosek ([gnosek](https://github.com/gnosek))
- Mauro Moltrasio ([#molter73](https://github.com/molter73))
- Andrea 


## Agenda

- [luca,leogr,melissa] Publishing rules 2.x for Falco 0.36.0
    - Should we publish three different flavors: _stable_, _incubating_, _sandbox_ or all together?
    - incertum: added new agreement to existing Phase 4 ticket, see https://github.com/falcosecurity/rules/issues/126

From https://github.com/falcosecurity/rules/blob/main/proposals/20230605-rules-adoption-management-maturity-framework.md
> Furthermore, we will start by implementing tagging for the rules and establishing new guides. Subsequently, we will gather feedback from the community. In the future, we believe it would be beneficial to divide the rules files into separate entities: falco_rules.yaml (keeping the old established file name for the stable rules), falco_rules.incubating.yaml, falco_rules.sandbox.yaml, and falco_rules.deprecated.yaml. However, since this change could potentially disrupt some adopters and result in breaking changes to the order in which rules are loaded, we believe it is necessary to prioritize other improvements first. For instance, we may need to introduce features such as allowing multiple rules to match on a single event or providing the ability to customize the loading order, to name just a few. 

- Target this for 0.36.0 and start advertise users?
    - ok for Luca
    - we have enough features in Falco to manage the rules tags we need
        - incertum: need minor adjustments as outlined in https://github.com/falcosecurity/falco/issues/2717
    - We need to expose the Falco tag option in the Falco yaml

- [luca] Falco images
    - for context https://github.com/falcosecurity/falco/tree/master/docker#readme
    - updating the driver loader image
        - falcosecurity/falco-driver-loader-legacy (with the current img)
        - falcosecurity/falco-driver-loader (with the updated image)
        - idea: tag them separately and keep adding
    - falcosecurity/falco? (with the updated image?)
    - using a more minimal image for no-driver (wolfi)
        - [luca,maxgio] can we ship two images (wolfi+debian) until we're sure in experimental mode?
        - we can proceed
- [luca,maxgio] re-releasing plugins+rules
    - We will re-publish them either way
    - Let's do it closer to the release
    - Let's do this end of august / early september for pre-releases to test the CI and continue with all plugins
- [leogr] third-party dependencies clean-up
    - [jasondellaluce] avocado-framework -> remove python regression tests
        - after that, we can also remove some CircleCI jobs
        - this was already planned when we started working on the new testing framework
        - https://github.com/falcosecurity/falco/pull/2716
    - UBI (never published, never got an answer about licensing)
        - https://github.com/cncf/foundation/issues/362
- Moving to 0.37
    - postponing falco-driver-loader deprecation (this means rewriting the script not deprecating the functionality)
        - https://github.com/falcosecurity/falco/blob/master/proposals/20221129-artifacts-distribution.md#deprecate-falco-driver-loader
    - postponing new k8s client
- [leogr] FYI: the CNCF is working to a _License exception for dual-licensed GPL-2.0 + approved license for in-kernel eBPF programs_
    - but did not include kernelmodule
    - https://github.com/cncf/foundation/issues/474#issuecomment-1650271054
    - working to address this
- [incertum] Falco Rules Modernization w/ Red Team input (tighter recommendations wrt control plane / k8s audit logs <-> syscalls correlations off host)
    - Work with some red teamers and check scenarios
    - Add more recommendation to the documentation (falco.org/docs , new rules in the repo or description in the rules)
    - @leogr improve docs on website wrt deployment of plugins on control node of cluster vs DaemonSet / syscalls monitoring on the knodes
- [incertum] Try improving container engine (adopters face many null image fields during any time of the lifetime)
    - It's not just the event happening close to the start of the container
    - We need to dive deeper to understand exactly when this happens
    - https://github.com/falcosecurity/falco/issues/2700 
- [incertum] Memory leaks in Falco? Keep investigating ...
    - First step check on output queue capacity, if this is not it, keep looking
    - https://github.com/falcosecurity/falco/pull/2711
    - https://github.com/falcosecurity/falco/issues/2495
