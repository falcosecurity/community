# Falco Community Call

[More Information](https://github.com/falcosecurity/community)
[Zoom Link](https://zoom.us/my/cncffalcoproject)
[Recording](https://youtube.com/playlist?list=PLgVVUpW8NIJAaZtszf1_nxB2y6mQrlY4s)

## 2022-06-01

### MC 

- Aldo Lacuku ([@alacuku](https://github.com/alacuku))

### Who joined

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- David Windsor ([dub](https://github.com/dwindsor))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Fred Araujo ([araujof](https://github.com/araujof))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Vicente Herrera ([@vicenteherrera](https://github.com/vicenteherrera))
- John Brydon ([@johnb](https://github.com/johnbrydon))
- Md Sadun Haq ([@sadunhaq123](https://github.com/sadunhaq123))
- Adao Junior ([junior](https://github.com/junior))

### This week highlights

- [Issif] Helm charts for new releases of Sidekick and Sidekick-UI are up to date
    -  The blog post about these releases is out too https://falco.org/blog/falcosidekick-2-25-0-falco-2-0-0/


### Agenda (Please add any items you would like to discuss here)

- [fededp] Updates on release duties
    - Tracking issue: https://github.com/falcosecurity/falco/issues/1993
    - Release is due to 3rd june
    - Dev builds are here: https://app.circleci.com/pipelines/github/falcosecurity/falco/2584/workflows/aaa60cd7-3b94-4952-868e-cd3c4e105f19/jobs/23635/artifacts
- [jasondellaluce]: proposing myself as a falco-exporter maintainer (https://github.com/falcosecurity/falco-exporter/pull/72)
- [leogr] We are going to refactor the Falco Helm chart
    - First baby-step [charts#340](https://github.com/falcosecurity/charts/pull/340) (still a WIP)

### Closing

- **MC Next Call**: 

## 2022-05-25

### MC 

- Thomas Labarussias ([@Issif](https://github.com/Issif))

### Who joined

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Adao Junior ([junior](https://github.com/junior))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Aldo Lacuku([@alacuku](https://github.com/alacuku))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- David Windsor ([dub](https://github.com/dwindsor))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Fred Araujo ([araujof](https://github.com/araujof))

### This week highlights


### Agenda (Please add any items you would like to discuss here)

- [leogr] Promote Helm Charts/K8s manifests/Plugins to "Official support" [evolution#144](https://github.com/falcosecurity/evolution/issues/144)
    - Sidekick could join Official list too
    - Update helm chart in hub after each release, not only once a week
    - [jasondellaluce] Big +1
- [fededp] Updates on release duties
- Tag/Release for libs is postponed after 0.32
    - everything is ready except CI
    - changes in driverkit have to be made
    - update building system in Falco either
- Arm64 support will be in 0.33 no 0.32 
    - https://github.com/falcosecurity/falco/pull/1990
    - https://github.com/falcosecurity/falco/pull/1997
    - https://github.com/falcosecurity/driverkit/pull/143  
- 0.32 is planned for 3rd of June
- plugin-sdk is updated and compatible with last version of plugin API in Falco > plugins will may not be able to compile
- [jasondellaluce] New GitHub plugin donated to Falcosecurity today! https://github.com/falcosecurity/plugins/tree/master/plugins/github
- [Issif] PR for charts are blocked because CI fails, [example](https://app.circleci.com/pipelines/github/falcosecurity/charts/963/workflows/a5a927aa-1ecb-4be2-b93e-0d7eb0832927/jobs/1780)
- plugin best practices https://github.com/falcosecurity/plugins/blob/master/docs/best-practices.md#plugin-directory-structure
- we're noticing issues with CircleCI, we encourage maintainers to migrate to Github Action or Prow for their projects
    - any help is welcome, a lot to do

### Closing

- **MC Next Call**: Aldo Lacuku([@alacuku](https://github.com/alacuku))

## 2022-05-11

### MC 

- Thomas Labarussias ([@Issif](https://github.com/Issif))

### Who joined

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Aldo Lacuku([@alacuku](https://github.com/alacuku))
- Giles Hutton ([@stringy](https://github.com/stringy))
- Fred Araujo ([araujof](https://github.com/araujof))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))


### This week highlights

- [Andreagit97] Umbrella issue for missing syscalls in Falco ([ISSUE#1998](https://github.com/falcosecurity/falco/issues/1998))
- [Andreagit97] Quick update on the modern BPF probe
    - v-table architecture ([PR#213](https://github.com/falcosecurity/libs/pull/213))
    - base infrastructure and maybe just one syscall
- [jasondellaluce] Thank you Teryl and Fred for your contribution and welcome onboard as maintainers!
    - https://github.com/falcosecurity/libs-sdk-go
    - https://github.com/falcosecurity/evolution/issues/135
- [loresuso] New Falco blog post on how to get started developing Falco
    - https://falco.org/blog/intro-development-falco/
- [Issif] Falcosidekick 2.25.0 on the way out ([PR#317](https://github.com/falcosecurity/falcosidekick/pull/317))
- [Issif] Falcosidekick-UI v2.0.0 :tada: ([Release](https://github.com/falcosecurity/falcosidekick-ui/releases/tag/v2.0.0))

### Agenda (Please add any items you would like to discuss here)

- No community call next week (KubeCon)

### Closing

- **MC Next Call**

## 2022-05-04

### MC 

- Thomas Labarussias ([@Issif](https://github.com/Issif))

### Who joined

- Vicente J. Jimenez Miras ([vjjmiras](https://github.com/vjjmiras))
- Fred Araujo ([araujof](https://github.com/araujof))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Pablo Lopez Zaldivar ([@pabloopez](https://github.com/pabloopez))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Leonardo Grasso ([leogr](https://github.com/leogr))

### This week highlights

- [fededp]: updates on arm64 (driverkit, falco): https://github.com/falcosecurity/driverkit/pull/143
    - kernel crawler has been donated to falcosecurity org and CI is set up https://github.com/falcosecurity/kernel-crawler/tree/main/kernels

### Agenda (Please add any items you would like to discuss here)

- [leogr] volunteering to maintain driverkit [driverkit#140](https://github.com/falcosecurity/driverkit/pull/140)
- [fededp]: proposing myself as release manager for the 0.32
- [@jasondellaluce]: K8S Audit logs became a plugin! https://github.com/falcosecurity/falco/pull/1952
- [leogr] WIP: moving rules files close to plugins

### Closing

- **MC Next Call**

## 2022-04-27

### MC

- Lorenzo Susini ([@loresuso](https://github.com/loresuso))

### Who joined

- Federico Di Pierro ([fededp](https://github.com/fededp))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Fred Araujo ([araujof](https://github.com/araujof))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Leonardo Grasso ([leogr](https://github.com/leogr))


### This week highlights

- fededp: first wip PR to auto generate driverkit configs: https://github.com/falcosecurity/test-infra/pull/684
- LucaGuerra: upcoming gvisor support
- leogr: hot reload in Falco when rules/config changes

### Agenda (Please add any items you would like to discuss here)

### Closing

- **MC Next Call**


## 2022-04-20

### MC

- Vicente J. Jimenez Miras ([vjjmiras](https://github.com/vjjmiras))

### Who joined

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Leonardo Grasso ([leogr](https://github.com/leogr))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Pablo Lopez Zaldivar ([@pabloopez](https://github.com/pabloopez))
- Fred Araujo ([araujof](https://github.com/araujof))

### This week highlights

- libs-sdk from Frederico Araujo & Teryl Taylor

### Agenda (Please add any items you would like to discuss here)

- Mauro Moltrasio: What is the status of the libs repo?
  A: Still work in progress.
- libs-sdk proposal (plan to open a PR in falcosecurity/evolution)
    - https://github.com/sysflow-telemetry/libs-sdk
    - https://github.com/orgs/sysflow-telemetry/packages?repo_name=libs

### Closing

- **MC Next Call**


## 2022-04-13

### MC

- Vicente J. Jimenez Miras ([vjjmiras](https://github.com/vjjmiras))

### Who joined

- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Giles Hutton ([@stringy](https://github.com/stringy))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Adao Junior ([junior](https://github.com/junior))
- Fred Araujo ([araujof](https://github.com/araujof))

### This week highlights

- Andrea Terzolo: Propose myself as a libs repo maintainer
- Jason Dellaluce: Falco is now compiled completely without Lua

### Agenda (Please add any items you would like to discuss here)


### Closing

- **MC Next Call**


## 2022-04-06

### MC

- Vicente J. Jimenez Miras ([vjjmiras](https://github.com/vjjmiras))

### Who joined

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Pablo Lopez Zaldivar ([@pabloopez](https://github.com/pabloopez))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Fred Araujo ([araujof](https://github.com/araujof))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Zsolt NEMETH ([zsmav](https://github.com/zsmav))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Adao Junior ([junior](https://github.com/junior))
- Gerald Combs ([@geraldcombs](https://github.com/geraldcombs))

### This week highlights

### Agenda (Please add any items you would like to discuss here)

- Vicente: Changes in the Website:
  - Include information about Falco Plugins
  - Documentation for Falco Sidekick
  - Survey to gather feedback: https://docs.google.com/forms/d/1V2qbgmzeyP7KHYoGYgZUYfYTFg7puNTESfCy1yqghnY
- Phoenix operator sidecar for Falco
- Jason: refactorings of Falco rule engine
    - https://github.com/falcosecurity/libs/pull/217 (already merged)
    - https://github.com/falcosecurity/falco/pull/1965
    - https://github.com/falcosecurity/falco/pull/1966
- Gerald: Shared libraries for falcosecurity/libs
    - https://github.com/falcosecurity/libs/pull/276

### Closing

- **MC Next Call**: 


## 2022-03-30

### MC

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))

### Who joined

- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- David Windsor ([dub](https://github.com/dwindsor))
- Andrea Bonanno ([andreabonanno](https://github.com/andreabonanno))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Giles Hutton ([@Stringy](https://github.com/Stringy))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Vicente J. Jimenez Miras ([vjjmiras](https://github.com/vjjmiras))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Fred Araujo ([araujof](https://github.com/araujof))

### This week highlights

- Okta Plugin for Falco: https://falco.org/blog/falco-okta-plugin/
- New bpf probe proposal: https://github.com/falcosecurity/libs/pull/268
- New driverkit builder for Rocky Linux: https://github.com/falcosecurity/driverkit/pull/130

### Agenda (Please add any items you would like to discuss here)

- Running integration tests on libs using sinsp-example
    - https://github.com/Molter73/falco-libs-qa
- Ubuntu driverkit fix
  - https://github.com/falcosecurity/driverkit/issues/127
  - https://github.com/falcosecurity/driverkit/issues/126

### Closing

- **MC Next Call**: 

## 2022-03-23

### MC

- Thomas Labarussias ([@Issif](https://github.com/Issif))

### Who joined

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Leonardo Grasso ([leogr](https://github.com/leogr))
- Pablo Lopez Zaldivar ([@pabloopez](https://github.com/pabloopez))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Giles Hutton ([@Stringy](https://github.com/Stringy))
- Andrea Bonanno ([andreabonanno](https://github.com/andreabonanno))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Vicente J. Jimenez Miras ([vjjmiras](https://github.com/vjjmiras))
- Fred Araujo ([araujof](https://github.com/araujof))

### This week highlights


### Agenda (Please add any items you would like to discuss here)

- Teryl: working (closed for now) on wrapper for Falco API in Go, used for Sysflow integration
- Giles: benchmark between kmod and ebpf probe: https://kubernetes.slack.com/files/U03234VD3GW/F038A94NF5Y/falco_ebpf___kernel_module_performance.pdf
- Contributor of the Month (Jan/Feb): Alban Créquy, for his work on Falco plugin for seccompagent. congrats

### Closing

- **MC Next Call**: 

## 2022-03-16

### MC

- Teryl Taylor ([terylt](https://github.com/terylt))

### Who joined

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Adao Junior ([junior](https://github.com/junior))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Fred Araujo ([araujof](https://github.com/araujof))
- Leonardo Grasso ([leogr](https://github.com/leogr))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Andrea Bonanno ([andreabonanno](https://github.com/andreabonanno))


### This week highlights


### Agenda (Please add any items you would like to discuss here)

- [Molter73] Is there any plans/ideas on tagging the libs repository?
    - https://github.com/falcosecurity/libs/blob/master/proposals/20210524-versioning-and-release-of-the-libs-artifacts.md#the-plan
    - https://github.com/falcosecurity/libs/blob/master/proposals/20220203-versioning-schema-amendment.md
- [LucaGuerra] Security content for Falco 0.31.1 and future improvements
    - https://github.com/falcosecurity/falco/security/advisories/GHSA-6v9j-2vm2-ghf7
    - https://github.com/falcosecurity/libs/issues/252
- [terylt,araujof,LucaGuerra,zuc] Falco 0.31.1 ubi image and build
    - https://github.com/sysflow-telemetry/falco/tree/falco_ubi_image/docker
    - https://github.com/sysflow-telemetry/falco/pkgs/container/falco
    - https://github.com/sysflow-telemetry/falco/actions


### Closing

- **MC Next Call**: 

## 2022-03-09

### MC

- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))

### Who joined

- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Fred Araujo ([araujof](https://github.com/araujof))
- Andrea Bonanno ([andreabonanno](https://github.com/andreabonanno))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Leonardo Grasso ([leogr](https://github.com/leogr))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Michele Zuccala ([@zuc](https://github.com/zuc))


### This week highlights


### Agenda (Please add any items you would like to discuss here)

- [LucaGuerra] Falco Patch Release 0.31.1 Update
    - https://github.com/falcosecurity/falco/issues/1924
- [zuc] Possible switch to test-infra from CircleCI to GitHub Actions and/or Prow
    - [leogr] +1
    - [deepskyblue86] +1 (slight preference towards gh-actions)
- [LucaGuerra, araujof, terylt, Molter73] UBI image and RedHat Catalog
    - It would be great to be able to contribute an UBI-based image to the RedHat catalog to:
        - Make it easier for RedHat shops to deploy Falco
        - Have an image that is constantly updated with the latest security fixes even if the Falco version doesn't change
        - Ideally, build it with a separate pipeline that can detect newer versions/security fixes to base UBIs and publish snapshots automatically
    - Mauro Moltrasio will try to understand if he can get more information for us to do this


### Closing

- **MC Next Call**: 


# Falco Community Call

[More Information](https://github.com/falcosecurity/community)
[Zoom Link](https://zoom.us/my/cncffalcoproject)
[Recording](https://youtube.com/playlist?list=PLgVVUpW8NIJAaZtszf1_nxB2y6mQrlY4s)

## 2022-03-02

### MC

- Federico Di Pierro ([fededp](https://github.com/fededp))

### Who joined

- Michele Zuccala ([@zuc](https://github.com/zuc))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Giles Hutton ([@Stringy](https://github.com/Stringy))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Fred Araujo ([araujof](https://github.com/araujof))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Pablo Lopez Zaldivar ([@pabloopez](https://github.com/pabloopez))
- Adao Junior ([junior](https://github.com/junior))
- Andrea Bonanno ([andreabonanno](https://github.com/andreabonanno))

### This week highlights

- Last calls records are now accessible through community page of falco.org https://falco.org/community/

### Agenda (Please add any items you would like to discuss here)

- Thomas asks to become maintainer of falco-website
    - Everyone agrees
- Performance measurement & comparison of kernel probes 
    - https://sysdig.com/blog/sysdig-and-falco-now-powered-by-ebpf/
    - https://github.com/falcosecurity/libs/pull/115 (analysis by @FedeDP)
- Falco patch release 0.31.1
    - https://github.com/falcosecurity/libs/pull/235
    - @LucaGuerra will lead the process, backed by existing Falco maintainers
    - https://github.com/falcosecurity/falco/pulls?q=is%3Apr+is%3Amerged+closed%3A%3E2022-01-31 <- additions since the last release
- Contributor of the month nominations
 
### Closing

- **MC Next Call**: Luca Guerra

## 2022-02-23

### MC

- Pablo Lopez Zaldivar ([@pabloopez](https://github.com/pabloopez))

### Who joined

- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Pablo Lopez Zaldivar ([@pabloopez](https://github.com/pabloopez))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Fred Araujo ([araujof](https://github.com/araujof))
- Andrea Bonanno ([andreabonanno] (https://github.com/andreabonanno))
- Alban Crequy ([@alban](https://github.com/alban))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- POP

### This week highlights

- 
### Agenda (Please add any items you would like to discuss here)

- Do Falco support for AWS EKS Fargate? Any suggested deployment strategies in production environment???
    - Leo suggest user-space instrumentation- 
    - https://github.com/falcosecurity/pdig
    - https://github.com/falcosecurity/kilt

- Falco training update PR
    - Leo approval after link updated

- Falco plugin for Seccomp Agent (seccomp-notify)
    - https://github.com/falcosecurity/plugins/pull/73
    - Approved!

- Plugins from external contributions (Thomas)
    - Architecture to include not just the source code, but docs and examples
    - Leo adds: 
        - plugins included in `falcosecurity/plugins` are packed directly with Falco
        - Plans to refactor k8s audit logs source as a plugin (this was discussed previously)
        - In general terms, it is required to define a better workflow to include, test & build new plugins
        - plus how to make them more usable. Leo is suggesting Helm Charts (+ Andrew Bonanno)
        - equivalent approach to distribute rules specific for each plugin
        - Template repository for new people to build their plugins
        - falcoctl effort associated with this workflow?
        - Thomas prefers a K8s operator approach more than the cli tool. Leo believe boths are required, for host installs
    - Artifact Hub - compatible? - ping
 
### Closing

- **MC Next Call**: Federico Di Pierro

## 2022-02-16

### MC

- Zsolt NEMETH ([@zsmav](https://github.com/zsmav))

### Who joined

- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Adao Junior ([junior](https://github.com/junior))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Mauro Moltrasio ([@Molter73](https://github.com/Molter73))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Fred Araujo ([araujof](https://github.com/araujof))
- Andrea Bonanno ([andreabonanno] (https://github.com/andreabonanno))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))
- POP

### This week highlights

- [Issif] First blog post about how to write a plugin: https://falco.org/blog/extend-falco-inputs-with-a-plugin-the-basics/

### Agenda (Please add any items you would like to discuss here)

- Issif: docs for plugins, where? how? (something along these lines? https://www.nginx.com/resources/wiki/modules/)
- Mauro: Quick intro and discussing upstreaming of some changes from RedHat.
- youtube streaming of meetings ([link](https://www.youtube.com/playlist?list=PLgVVUpW8NIJAaZtszf1_nxB2y6mQrlY4s))
- maybe put the youtube channel up here: https://falco.org/community/

### Closing

- **MC Next Call**: Pablo

## 2022-02-09

### MC

- Thomas Labarussias ([@Issif](https://github.com/Issif))

### Who joined

- Federico Di Pierro ([fededp](https://github.com/fededp))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Fred Araujo ([araujof](https://github.com/araujof))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Matt Moyer ([mattmoyer](https://github.com/mattmoyer))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))
- POP
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Fernando Nogueira ([fjsnogueira](https://github.com/fjsnogueira))
- Adao Junior ([junior](https://github.com/junior))

### This week highlights

- Helm chart for Falco 0.31 is out (without plugin management for now)

### Agenda (Please add any items you would like to discuss here)

- ([alban](https://github.com/alban)) Idea: Seccomp Notify & Seccomp Agent as a data source for Falco?
   - Using Seccomp Notify & Seccomp Agent to freeze a container on a bad syscall
   - Gather data for forensics: processes stack, rootfs tarball, etc.
   - https://github.com/kinvolk/seccompagent/pull/18
   - https://github.com/kinvolk/seccompagent/pull/20
   - Does it make sense, is it useful? Or does it belong to another project?
     - [leogr] suggestion for the PoC: Try to write a plugin!
- Conventions are upcoming, please, feel free to submit talks about Falco

### Closing

- **MC Next Call**: To be determined 

## 2022-02-02

### MC

- Leonardo Grasso ([leogr](https://github.com/leogr))

### Who joined

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Zsolt NEMETH ([@zsmav](https://github.com/zsmav))
- POP
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Adao Junior ([junior](https://github.com/junior))
- Tim Graves ([atimgraves](https://github.com/atimgraves))
- Gilson Melo ([gilsonmelo](https://github.com/gilsonmelo))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))
- Fred Araujo ([araujof](https://github.com/araujof))


### This week highlights

- Falco 0.31.0 (a.k.a. "Gyrfalcon") is out! 
    - Check out the [blog post](https://falco.org/blog/falco-0-31-0/)!
    - Helm chart updated
    - falco-exporter updated

### Agenda (Please add any items you would like to discuss here)

- Please share your experience with plugins!

### Closing

- **MC Next Call**: Thomas or Leogr as backup

## 2022-01-26

### MC

- Federico Di Pierro ([fededp](https://github.com/fededp))

### Who joined

- Leonardo Grasso ([leogr](https://github.com/leogr))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- POP
- Sreeda U M ([sreedaum] (https://github.com/sreedaum)
- Fred Araujo ([araujof](https://github.com/araujof))

### This week highlights

### Agenda (Please add any items you would like to discuss here)

- [pabloopez] Falco Training [updates](https://kubernetes.slack.com/archives/CMWH3EH32/p1643207852219800)
- [jasondellaluce] Falco 0.31.0 release agenda: https://github.com/falcosecurity/falco/issues/1857

### Closing

- **MC Next Call**: Leonardo Grasso ([leogr](https://github.com/leogr))

## 2022-01-19

### MC

- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))

### Who joined

- Leonardo Grasso ([leogr](https://github.com/leogr))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Thomas Labarussias ([Issif](https://github.com/Issif))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))
- Fred Araujo ([araujof](https://github.com/araujof))
- Federico Di Pierro ([fededp](https://github.com/fededp))

### This week highlights

- Upcoming release highlights:
    - Brand new plugin system! :)
    - Improved stability and support of eBPF probe
    - New system calls
        - openat2
        - mprotect
        - execveat
        - is_exe_writable flag
    - Simple consumer optimisation
    - Support to blocks large up to 4GB
        - Better support and improved security
    - Lua scripts are embedded in Falco
    - Many rule updates
        - Security improvements
    - Buf fixes and improvements on http output and json formatting
    - Dependencies have been updated (CivetWeb, OpenSSL)
    - Improvements in CMake building system
        - No patches anymore :)
    - Bug fixes and stability improvements in rule engine (rule disabling, json pointer)
    - Compilation improvements in libs for some platforms

- Golang SDK for plugin v0.1.0 is out
    - https://github.com/falcosecurity/plugin-sdk-go

- Plugin registry is (almost) complete!
    - https://github.com/falcosecurity/plugins

- Stable plugin builds for Linux x64
    - https://download.falco.org/?prefix=plugins/stable/

### Agenda

- [jasondellaluce] Falco 0.31.0 release agenda: https://github.com/falcosecurity/falco/issues/1857
- [Thomas] Some update about test-infra and driverkit
    - The latest version of driverkit is not yet running on test-infra, but it will be fixed soon
- [Thomas] Falco Talon https://github.com/Issif/falco-talon

### Closing

- **MC Next Call**: Federico Di Pierro

## 2022-01-12

### MC

- Thomas Labarussias ([Issif](https://github.com/Issif))

### Who joined

- Jason Dellaluce ([jasondellaluce](https://github.com/jasondellaluce))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Leonardo Grasso ([leogr](https://github.com/leogr))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Fred Araujo ([araujof](https://github.com/araujof))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Zsolt Nemeth ([zsmav](https://github.com/zsmav))

### This week highlights

- Huge release at the end of the month. Jason will be release manager (Teryl and Thomas will shadow).
    - What's coming will be shared next coming
    - No blocker

### Agenda

- Driverkit:
    - current situation
    - volunteers for maintainers?
        - Issif (Thomas) proposes himself as new Maintainer: everybody agrees
        - Luca will help with Driverkit
- Libs:
    - Federico proposed as Maintainer: everybody agrees

- Contributor of the Month Nominations

### Closing

- **MC Next Call**: Issif (Thomas)

## 2022-01-05

### MC

- Thomas Labarussias ([Issif](https://github.com/Issif))

### Who joined

- Jason Dellaluce ([jasondellaluce](https://github.com/jasondellaluce))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))
- POP
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Fred Araujo ([araujof](https://github.com/araujof))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Teryl Taylor ([terylt](https://github.com/terylt))

### This week highlights

- Issif (Thomas) is now OSS/Ecosystem Advocate at Sysdig

### Agenda

- falco-driver-check (Issif) https://github.com/Issif/falco-driver-check
    - please test it for checking if there's no false positive or revert
- falco release reminder (jasondellaluce)
    - Jason proposes itself as release manager
    - Teryl will shadow
    - Thomas will shadow

### Closing

- **MC Next Call**: Issif (Thomas)

## 2021-12-08

### MC

- Fred Araujo ([araujof](https://github.com/araujof))

### Who joined

- Thomas Labarussias ([Issif](https://github.com/Issif))
- Fred Araujo ([araujof](https://github.com/araujof))
- POP
- Zsolt Nemeth ([zsmav](https://github.com/zsmav))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))
- Carlos Panato ([cpanato](https://github.com/cpanato))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))

### This week highlights
Link to Goreleaser(https://goreleaser.com/)

### Agenda

- Falco Talon, aka how to claw with class
- Surprise from Thomas
- Sign falcosidekick with [cosign](https://github.com/sigstore/cosign/)? - as starting point (Carlos Panato)
- Branch rename from master to main (Carlos Panato)
  https://inclusivenaming.org/
- Falcosidekick with more Linux platforms available (Carlos Panato)
  https://github.com/falcosecurity/falcosidekick/pull/288
- Vote to make this meeting the last of the year (holidays),  Reconvene in Jaunary
  - VOTE WAS YES UNANIMOUS
- Contributor of the Month Award! ???

### Closing

- **MC Next Call**: 

## 2021-12-01

### MC

- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))

### Who joined

- Teryl Taylor ([terylt](https://github.com/terylt))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Thomas Labarussias ([Issif](https://github.com/Issif))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Akos Kaldy ([kaldyka](https://github.com/kaldyka))


### This week highlights


### Agenda

- [Teryl] Falco base Images
    - Adding an image to make it easier for people to build the libs (example code from Teryl: https://github.com/terylt/libs/commit/fc437483e694c7b9b2f794daba2a92c3b995c05c)
    - Adding an UBI based image as an alternative Falco image
    - [LucaG] I think they're both great ideas, personally I would suggest starting from the UBI image because it's easier to propose (adding to docker/) and would help some people with compatibility (RH ecosystem), potential certification and security scanning requirements
- [Andrea] Add support to execveat syscall(https://github.com/falcosecurity/libs/pull/141)

### Closing

- **MC Next Call**: 


## 2021-11-17

### MC

- POP

### Who joined
- Zsolt Nemeth ([zsmav](https://github.com/zsmav))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Leonardo Grasso ([leogr](https://github.com/leogr))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- POP
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Jason Dellaluce ([jasondellaluce](https://github.com/jasondellaluce))
- Akos Kaldy ([kaldyka](https://github.com/kaldyka))

### This week highlights


### Agenda
- Team R6 contribution to Falco - using automated triggers for moving target defense ()    (link provided for contributing: https://github.com/falcosecurity/.github/blob/master/CONTRIBUTING.md)
- Contributor of the Month Nomination!  (POP)
- Add support to clone3 syscall (https://github.com/falcosecurity/libs/pull/129)
- Vote to Cancel next week's meeting due to US holiday?  (Majority Vote to Cancel next weeks meeting)

### Closing

- **MC Next Call**: 


## 2021-11-10

### MC

- POP

### Who joined
- Jason Dellaluce ([jasondellaluce](https://github.com/jasondellaluce))
- POP
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Leonardo Grasso ([leogr](https://github.com/leogr))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))


### This week highlights


### Agenda
- Dev Build for Plugins - https://app.circleci.com/pipelines/github/falcosecurity/falco/1795/workflows/06438037-2b18-4b13-9da2-1312a9d7fba3/jobs/15815/artifacts


### Closing

- **MC Next Call**: 


## 2021-11-03

### MC

- Jason Dellaluce ([jasondellaluce](https://github.com/jasondellaluce))

### Who joined

- Leonardo Grasso ([leogr](https://github.com/leogr))
- Marky Jackson ([markyjackson-taulia](https://github.com/markyjackson-taulia)
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- John Brydon ([jbrydon-scwx](https://github.com/jbrydon-scwx))
- Teryl Taylor ([terylt](https://github.com/terylt))
- David Windsor ([dwindsor](https://github.com/dwindsor))

### This week highlights


### Agenda
- [dwindsor] CentOS 8 kernel drivers on S3 (update)
    - SELinux prevents falco-driver-loader from executing insmod on CentOS 8 (MERGED 🙏)
    - Since CentOS <= 8.3 have been moved to Vault, need to update driverkit centos builder (still need)
        - Issue: https://github.com/falcosecurity/driverkit/issues/105
        - PR: https://github.com/falcosecurity/driverkit/pull/104
- [plugins] newest updates on the plugin system
    - Current state of plugin system development
        - https://github.com/falcosecurity/libs/pull/93
        - https://github.com/falcosecurity/libs/pull/107
    - [jasondellaluce] `plugin-sdk-go` refactoring, little demo with `dummy` plugin
        - https://github.com/falcosecurity/plugin-sdk-go/pull/18
        - https://github.com/falcosecurity/plugins/pull/28
    - Adding @jasondellaluce to `plugin-sdk-go` OWNERS
    - Master TODO list: https://github.com/falcosecurity/evolution/issues/103
- [markyjackson-taulia] Owners file
    - Discuss the governance process

### Closing

- **MC Next Call**: 


# Falco Community Call

[More Information](https://github.com/falcosecurity/community)
[Zoom Link](https://zoom.us/my/cncffalcoproject)
[Recording](https://)

## 2021-10-27

### MC

- Teryl Taylor ([terylt](https://github.com/terylt))

### Who joined 

- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Jason Dellaluce ([jasondellaluce](https://github.com/jasondellaluce))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- David Windsor ([dwindsor](https://github.com/dwindsor))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Andrew Pollack ([@andrewpollack](https://github.com/andrewpollack))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Maide UYGUR ([@maideuygur](https://github.com/maideuygur))
- Daniele Di Vito ([@danieledivito](https://github.com/danieledivito))
- 

### This week highlights

- [dwindsor] CentOS 8 kernel drivers
  - PR (merged): https://github.com/falcosecurity/test-infra/pull/528 (CentOS 8.4 drivers)
  - Since CentOS <= 8.3 have been moved to Vault, need to update driverkit centos builder
    - Issue: https://github.com/falcosecurity/driverkit/issues/105
    - PR: https://github.com/falcosecurity/driverkit/pull/104
  - SELinux prevents falco-driver-loader from executing insmod on CentOS 8
    - Issue: https://github.com/falcosecurity/falco/issues/1755
    - PR: https://github.com/falcosecurity/falco/pull/1756
- [dwindsor] Digests for kernel drivers, eBPF probes hosted on download.falco.org?
- [dwindsor] Possibly add gpg signing for kernel drivers/eBPF probes to driverkit driverbuilders?

### Agenda
- [dwindsor] CentOS 8 kernel drivers on S3

### Closing

- **MC Next Call**: 

## 2021-10-20

### MC

- POP

### Who joined 

- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Michele Zuccala ([zuc](https://github.com/zuc))
- Thomas Labarussias ([Issif](https://github.com/Issif))
- Fred Araujo ([araujof](https://github.com/araujof))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Jason Dellaluce ([jasondellaluce](https://github.com/jasondellaluce))
- Lorenzo Susini ([loresuso](https://github.com/loresuso))
- Federico Di Pierro ([fededp](https://github.com/fededp)) 
- Andrea Ceresoni ([cere](https://gihub.com/berez23))
- Sujogya Kumar Sahu([Sujogya123](http://github.com/Sujogya123))
- Sujit Kumar Sahu([sujit kumar sahu](http://github.com/sujit-kumar-sahu))

### This week highlights
- Kubecon Recap


### Agenda
- [Luca] proc.is_exe_writable proposal
    - PR: https://github.com/falcosecurity/libs/pull/97
    - Rationale and demo
- [zuc] CI/CD pipeline to publish Falco plugins dev builds on S3

### Closing

- **MC Next Call**: 


## 2021-10-06

### MC

- POP

### Who joined 

- Leonardo Grasso ([leogr](https://github.com/leogr))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Pablo Lopez Zaldivar ([pabloopez](https://github.com/pabloopez))
- Jason Dellaluce ([jasondellaluce](https://github.com/jasondellaluce))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Fred Araujo ([araujof](https://github.com/araujof))
- Vicente Herrera ([vicenteherrera](https://github.com/vicenteherrera))
- John Brydon ([jbrydon-scwx](https://github.com/jbrydon-scwx))

### This week highlights

- Falco 0.30.0 is out!
    - [Blog post](https://falco.org/blog/falco-0-30-0/)
    - [Changelog](https://github.com/falcosecurity/falco/blob/master/CHANGELOG.md#v0300)
- [client-go](https://github.com/falcosecurity/client-go/releases/tag/v0.4.0) and [client-py](https://github.com/falcosecurity/client-py/releases) have been updated
- [falco-exporter v0.6.0](https://github.com/falcosecurity/falco-exporter/releases/tag/v0.6.0) has been released
- Helm charts update
    - `falco` chart updated ([changelog](https://github.com/falcosecurity/charts/blob/master/falco/CHANGELOG.md#v1160))
    - `falco-export` chart ([PR waiting for review](https://github.com/falcosecurity/charts/pull/279))


### Agenda

- [Pablo] Falco Labs ([Link](https://falco.org/labs/))
    - revamp existing materials
    - ways to contribute: open an issue with course requests or send PRs here: [source code](https://github.com/falcosecurity/katacoda-scenarios)
- canceling next week community call (because of KubeCon)

### Closing

- **MC Next Call**: 

