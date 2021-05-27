
# Falco Community Call

[More Information](https://github.com/falcosecurity/community)
[Zoom Link](https://zoom.us/my/cncffalcoproject)
[Recording](https://)

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

- Massimiliano Giovagnoli ([@maxgio](https://github.com/maxgio92))

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
