## 2026-05-06

### MC

- [Jonas Rosland](https://github.com/jonasrosland)

### Who joined

- [Jonas Rosland](https://github.com/jonasrosland)
- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Libby Schulze](https://github.com/libbyschulze1)
- [Dylan Lee](https://github.com/atleticomadrid07)

## Agenda

- [Prempti](https://prempti.falco.org) launch last week, comments and feedback
- Falco Operator Helm Chart v0.1.0 release:
    -  [Official Installation guide](https://github.com/falcosecurity/falco-operator/blob/main/docs/installation.md)
    -  [Helm chart repo](https://falcosecurity.github.io/charts)

## 2026-05-06

### MC

- [Gerald Combs](https://github.com/geraldcombs)

### Who joined

- [Leonardo Grasso](https://github.com/leogr)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Jonas Rosland](https://github.com/jonasrosland)
- Libby Schulze
- [Mauro Moltrasio](https://github.com/Molter73)

## Agenda

- https://github.com/falcosecurity/prempti (a.k.a coding-agents-kit):
    -  moved into `falcosecurity`
    -  [v0.2.0](https://github.com/falcosecurity/prempti/releases/tag/v0.2.0) released!
- Delivered fix for lack of UTF-8 sanitization
    - [Incosistent string sanitization and missing UTF-8-awareness](https://github.com/falcosecurity/libs/issues/2965)
- Upcoming releases (Libs 0.25.0 and 0.26.0, and Falco 0.44.0)
- Falco Sidekick: we are cooking something cool!
- Let's meet at KCD New York https://kcdnewyork.com/
- CNCF webinar May 12th!
    - [Cloud Native Live: Falco's Nest & the Evolution of Runtime Security
](https://community2.cncf.io/events/details/cncf-cncf-online-programs-presents-cloud-native-live-falcos-nest-amp-the-evolution-of-runtime-security/)
- [Falco Virtual Workshop May 12th!](https://go.sysdig.com/Falco-Virtual-Community-Workshops.html)

## 2026-04-22

### MC

- [Leonardo Grasso](https://github.com/leogr)

### Who joined

- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Jonas Rosland](https://github.com/jonasrosland)
- Libby Schulze
- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Gerald Combs](https://github.com/geraldcombs)

## Agenda

- `coding-agents-kit`
  - [Proposal](https://github.com/falcosecurity/evolution/issues/512)
  - https://github.com/leogr/coding-agents-kit
- Helm Chart for Falco Operator
- [Inconsistent string sanitization and missing UTF-8-awareness](https://github.com/falcosecurity/libs/issues/2965)
- Survey result will be published soon!

## 2026-04-08

### MC

- [Iacopo Rozzo](https://github.com/irozzo-1A)

### Who joined

- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Leonardo Grasso](https://github.com/leogr)

## Agenda

- KubeCon + CloudNativeCon EU 2026 debrief
- Update on [multi-thread initiative](https://github.com/falcosecurity/falco/issues/3749)
- [Falco Operator 0.2.0](https://falco.org/blog/falco-operator-0-2-0/)

## 2026-03-11

### MC

- [Leonardo Di Giovanna](https://github.com/ekoops)

### Who joined

- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Leonardo Grasso](https://github.com/leogr)
- [Gerald Combs](https://github.com/geraldcombs)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Jonas Rosland](https://github.com/jonasrosland)
- Libby Schulze

## Agenda

- BPF iterator Support updates
    - [Tracking issue](https://github.com/falcosecurity/libs/issues/2879)
-  Multi-thread Support updates
    -  Iacopo is evaluating his PoC:
        -  libs code: https://github.com/irozzo-1A/agent-libs/tree/experiment/folly-concurrent-hashmap
        -  falco code: https://github.com/irozzo-1A/falco/tree/experimental/multi-thread
- Falco Operator
    - Repository: https://github.com/falcosecurity/falco-operator
    - Release expected for the next week
- Join us at KubeCon + CloudNativeCon 2026 - Amsterdam, 23-26 March
    - Event link: https://events.linuxfoundation.org/kubecon-cloudnativecon-europe/
    - No community call on 25 March
    - Falco Workshop on Monday March 23: https://sysdig.pathfactory.com/kceu26-falco-workshop
- Falco survey - last day March 13!
    - https://forms.gle/6o6AaWCVa8UAgMcWA

## 2026-02-25

### MC

- [Alessandro Cannarella](https://github.com/c2ndev)

### Who joined

- [Jonas Rosland](https://github.com/jonasrosland)
- [Gerald Combs](https://github.com/geraldcombs)
- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Marko Zbirka]
- [John Bain]
- [Libby Schulze]
- [Kapil Agrawal]


## Agenda

- Multi-thread Support updates: Iacopo will share the latest progress on [multi-thread support for Falco](https://github.com/falcosecurity/falco/issues/3749) 
- Falco Operator: project update and roadmap
- Falco Ecosystem: introducing [falco-lsp](https://github.com/falcosecurity/falco-lsp)
    - Falco Rules VSCode Extension: Alessandro will demo the new VSCode extension for Falco rules
    - Language Server Protocol
- [Falco survey blog post](https://github.com/falcosecurity/falco-website/pull/1533)


## 2026-02-11

### MC

- [Gerald Combs](https://github.com/geraldcombs)

### Who joined

- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Brandt Keller](https://github.com/brandtkeller)
- [Mauro Moltrasio](https://github.com/molter73)
- [Alessandro Cannarella](https://github.com/c2ndev)


## Agenda

- [Libs and plugins changes required for Stratoshark](https://docs.google.com/presentation/d/1NBusHGgGM8DAOLAT8w5fls_Vw7DU_DCw0C6JjR6Igm8/edit?usp=sharing)
- [Offline Documentation and Zarf](https://github.com/zarf-dev/zarf)
