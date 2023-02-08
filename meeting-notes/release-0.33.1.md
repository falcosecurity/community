## 2023-02-01

### MC

- Jacqueline Salinas [jsalinas32](https://github.com/jsalinas32)

### Who joined

- Thomas Labarussias [Issif](https://github.com/Issif)
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Fred Araujo ([araujof](https://github.com/araujof))
- Leonardo Grasso ([leogr](https://github.com/leogr))
- Federico Di Pierro ([@fededp](https://github.com/FedeDP))
- Samuele Cappellin ([@cappellinsamuele](https://github.com/cappellinsamuele))
- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- Vicente JJ. Miras ([vjjmiras](https://github.com/vjjmiras))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Jacqueline Salinas [jsalinas32](https://github.com/jsalinas32)
- Melissa Kilby ([@incertum](https://github.com/incertum))
- Angelo Puglisi [@deepskyblue86](https://github.com/deepskyblue86)
- Stanley Chan [@happy-dude](https://github.com/happy-dude)

### Weekly highlights

### Agenda

- [LucaG] Falco 0.34.0 Release Update
- [Melissa] proposing as libs maintainer (YAY!!!)
- [Federico] BPF issue with clang15: https://github.com/falcosecurity/libs/pull/858


## 2023-01-25

### MC

- Mauro Moltrasio ([Molter73](https://github.com/Molter73))

### Who joined

- Jacqueline [jsalinas32](https://github.com/jsalinas32)
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Adao Oliveira Junior ([junior](https://github.com/junior))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- Samuele Cappellin ([@cappellinsamuele](https://github.com/cappellinsamuele))
- Thomas Labarussias [Issif](https://github.com/Issif)
- Stanley Chan ([@happy-dude](https://github.com/happy-dude))
- Vicente JJ. Miras ([vjjmiras](https://github.com/vjjmiras))
- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Fred Araujo ([araujof](https://github.com/araujof))
- Federico Di Pierro ([@fededp](https://github.com/FedeDP))


### Weekly highlights


### Agenda
- [vjjmiras] proposing as an approver for the falco-website repository
- [vjjmiras] upcoming falco tutorials:: i.e. https://killercoda.com/pmusa/scenario/installing-falco-ubuntu
- [jsalinas32] proposing as website reviewer
- [jsalinas32] planning for kubecon eu - falco representation 
    - Need volunteers that are attending kubecon
    - [LucaGuerra] proposes some kind of interactive activity such as a CTF, installing falco, etc...
    - [vjjmiras] since it is 4 hours, maybe split by level of familiarity with Falco.
- [jsalinas32] 0.34.00 activities & promotion
    - https://github.com/falcosecurity/falco/issues/2368
    - CNCF project benefits: on-demand webinar March 23rd
    - CNCF project benefits: youtube playlist submission Mar 3rd
    - Blog/release n
- [jsalinas32] [community survey](https://docs.google.com/document/d/1-rp4yLebf6k1oEjSHmamQdmsP7kOUA2iLbyx3MrRiX0/edit?usp=sharing)
- [jason/leo] how do you deploy Falco in production? https://github.com/falcosecurity/falco/issues/2376
- [jacque] submit your [FAQ]( https://docs.google.com/forms/d/e/1FAIpQLSc2UWOjCNW7v1dryvzwNc7pQTbzfP84wY9aF7Gx1_YgJMjqtQ/viewform)

- [jsalinas32] volunteers as MC next week :D

---

## 2023-01-18

### MC

- Leonardo Grasso ([@leogr](https://github.com/leogr))

### Who joined

- Federico Di Pierro ([@fededp](https://github.com/FedeDP))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Samuele Cappellin ([@cappellinsamuele](https://github.com/cappellinsamuele))
- Fred Araujo ([araujof](https://github.com/araujof))
- Thomas Labarussias [Issif](https://github.com/Issif)
- Vicente JJ. Miras ([vjjmiras](https://github.com/vjjmiras))
- Adao Oliveira Junior ([junior](https://github.com/junior))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Sumit Bindal ([sumitb](https://github.com/sumitb))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Haydn Johnson ([@haydz](https://github.com/haydz))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))


### Weekly highlights


### Agenda

* [leogr] Upcoming Falco release (by Jan)
    - Retrieve and automatically update artifacts (e.g., plugins)
    - CORE eBPF driver
    - Luca is the Release Manager
* [luca]
    - to open a tracking issue for the relase
    - before we start the usual release actions we need to make sure our CI/CD pipeline is secure
        - circleci had a data breach which might have impacted us
        - all internal secrets/keys have been refreshed
        - no evidence was found that suggests that unauthorized access happened anywhere in our CI/CD infrastructure but we need to be safe
        - we're ensuring everything is ok on our side before proceeding
    - GPG key to sign packages will change
* [jason] working on rotating GPG key
    - providing a new key
    - re-signing old packages

- [leogr] test-infra long term
    - We are going to abdon circleci in favor of GHA
    - On-going efforts to port jobs and renovate our infra

- [Thomas/luca] First meeting Supply Chain WP tomorrow 
    - https://lists.cncf.io/g/cncf-falco-dev/viewevent?repeatid=49479&eventid=1795103&calstart=2023-01-19
    - https://hackmd.io/FwSPVkdHT0i8T4Q8JdfOaw
>When:
Thursday, January 19th, 2023
6:00pm to 7:00pm
(UTC+01:00) Central European Time - Rome
Repeats: Every Thursday
Organizer: Luca Guerra
Description: Supply Chain Security Working Group
>
>Slack channel: https://cloud-native.slack.com/messages/falco-sscs-wg
HackMD: https://hackmd.io/FwSPVkdHT0i8T4Q8JdfOaw
Join the call: https://zoom.us/my/cncffalcoproject

- [Mauro] voloutered to MC next week! yay!

---

## 2023-01-11

### MC

* Thomas Labarussias [Issif](https://github.com/Issif)

### Weekly highlights

### Who joined
* Jacqueline [jsalinas32](https://github.com/jsalinas32)
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Vicente JJ. Miras ([vjjmiras](https://github.com/vjjmiras))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Adao Oliveira Junior ([junior](https://github.com/junior))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Angelo Puglisi [@deepskyblue86](https://github.com/deepskyblue86)
- Federico Di Pierro ([@fededp](https://github.com/FedeDP))
- Aizhamal Nurmamat kyzy ([aijamalnk](https://github.com/aijamalnk))

### Agenda
* [Aizhamal] [Falco.org revamp proposal](https://docs.google.com/document/d/1hknrzUv_dOlptK1q59aCe9DnWzwyQWCEsDI2ilehZGs/edit#) 
* [Issif] Falcosidekick 2.27.0 and Falcosidekick-UI 2.1.0 are out !! https://falco.org/blog/falcosidekick-2-27-0-ui-2-1-0
* [jasondellaluce] proposing myself as a falcosecurity/libs maintainer
* [LucaG] Falco 0.34.0 release
    * libs 0.10.0
    * massive new features:
        * New eBPF probe! CO-RE support and more
        * Including Falcoctl to automatically update the rules without needing to upgrade the entire Falco
    * [LucaG] proposing myself as release manager for this version
    * [AndreaTerzolo] volunteering as release shadow
* Next week 1st meeting of WG for Supply Chain Security
    * Jacque is to add the event to the community calendar
    * Jacque is to find out how to give permission to other community members to the calendar and document the process
    * Time and date: Thursdays (starting January 19th 2023) at 6PM Central Europe

## HOLIDAY BREAK!

The next Falco call will be on January 11th 2023! 🎄


## 2022-12-14

### MC

- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))

### Who joined
* Jacqueline Salinas (https://github.com/jsalinas32)
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Adao Oliveira Junior ([junior](https://github.com/junior))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Angelo Puglisi [@deepskyblue86](https://github.com/deepskyblue86)
- Stanley Chan ([@happy-dude](https://github.com/happy-dude))
- Vicente JJ. Miras ([vjjmiras](https://github.com/vjjmiras))
- Jason Dellaluce ([@fededp](https://github.com/jasondellaluce))
- Federico Di Pierro ([@fededp](https://github.com/FedeDP))
- Samuele Cappellin ([@cappellinsamuele](https://github.com/cappellinsamuele))
- Thomas Labarussias [Issif](https://github.com/Issif)
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))

### This weeks highlights 
* 

### Agenda
* [Edvin] https://github.com/falcosecurity/falco-exporter/issues/81 help needed.
    * The issue seems to persist with the latest version of the helm chart
* [LucaG] Falco Supply Chain Security WG
    * Join us on #falco-scss-wg on the CNCF Slack
    * https://hackmd.io/FwSPVkdHT0i8T4Q8JdfOaw
* [jacque] linkedin page & group https://www.linkedin.com/company/91577955/admin/
* [jacque] housekeeping items: https://docs.google.com/document/d/1mDCIsBLzty4RILTHt_r1nLADiGo656cxbAQNsbjLPks/edit?usp=sharing 
* [Andreagit97] Propose c++17 as default standard for falcosecurity libraries
    * [Molter73] The compiler we're using is the one shipped with UBI8 (possibly gcc-8)
    * [leogr] Big +1!
    * [Angelo] gcc support: https://gcc.gnu.org/projects/cxx-status.html#cxx17
- [leogr] Artifacts distribution proposal
  - https://github.com/falcosecurity/falco/pull/2304
  - Can we proceed?
  - I'd like to start with moving rules out from the Falco repo and make falcoctl official by Falco 0.34
  - [LucaG] +1
* [Stanley] general question on if there has been any testing with Falco on Linux kernel ≥ 6.1 ?
    * 6.1 is the next LTS kernel so it's specifically interesting
* [Stanley] is there a testing criteria/validation for modern BPF probe? I see that we can currently build it if we are following HEAD
    * [Andreagit97] The plan is to make this available but experimental in falco 0.34, completing syscall support for 0.35
* [Angelo] It would be great to run e2e test on the modern ebpf probe as well
    * [Molter73] Looking into it, requires some update to the base image

Last Falco Call of the year 2022! See you on January 11th 2023! 🎄


## 2022-12-07

### MC

- Thomas Labarussias [Issif](https://github.com/Issif)

### Who joined

- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- David Windsor ([dub](https://github.com/dwindsor))
- Fred Araujo ([araujof](https://github.com/araujof))
- Adao Oliveira Junior ([junior](https://github.com/junior))
- Stanley Chan ([happy-dude](https://github.com/happy-dude))

### This week highlights

- 

### Agenda

- Cancelled because of lack of items (+ Italian holidays)

## 2022-11-30

### MC

- Federico Di Pierro ([@fededp](https://github.com/FedeDP))

### Who joined

- Federico Di Pierro ([@fededp](https://github.com/FedeDP))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Jason Dellaluce ([@fededp](https://github.com/jasondellaluce))
- Angelo Puglisi [@deepskyblue86](https://github.com/deepskyblue86)
- Vicente JJ. Miras ([vjjmiras](https://github.com/vjjmiras))
- Lorenzo Susini ([@loresuso](https://github.com/loresuso))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Samuele Cappellin ([cappellinsamuele](https://github.com/cappellinsamuele))
- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Ali Adnan ([adduali1310])(https://github.com/adduali1310))
- Adao Oliveira Junior ([junior](https://github.com/junior))
- Massimiliano Giovagnoli ([@maxgio92](https://github.com/maxgio92))
- Thomas Labarussias [Issif](https://github.com/Issif)
- Leonardo Grasso [leogr](https://github.com/leogr)


### This week highlights

- [LucaGuerra] Patch release for Falco: 0.33.1

### Agenda

- [fededp] Nearing next libs+driver tag
- [Issif] AWS Security Lake: Falco is one the first OSS source:
    - [docs](https://docs.aws.amazon.com/security-lake/latest/userguide/integrations-third-party.html) 
    - [PR](https://github.com/falcosecurity/falcosidekick/pull/387)
    - [blog post](https://falco.org/blog/falco-on-aws/)
- [Issif] Falcosidekick 2.27.0 is upcoming next week (I hope)
- [LucaGuerra, maxgio92] Proposing a Falco supply chain security WG
    - Consistent artifact+release signing
    - Artifact signature verification with falcoctl
    - SBOMs for Falco
    - Improving the Falco official container image to play nicer with SCA tools and vulnerability scanners
- [Issif] (following up from above) Towards a more consistent CI/CD for Falcosecurity projects, especially ones written in Go
    - example of Falcosidekick: [goreleaser](https://github.com/falcosecurity/falcosidekick/blob/361e42324bf17504ac2bb19faf2a3f3965e3dfb6/.goreleaser.yml#L128)
- [vjjmiras] Updates to Falco docs
- [leogr] still WIP - Artifact distribution proposal
    - https://github.com/falcosecurity/falco/pull/2304
    - early feedback is appreciated
- [leogr] graduation updates
    - we are still looking for adopters
    - duo-diligence doc to be shared asap

