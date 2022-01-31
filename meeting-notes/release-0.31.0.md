# Falco Community Call

[More Information](https://github.com/falcosecurity/community)
[Zoom Link](https://zoom.us/my/cncffalcoproject)
[Recording](https://)

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

