
## 2021-06-09

### MC
- POP ([POP](https://github.com/danpopsd))

### Who joined
- Pablo Lopez ([@pabloopez](https://github.com/pabloopez/))
- Stefan Uygur ([@ostendali](https://github.com/ostendali))
- Alba Ferri ([@alba-ferri](https://github.com/alba-ferri/))
- Alejandro Villanueva ([@seishinsha](https://github.com/seishinsha/))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- [Cash Williams](https://github.com/cashwilliams)

### This week highlights


### Agenda

- Allow Issif to be maintainer of falco-website
  - POP +1 
- Add tags in falco output  (tagging @leogr for response in subsequent meetings)
- Discuss timeframe/alternatives around issue #778
- [Release 0.29.0](https://github.com/falcosecurity/falco/issues/1668) postpone due to prebuilt drivers build delay ([fix](https://github.com/falcosecurity/test-infra/pull/422), [issue](https://github.com/falcosecurity/test-infra/issues/421)). Blocking updates:
  - [May 27th updates](https://github.com/falcosecurity/test-infra/pull/411)
  - [June 2nd updates](https://github.com/falcosecurity/test-infra/pull/417)
  - [June 6th updates](https://github.com/falcosecurity/test-infra/pull/419)
- [pablopez] Labs status update: under review + embed [proposal](https://kubernetes.slack.com/files/U01UC42UZFC/F024VEW15FB/jun-09-2021_13-32-34.mp4)
    - prepare a new blogpost: expl
    - new lab: basic rule creation
    - more ideas? -> ask in the channel
- [pop] Contributor of the Month Reminder (announcing the winner 6/16) 
- [alejandro] MITRE ATT&CK matrix for containers. Work done so far to map it to Falco rules https://docs.google.com/spreadsheets/d/1lK2luf4iuOHDJEZ9EGcv3DkuuHeyRJAfeBzQCu2AuUI/edit#gid=0 
    - All contributions welcome.
- [Stefan] Logging question about 0.28.2
    - https://github.com/falcosecurity/falco/releases shows 0.28.1 as latest release, but yum and deb have 0.28.x released.
- [Stefan] falco installation script obsoleted, would like to maintain as it is very useful

## 2021-05-26

### MC

 - Leonardo Di Donato

### Who joined

- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Loris Degioanni ([@ldegio](https://github.com/ldegio))
- POP ([POP](https://github.com/danpopsd))
- [Ginny Ghezzo](https://github.com/gghezzo)
- [Gus Parvin](https://github.com/gparvin)
- [Vicente Herrera](https://github.com/vicenteherrera/)
- Ali Bulut([@aliblt](https://github.com/aliblt))
- Pablo Lopez ([@pabloopez](https://github.com/pabloopez/))

### This week highlights

- [0.28.2 Falco release in the making!](https://github.com/falcosecurity/falco/issues/1653)

### Agenda

- [leodido] Proposal regarding a versioning and release process for `falcosecurity/libs`
- [jscrivanich] Bug with new systemd falco installation on AMIs that don't have systemd
    - [falco#1625](https://github.com/falcosecurity/falco/issues/1625)
    - [leogr/leodido] likely we don't want to officially support initd anymore
    - [leogr] Proposed workaround: write examples/tutorial how to add an initd configuration manually
- We should remove https://github.com/falcosecurity/falco-website/tree/master/static/script (since it's not tested anymore, likely broken)
- [gparvin] Update from Policy workgroup
- [pablopez] Falco labs update [here](https://github.com/pabloopez/katacoda-scenarios). 
    - [Reviewer](https://github.com/pomyslowynick)
    - Website embed
    - To update the issue
    - OWNERS

## 2021-05-19

### MC

- POP ([@danpopsd](https://github.com/danpopsd))

### Who joined
- [Vicente Herrera](https://github.com/vicenteherrera/)
- [Ginny Ghezzo](https://github.com/gghezzo)
- [Cash Williams](https://github.com/cashwilliams)
- [POP](https://github.com/danpopsd))
- [Loris Degioanni](https://github.com/ldegio)
- [Edvin Norling](https://github.com/NissesSenap)
- [Massimiliano Giovagnoli](https://github.com/maxgio92)
- [Magno Logan](https://github.com/magnologan)
- [Shane Lawrence](https://github.com/shane-lawrence)
- [Ali Bulut](https://github.com/aliblt)
- [Gus Parvin](https://github.com/gparvin)
- [Leonardo Grasso](https://github.com/leogr)
- [Sruthy Santhosh](https://github.com/sruthy-santhosh)
- [Lorenzo Fontana](https://github.com/fntlnz)

### This week highlights


### Agenda

- [Vicente Herrera] New MITRE ATT&CK matrix for containers. Work done so far to map it to Falco rules https://docs.google.com/spreadsheets/d/1lK2luf4iuOHDJEZ9EGcv3DkuuHeyRJAfeBzQCu2AuUI/edit#gid=0 
- [loris] https://github.com/falcosecurity/libs/pull/40  (Parametrize the metadata download PR)
    - Other complementary approaches:
        - [leogr] Filtering by node https://github.com/falcosecurity/libs/issues/43
        - [zemek] Get k8s pod metadata and namespace name from container labels https://github.com/falcosecurity/libs/pull/15
- [pop] ArgoCD  Falco Blog 
- Community Open Floor


## 2021-05-12

### MC

Massimiliano Giovagnoli ([@maxgio](https://github.com/maxgio92))

### Who joined

- [Thomas Labarussias](https://github.com/Issif)
- Pablo Lopez ([@pablopez](https://github.com/pabloopez))
- Stefano Chierici ([@darryk10](https://github.com/darryk10))
- [Cash Williams](https://github.com/cashwilliams)
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- POP ([@danpopsd](https://github.com/danpopsd))
- Stefan Uygur ([@ostendali] (https://github.com/ostendali))

- [Ginny Ghezzo](https://github.com/gghezzo)
- Gus Parvin ([@gparvin](https://github.com/gparvin))
- Leonardo Di Donato ([@leodido](https://github.com/leodido))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Massimiliano Giovagnoli ([@maxgio](https://github.com/maxgio92))

### This week highlights

- Falco 0.28.1 is out!
    - Thanks Carlos for leading the releaaaaase!

### Agenda

- [developer-guy]falco-hot-reloader: A Proof Of Concept project about adding hot-reloading support to Falco using sidecar container concept in Kubernetes environment: [Github Repository](https://github.com/developer-guy/falco-hot-reload-with-sidecar)
- [leogr] 0.28.2 Release
    - Initially proposed by [leodido] and discussed in [falco #1635](https://github.com/falcosecurity/falco/issues/1635#issuecomment-833338118)
    - [falco #1552](https://github.com/falcosecurity/falco/pull/1552) depends on
        - [libs #42](https://github.com/falcosecurity/libs/pull/42)
        - [libs #30](https://github.com/falcosecurity/libs/pull/30)
    - *TODO:* add the new driver version on our DBG (once libs' PRs get merged)
    - We need a release team
        - Max to lead!
- [leodido/loris] improvements to the k8s metadata fetching in the Falco libs
    - [falco #778](https://github.com/falcosecurity/falco/issues/778)
    - [libs #40](https://github.com/falcosecurity/libs/pull/40)
    - what I'll do on Falco side
- [Issif] New blog post for creation of a Response Engine with falcosidekick and Knative (thanks to @n3wscott)
- [Issif] I'm asking for a vote to add @developper-guy as official maintainer for falcosidekick
    - [leogr] +1
    - Approved.
- [pablopez] [Katacoda Portal](https://www.katacoda.com/falco/courses/falco) Learning environments: katacoda maintenance & proposals (see [evolution #70](https://github.com/falcosecurity/evolution/issues/70))
- [darryk10] New proposal default minimal falco_rules.yaml or split rules by technology or MITRE ATT&CK Category (see [falco #1584](https://github.com/falcosecurity/falco/issues/1584), [falco #1627](https://github.com/falcosecurity/falco/issues/1627), [falco #1646](https://github.com/falcosecurity/falco/issues/1646))
- [Gus] Adoption investigation: Generate PolicyReport from alerts (see [PolicyReports](https://github.com/kubernetes-sigs/wg-policy-prototypes/tree/master/policy-report))
- [pop] New Adopters!  [Replicated](https://github.com/falcosecurity/falco/commit/601ec5cf856620dcea466725d9fafb0edcb5d829#diff-12e0a48d6c5f2a58f4caa284b0546243f1a5431590701dd26e9c4f94180127e6), [Yahoo! JAPAN](https://github.com/falcosecurity/falco/commit/0f36ff030e269008f99cd280a62d4dfbd58aadad#diff-12e0a48d6c5f2a58f4caa284b0546243f1a5431590701dd26e9c4f94180127e6)

## 2021-04-28

### MC

- Jonah Jones ([@jonahjon](https://github.com/jonahjon))

### Who joined

- Jonah Jones ([@jonahjon](https://github.com/jonahjon))
- POP ([@danpopsd](https://github.com/danpopsd))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Ginny Ghezzo ([@gghezzo](https://github.com/gghezzo))
- Cash Williams ([@cashwilliams](https://github.com/cashwilliams))
- Gus Parvin ([@gparvin](https://github.com/gparvin))
- Leonardo Di Donato ([@leodido](https://github.com/leodido))

### This week highlights

- Maintainers for Falco talking at Kubecon Booth
- Translation for Falco highlight 
- Jonah - brought everyone up to date on sandbox projects
- Gus Parvin (Red Hat) - discussing the Falco Operator and how Red Hat to contribute back to it.   Evolution suggested - https://github.com/falcosecurity/evolution

### Agenda

- [leodido] Updates about the graduation process
- Sandbox credits (Working on 2 paths 1st for marketing credits (6 months) for ASAP graduation, 2nd is for long term tech credits that don't expire)
- Open Floor



## 2021-04-21

### MC

- Leonardo Grasso ([@leogr](https://github.com/leogr))


### Who joined

- Michele Zuccala ([@zuc](https://github.com/zuc))
- Loris Degioanni ([@ldegio](https://github.com/ldegio))
- Leonardo Di Donato ([@leodido](https://github.com/leodido))
- Stefan Uygur ([ostendali](https://github.com/ostendali))
- Jonah Jones ([@jonahjon](https://github.com/jonahjon))


### This week highlights

- Falco applied for the CNCF graduation [cncf/toc#641](https://github.com/cncf/toc/pull/641)


### Agenda

- Plan release 0.28.1 with the community (ask over slack who wants to be part of the release team)
- Organizational vote
    - https://github.com/falcosecurity/.github/pull/43
- AWS credits for running test-infra expired
    - jonah is helping!



### Closing

- **MC Next Call**: 
- **Next Release**: 
    - Falco 0.28.1 planning to be released in May

## 2021-04-14

### MC
- Carlos Panato ([@cpanato](https://github.com/cpanato))


### Who joined

- Loris Degioanni ([@ldegio](https://github.com/ldegio))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- POP ([@danpopsd](https://github.com/danpopsd))
- Natch Ruengsakulrach ([@natchaphon-r](https://github.com/natchaphon-r))
- Jonah Jones ([@jonahjon](https://github.com/jonahjon))
- Daniele Divito([@danieledivito](https://github.com/danieledivito))
- Ali Bulut([@aliblt](https://github.com/aliblt))
- Leonardo Di Donato ([@leodido](https://github.com/leodido))
- Ricardo Katz ([@rikatz](https://github.com/rikatz))

### This week highlights


### Agenda

- [Loris Degioanni] Plugin system proposal and demo
    - Incubation request for related projects [evolution#62](https://github.com/falcosecurity/evolution/issues/62)
- New Members
    - Natch, Ricardo and Ali
- Contributor of the Month Revealed!
- Falco 0.28 released!
    - [Changelog](https://github.com/falcosecurity/falco/releases/tag/0.28.0)
    - [Blogpost](https://falco.org/blog/falco-0-28-0/)
- Falco wants to apply for CNCF graduation
    - Maintainers will communicate a task list soon

### Closing

- **MC Next Call**: 
- **Next Release**: 
    - Falco 0.28.1 planning to be released in May
---
