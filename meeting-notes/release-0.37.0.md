# Falco Community Call

[More Information](https://github.com/falcosecurity/community)
[Zoom Link](https://zoom.us/my/cncffalcoproject)
[Recording](https://youtube.com/playlist?list=PLgVVUpW8NIJAaZtszf1_nxB2y6mQrlY4s)

## 2024-01-24

### MC

- Nigel Douglas

### Who joined

- [Federico Di Pierro](https://github.com/fededp)
- [Mike Coleman](https://github.com/mikegcoleman)
- [Leonardo Grasso](https://github.com/leogr)
- [Angelo Puglisi](https://github.com/deepskyblue86)
- [Thomas Labarussias](https://github.com/Issif)
- [Aldo Lacuku](https://github.com/alacuku)
- [Roberto Scolaro](https://github.com/therealbobo)
- [Teryl Taylor](https://github.com/terylt)

### Weekly highlights

- Some polls:
    - https://github.com/falcosecurity/falco/discussions/3023
    - https://github.com/falcosecurity/falco/discussions/3025

### Agenda

- [Thomas Labarussias] Tracking of download stats with [scarf](https://about.scarf.sh/) p2
- Falco 0.37 release is on track
    - Released `falcoctl` https://github.com/falcosecurity/falcoctl/releases/tag/v0.7.1
    - Released Falco 0.37.0-rc2 yesterday: https://github.com/falcosecurity/falco/releases/tag/0.37.0-rc2
    - Investigating potential performance issue (might delay the release a bit)


## 2024-01-17

### MC

- [Mike Coleman](https://github.com/mikegcoleman)

### Who joined

- [Thomas Labarussias](https://github.com/Issif)
- [Federico Di Pierro](https://github.com/fededp)
- [Roberto Scolaro](https://github.com/therealbobo)
- Melissa Kilby ([@incertum](https://github.com/incertum))
- [Leonardo Grasso]([@leogr](https://github.com/leogr))
- [Mike Coleman](https://github.com/mikegcoleman)
- [Luca Guerra](https://github.com/LucaGuerra)
- [Aldo Lacuku](https://github.com/alacuku)
- Dirk Marwinski
- [Mark Stemm](https://github.com/mstemm)

### Weekly highlights

### Agenda

- [Thomas Labarussias] Tracking of download stats with [scarf](https://about.scarf.sh/)
    - Scarf is a service that allows the tracking of download statistics
    - Can be used to figure out what drivers are being downloaded etc to help with prioritization
    - Thomas is leading the PoC if you have any feedback questions
- [Melissa Kilby @incertum] Discuss on host anomaly detection proposal https://github.com/falcosecurity/falco/pull/2655#issuecomment-1832871000. 
    - Dedicated HackMD doc https://hackmd.io/Ss0_1avySUuxArBQm-oaGQ?view.
    - Record of Melissa's talk at KubeCon NA 2023 https://www.youtube.com/watch?v=1y1m9Vz93Yo
- Dirk discussed rolling out Falco to SAP and their Gardner-based K8s environments. Experiencing some issues, so hoping to get involved here to get some help (dropped events, crashes, etc.)


## 2024-01-10

### MC

- [Andreagit97](https://github.com/Andreagit97)

### Who joined

- [Thomas Labarussias](https://github.com/Issif)
- [Andreagit97](https://github.com/Andreagit97)
- [Aldo Lacuku](https://github.com/alacuku)
- [Roberto Scolaro](https://github.com/therealbobo)

### Weekly highlights

- [Andrea] Falco 0.37.0 tracking issue
    - https://github.com/falcosecurity/falco/issues/3003
    - follow it to receive updates on the release
- [Andrea] k8s plugin integration with Falco 0.36.2
    - the old k8s enrichment was not working correctly so we replaced it in Falco 0.37.0 with a plugin + a remote collector (called k8s-metacollector)
    - plugin repo: https://github.com/falcosecurity/plugins/tree/master/plugins/k8smeta
    - k8s-metacollector repo: https://github.com/falcosecurity/k8s-metacollector
    - the `k8smeta` plugin + the `k8-smetacollector` will be officialy released with Falco 0.37.0 as **EXPERIMENTAL** features. We have a custom helm chart to test the integration of these components with Falco 0.36.2, so you can help us to test the new features at scale -> https://github.com/falcosecurity/charts/tree/master/charts/k8s-metacollector
    - Read more here: https://github.com/falcosecurity/falco/issues/2973

### Agenda

- 

## 2024-01-03

### MC

- [Andreagit97](https://github.com/Andreagit97)

### Who joined

- [Federico Di Pierro](https://github.com/fededp)
- [Aldo Lacuku](https://github.com/alacuku)
- [Adao Oliveira Junior](https://github.com/junior)
- [Roberto Scolaro](https://github.com/therealbobo)
- [Mike Coleman](https://github.com/mikegcoleman)
- [Andreagit97](https://github.com/Andreagit97)

### Weekly highlights

- [Andrea] Libs release 0.14.1
    - we will use it for Falco 0.37.0
    - tracking issue: https://github.com/falcosecurity/libs/issues/1608
- [Andrea] proposal to set the modern ebpf driver as the default driver in our documentation:
    - https://github.com/falcosecurity/falco-website/issues/1229
    - maybe we could create a documentation page with all the common issues and how to solve them: https://github.com/falcosecurity/falco/issues/2873

### Agenda

- Happy 2024! :D 

## 2023-12-20

### MC
- [Thomas Labarussias](https://github.com/Issif)

### Who joined

- [Aldo Lacuku](https://github.com/alacuku)
- [Roberto Scolaro](https://github.com/therealbobo)
- [Andreagit97](https://github.com/Andreagit97)
- [Leonardo Grasso](https://github.com/leogr)
- [Federico Di Pierro](https://github.com/fededp)

### Weekly highlights

- Features Adoption and Deprecation Policies Proposal (Request for comment)
    - https://github.com/falcosecurity/falco/pull/2986/files
- Libs 0.14.0 is out!
    - https://github.com/falcosecurity/libs/releases/tag/0.14.0
    - it will be used by Falco 0.37.0. It's also possible that we will use a patch release so something like 0.14.1
- Need to start (once) again the Contributor of the Month
- No call next week, have great Christmas and New Eve (next call 3rd of Jan, 2024)

### Agenda

- https://falco.org/docs/contribute/contributor-of-the-month/
    - proposed Aldo and Andrea

## 2023-12-13

### MC
- [Andreagit97](https://github.com/Andreagit97)

### Who joined
- [Thomas Labarussias](https://github.com/Issif)
- [Mike Coleman](https://github.com/mikegcoleman)
- [Aldo Lacuku](https://github.com/alacuku)
- [Federico Di Pierro](https://github.com/fededp)
- [Roberto Scolaro](https://github.com/therealbobo)

### Weekly highlights

- [Andrea] Release libs 0.14.0
    - we will try to tag it within this week or early next week
    - might be included in Falco 0.37
- [FedeDP] Falco master images now ship new falcoctl driver loader. GIVE IT A SPIN!
- [Andrea] update on k8s plugin
    - PR for the integration inside plugin repo: https://github.com/falcosecurity/plugins/pull/378

### Agenda
- 


## 2023-12-06

### MC
- [Mike Coleman](https://github.com/mikegcoleman)

### Who joined

- [Roberto Scolaro](https://github.com/therealbobo)
- [Luca Guerra](https://github.com/LucaGuerra)
- [Mike Coleman](https://github.com/mikegcoleman)
- [Pablo Musa](https://github.com/pmusa)
- [Aldo Lacuku](https://github.com/alacuku)
- [Andreagit97](https://github.com/Andreagit97)
- [Thomas Labarussias](https://github.com/Issif)


### Weekly highlights

- [Andrea] Release libs 0.14.0
    - we are a little bit late due to some fixes and some open discussions

### Agenda
- [Mike] Falco documentation process 
    - A process to ensure that Falco docs stay in sync with any new or update features
    - https://github.com/falcosecurity/falco/issues/2951


## 2023-11-29

### MC
- [Mike Coleman](https://github.com/mikegcoleman)

### Who joined

- [Roberto Scolaro](https://github.com/therealbobo)
- [Mike Coleman](https://github.com/mikegcoleman)
- [Aldo Lacuku](https://github.com/alacuku)
- [Vicente J. Jiménez Miras](https://github.com/vjjmiras)
- [Thomas Labarussias](https://github.com/Issif)
- [Dmitrii](https://github.com/erthalion)
- [Aizhamal](https://github.com/aijamalnk)
- [Adao Oliveira Junior](https://github.com/junior)

### Weekly highlights

- [Andrea] Release libs 0.14.0
    - we are a little bit late due to some fixes and some open discussions

### Agenda
- [Nigel] Docs restructure
    - Context: to make it easier to navigate the install guides. Most of the content exists, it is matter of moving content to make them more discoverable. 
    - Main parts of docs affected: 
        - Install and operate
        - Plugins 
    - https://github.com/falcosecurity/falco-website/issues/1206
    - https://github.com/falcosecurity/falco-website/issues/1207
    - Mike: to socialize it in Slack
- [Dmitrii] Allow loading tracepoints other than the ones needed by Falco #1376
    - Context: using custom attachment point on Falco fork
    - https://github.com/falcosecurity/libs/issues/1376
- [Aizhamal] https://thomas.labarussias.fr/falco-rules-explorer/index.html 
    - Thomas: Trying to donate to falco/security organization and make it part of the falco.org



## 2023-11-22

### MC
- [Federico Di Pierro](https://github.com/fededp)

### Who joined

- [Federico Di Pierro](https://github.com/fededp)
- [Aldo Lacuku](https://github.com/alacuku)
- [Roberto Scolaro](https://github.com/therealbobo)
- [Mike Coleman](https://github.com/mikegcoleman)
- [Pablo Musa](https://github.com/pmusa)
- [Andreagit97](https://github.com/Andreagit97)

### Weekly highlights

- Weekly highlights become a (hopefully) weekly blog post! https://falco.org/blog/falco-w-46/
- drver-loader embedded into falcoctl PR is now merged -> https://github.com/falcosecurity/falcoctl/pull/343 `falcoctl driver printenv`

### Agenda

- [Andrea] Release libs 0.14.0
    - we are a little bit late due to some fixes and some open discussions
- [Aldo] falcoctl artifact manifest/config commands:
    - https://github.com/falcosecurity/falcoctl/pull/340
    - https://github.com/falcosecurity/falcoctl/pull/351
- [Andrea] Kudos to Aldo for the new k8s-metacollector repo :heart: 
    - https://github.com/falcosecurity/k8s-metacollector

## 2023-11-15

### MC

- [Andreagit97](https://github.com/Andreagit97)

### Who joined

- [Andreagit97](https://github.com/Andreagit97)
- [LucaGuerra](https://github.com/LucaGuerra)
- [Federico Di Pierro](https://github.com/fededp)
- [Aldo Lacuku](https://github.com/alacuku)
- [Roberto Scolaro](https://github.com/therealbobo)
- [Teryl Taylor](https://github.com/terylt)
- [Vicente J. Jiménez Miras](https://github.com/vjjmiras)
- [Pablo Musa](https://github.com/pmusa)

### Weekly highlights

- [Luca] KubeCon presence
    - We had two talks on Falco, maintainer track + detection talk, will add the links once available
    - https://kccncna2023.sched.com/event/1R2oH/avoid-an-ill-wind-and-catch-the-jet-stream-using-falco-to-detect-attackers-compliance-violations-jason-dellaluce-leonardo-grasso-luca-guerra-sysdig-melissa-kilby-apple-carlos-tadeu-panato-junior-chainguard
    - https://kccncna2023.sched.com/event/1R2mX/a-wind-of-change-for-threat-detection-melissa-kilby-apple
- [Andrea] support to powerpc for modern ebpf and riscv64 for kernel module
    - almost untested but at least it should compile and run
 
### Agenda

- [Andrea] Release libs 0.14.0
    - target releease day 24th of November
    - we will release a dev Falco build with this libs tag to test the new plufin for Kubernetes enrichment
