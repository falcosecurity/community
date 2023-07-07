# 2023-07-06 Falco Core Maintainers (monthly)

## MC

- Luca

## Who Joined

- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Mauro Moltrasio ([@molter73](https://github.com/Molter73))
- Jason Dellaluce ([@leogr](https://github.com/jasondellaluce))
- Federico Di Pierro ([@fededp](https://github.com/fededp))
- Luca Guerra ([@LucaGuerra](https://github.com/LucaGuerra))
- Melissa Kilby ([@incertum](https://github.com/incertum))

## Agenda

- [luca] Falco 0.36.0 proposed roadmap items

**Graduation items as requested by TOC** 
(see: https://github.com/falcosecurity/evolution/issues/281)
- Rule maturity framework
    - https://github.com/falcosecurity/rules/pull/76
    - TOC recommended timeline: **May-July 2023**
- Kernel version testing
    - https://github.com/falcosecurity/libs/pull/1131
    - TOC recommended timeline: **May-August 2023**
- Document API and data flow boundaries between userspace and kernel
    - https://github.com/falcosecurity/libs/issues/1189
    - TOC recommended timeline: **May-July 2023**

**Falco 0.36.0 items**
- Symlink bypass solution
    - https://github.com/falcosecurity/falco/issues/2203
    - https://github.com/falcosecurity/libs/issues/1111
- DNS parsing improvements
    - See Shopify comment, Lorenzo's and Melissa's discussion
- cgroups v2 support
    - https://github.com/falcosecurity/libs/pull/1058
- Finalize metrics feature, see other related items under (already in progress captured by jason)
- Signatures & verification for plugins & rules
    - https://github.com/falcosecurity/plugins/issues/244
    - https://github.com/falcosecurity/falcoctl/issues/174
    - https://github.com/falcosecurity/rules/issues/65
- Inconsistent process hierarchy in thread tables
    - https://github.com/falcosecurity/libs/pull/1182
- Container image work (+supply chain)
    - https://github.com/falcosecurity/evolution/issues/261
- Allow multiple rules to match an event (opt-in)
    - https://github.com/falcosecurity/falco/issues/1542
- Upgrade OpenSSL to v3.x in Falco and libs
    - https://github.com/falcosecurity/libs/issues/1038
- Deprecate falco-driver-loader
    - https://github.com/falcosecurity/falco/blob/master/proposals/20221129-artifacts-distribution.md#deprecate-falco-driver-loader
- Windows + MacOS CI for Falco
    - Allows plugin consumers to run and test on non-linux environments
    - Enhances developer experience
    - https://github.com/falcosecurity/falco/issues/2672
- Enhancing kubernetes metadata acquisition
    - https://github.com/falcosecurity/libs/issues/987
- Solving issues and add features in Falco's rule language
    - Select a part of the issues that fit into the release

**Discussion**
- We may want to expand the concept of kubernetes metadata acquisition to other platform (using plugins)
- User asked about "merging" rules, [@molter73] suggests using a rule as a prerrequisite for another rule might make more sense in order to prevent a breaking change. This would be similar to using a macro to copy the same conditions over to multiple rules, but only output an event for the rule that closest matches the event.

## Action items:

- [ ] update the Roadmap GitHub Project
    - https://github.com/orgs/falcosecurity/projects/5
- [ ] Falco’s rule language and rules loading management (DevOps): Select a part of the issues that fit into the release
    - Melissa and Jason?
        - https://github.com/falcosecurity/falco/issues/2127 "Access to more variables in output_fields" -> callout to support `append` option for `output` as well, addressed in https://github.com/falcosecurity/falco/pull/2671, TODO check on plugins support for this? https://github.com/falcosecurity/falco/issues/2289
        - https://github.com/falcosecurity/falco/issues/1340 Allow for partial override of properties, TODO first decide on design and this is related to this issue https://github.com/falcosecurity/falco/issues/2477 and also to this one https://github.com/falcosecurity/falco/issues/2541
        - https://github.com/falcosecurity/falco/issues/2480 a global redefinition of additional outputs fields based on a specific tag, see also https://github.com/falcosecurity/falco/issues/2127#issuecomment-1611143944 TODO after first PR is merged.
        - Only load rules with a certain tag that reflects hostgroups, see https://github.com/falcosecurity/falco/issues/2660, while it may sound like an edge case, Melissa rates this as highly important for DevOps as in Kubernetes settings you typically only have the option to ship one rules definition to different clusters and different monitoring for some hostgroups not just highly desired, but can also be necessary to successfully use Falco.
        - All of the above issues are examples that highlight (1) inconsistencies and (2) major pain points for adopters in terms of managing Falco rules and using Falco effectively. In order to ensure a positive user experience we need to address them in a reasonable order and time frame.
        - Inconsistent priority on enabling a rule in the YAML file and by using the CLI `-T` / `-t` / `-D` selectors

- [ ] Review https://github.com/falcosecurity/rules/pull/76
    - We agree to split rule files
    - If split in 0.36 we have to advertise users
