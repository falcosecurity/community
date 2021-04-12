
# Falco Community Call

[More Information](https://github.com/falcosecurity/community)
[Zoom Link](https://zoom.us/my/cncffalcoproject)
[Recording](https://)

## 2021-04-07

### MC

Lorenzo Fontana ([@fntlnz](https://github.com/fntlnz))

### Who joined

- Lorenzo Fontana ([@fntlnz](https://github.com/fntlnz))
- POP ([@danpopsd](https://github.com/danpopsd))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Loris Degioanni ([@ldegio](https://github.com/ldegio))
- Leonardo Di Donato ([@leodido](https://github.com/leodido))


### This week highlights


### Agenda

- [fntlnz] Revert exceptions in default ruleset https://github.com/falcosecurity/falco/pull/1602
- [leodido] Updates on release
- [David Windsor (dub)] Documentation examples for libsinsp
- [Loris Degioanni] scap files minor version number
  - https://gitlab.com/wireshark/wireshark/-/merge_requests/2631#note_545332971

---

## 2021-03-31

### MC

- POP ([@danpopsd](https://github.com/danpopsd))


### Who joined

- Leonardo Grasso ([@leogr](https://github.com/leogr))
- POP ([@danpopsd](https://github.com/danpopsd))
- Jonah Jones ([@jonahjon](https://github.com/jonahjon))
- Robby Cochran ([@robbycochran](https://github.com/robbycochran))
- Loris Degioanni ([@ldegio](https://github.com/ldegio))
- Lorenzo Fontana ([@fntlnz](https://github.com/fntlnz))
- Paul Morie ([@pmorie](https://github.com/pmorie))
- Magno Logan ([@magnologan](https://github.com/magnologan))


### This week highlights

- [leogr] Migration from Bintray to download.falco.org completed!
  - Please do not use https://dl.bintray.com/falcosecurity/ anymore
  - You can now find packages at https://download.falco.org/?prefix=packages/
  - Upgrade paths https://falco.org/docs/getting-started/upgrade/
  - Special thanks to [leodido] and [fntlnz] for reviewing and helping

### Agenda

- [@robbycochran] RedHat+StackRox intros and contributions to falcosecurity/libs
- [pop] Falco Survey -- Brief Update. (Make sure to share if you all can as well) https://twitter.com/falco_org/status/1376525535413698560?s=20
- [pop] Contributor of the Month Nominations are open until April 12th.
- [leogr] Bulk archiving of abandoned projects [evolution#51](https://github.com/falcosecurity/evolution/issues/51)
  - +1 [fntlnz]
  - +1 [pop]
- [fntlnz] bpf harness needs love + being moved to falco
- [@jonahjon] Jonah Jones - monitoring of incomplete jobs and the implications to slack.  (options discussed)
  - #falco-alerts channel will be created on sysdig opensource channel for prow alerts (Lorenzo and Jonah to work on this)

---

## 2021-03-24

### MC

- POP ([@danpopsd](https://github.com/danpopsd))


### Who joined

- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Barak Stout ([@barakstout](https://github.com/barakstout))
- Stefan Uygur ([@ostendali](https://github.com/ostendali))
- Yusuf ([@Yufi_99](https://github.com/Edge2Ops))
- Leonardo Di Donato ([@leodido](https://github.com/leodido))

### This week highlights

- [pop] Discussion on Falco Spring survey
- [thomas] Frank's elevation to maintainer
  - [leodido] +1
  - [pop] +1
- [leodido] Support for the newer kernels (> 5.4) on Amazon Linux 2
  - Will ship a bunch of them next week
- [leodido] Radhika working on creating a step-by-step guide for translating the Falco website

### Agenda

- Falco Spring 2021 Community Survey -- POP
- Accept Frank as maintainer for Falcosidekick
- Thomas presents a talk about Falco tomorrow for CNCF Paris (in French)

---

## 2021-03-17

### MC

- Leonardo Grasso ([@leogr](https://github.com/leogr))

### Who joined

- Frank Jogeleit ([@fjogeleit](https://github.com/fjogeleit))
- Leonardo Di Donato ([@leodido](https://github.com/leodido))
- Jonah Jones ([@jonahjon](https://github.com/jonahjon))
- Barak Stout ([@barakstout](https://github.com/barakstout))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Lorenzo Fontana ([@fntlnz](https://github.com/fntlnz))
- Thomas Labarussias ([@Issif](https://github.com/Issif))

### This week highlights

### Agenda

- [leogr] Update about packages migration from Bintray to download.falco.org
  - New publishing job almost ready PR [#1577](https://github.com/falcosecurity/falco/pull/1577) (testing in progress)
  - Documentation PR [falco-website#405](https://github.com/falcosecurity/falco-website/pull/405)
  - All other details in the issue [#1567](https://github.com/falcosecurity/falco/issues/1567)
- [leodido] Proposal to postpone Falco 0.28.0
  - [fntlnz] +1 binding
  - [grasso] +1 binding
  - Community agrees, nothing against
  - Targeting end of March
- [fjogeleit] preview new Falcosidekick UI
  - [leodido] +100 for material! :heart_decoration:
- [fntlnz] BPF probe updates
  - [leodido] +1 binding
  - Open incubating issue in evolution
- Release process
  - [fntlnz] Choose a release team immediatelly after a release

---

## 2021-03-10

### MC

- POP ([@danpopsd](https://github.com/danpopsd))

### Who joined

- Leonardo Grasso ([@leogr](https://github.com/leogr))
- POP ([@danpopsd](https://github.com/danpopsd))
- Frank Jogeleit ([@fjogeleit](https://github.com/fjogeleit))
- Loris Degioanni ([@ldegio](https://github.com/ldegio))
- Néstor Salceda ([@nestorsalceda](https://github.com/nestorsalceda))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Leonardo Di Donato ([leodido](http://github.com/leodido))
- Paulo Simoes ([@pasimoes](https://github.com/pasimoes))
- Spencer Krum ([@nibalizer](https://github.com/nibalizer))

### This week highlights


### Agenda

- [leogr] Migration from Bintray to S3 (ie. download.falco.org) [#1567](https://github.com/falcosecurity/falco/issues/1567)
  - Starting from April, Bintray will have some short service brown-outs
    - it's not clear if new package submissions will be accepted
  - Then, Bintray is going into the sunset on May 1st
  - The 0.28 release (due by 18th Mar) is the last opportunity to test the CI automation before the Bintray shutdown
  - Build deps already migrated to https://download.falco.org/dependencies/
    - PR [1572](https://github.com/falcosecurity/falco/pull/1572) needs approvals
  - New mechanism to manage DEB and RPM repositories
    - WIP [here](https://github.com/falcosecurity/falco/compare/build/publish-pkg-on-s3)

- Contributor of the Month
  - Frank https://twitter.com/falco_org/status/1369686856351309835?s=20

---

## 2021-03-03

### MC

- Spencer Krum ([@nibalizer](https://github.com/nibalizer))

### Who joined

- Magno Logan ([@magnologan](https://github.com/magnologan))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Loris Degioanni ([@ldegio](https://github.com/ldegio))
- Stefan Uygur ([@ostendali](https://github.com/ostendali))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Thomas Labarussias ([@Issif](https://github.com/Issif))

### This week highlights


### Agenda

- Falco release w/ debugging symbols? - > Open Github Issue  (@angelo follow up for next meeting)
- Contributor of the Month Nominations!  (Vote in Channel, will be selected on 3/10 meeting)
- Falcosidekick survey results

---

## 2021-02-24

### MC

- Spencer Krum ([@nibalizer](https://github.com/nibalizer))

### Who joined

- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Leonardo Di Donato ([@leodido](https://github.com/leodido))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- POP ([@danpopsd](https://github.com/danpopsd))
- Frank Jogeleit ([@fjogeleit](https://github.com/fjogeleit))
- Loris Degioanni ([@ldegio](https://github.com/ldegio))
- Stefan Uygur ([@ostendali](https://gitgub.com/ostendali))
- Scott Nichols ([@n3wscott](https://github.com/n3wscott))
- Bala ([@balasu](https://github.com/balasu))
- Steve Gargan ([@sgargan](https://github.com/sgargan))
- Michele Zuccala ([@zuc](https://github.com/zuc))
- Domenico Chirabino ([@dchirabino](https://github.com/dchirabino))
- Daniele Di Vito ([@danieledivito](https://github.com/danieledivito))

### This week highlights

- It's official now: libraries and drivers source code contributed to the CNCF (falcosecurity org).
  - Read more: https://falco.org/blog/contribution-drivers-kmod-ebpf-libraries

### Agenda

- [POP] Adoption Survey
  - get a pulse to the adoption of Falco
- [Thomas] Sidekick Outputs Form
  - Send user survey on outputs - [survey here](https://docs.google.com/forms/d/e/1FAIpQLSeXcJGB-4855PQ-qiB55XnMj18CZeKAjLm6TOEkh1aTiQAntw/viewform)
- [leodido] Improvements to the CONTRIBUTING and GOVERNANCE of the GitHub organization
  - PTAL https://github.com/falcosecurity/.github/pull/33
- [leodido/leogr] Archive kubernetes-response-engine
  - See [evolution#48](https://github.com/falcosecurity/evolution/issues/48)
- Falco release w/ debugging symbols? - > Open Github Issue

---

## 2021-02-17


### MC

Leonardo Di Donato ([@leodido](https://github.com/leodido))

### Who joined

- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Stefan Uygur[@ostendali](https://github.com/ostendali)
- POP ([@danpopsd](https://github.com/danpopsd))
- Loris degioanni ([@ldegio](https://github.com/ldegio))
- Ismail YENIGUL ([@ismailyenigul](https://github.com/ismailyenigul))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Néstor Salceda ([@nestorsalceda](https://github.com/nestorsalceda))
- Spencer Krum ([@nibalizer](https://github.com/nibalizer))
- Lorenzo Fontana ([@fntlnz](https://github.com/fntlnz))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))

### This week highlights

Lot of work under the hoods...

- On-going contribution of the libraries and drivers source code!
  - [1737](https://github.com/draios/sysdig/pull/1737)
  - [OWNERS](https://github.com/falcosecurity/libs/blob/master/OWNERS) file (as per proposal) okay
  - Prow (poiana) [setup](https://github.com/falcosecurity/test-infra/pull/314) okay
  - We'll go from here!
  - Blog posts and official announcements soon!

### Agenda

- [ismailyenigul] Commercial product images in Falco rules: to include or not to include
  - Discussion from Slack thread [here](https://kubernetes.slack.com/archives/CMWH3EH32/p1612990980436900)
  - [leodido] Let's define rules hygiene
    - Define what makes a container image ok to be in a Falco rule macro/list by default
    - Define where and how to provide extension points for Falco rule conditions
    - Define when we can include something in macros/list versus when we prefer to use the exceptions
- Review falco#1555
- [ismailyenigul] Talking about recent rules updates
- [thomas] FalcoSidekick UI
  - Welcome Frank Jogeleit!
- [ismailyenigul] Double-check the following blog post on AWS
  - https://aws.amazon.com/blogs/containers/implementing-runtime-security-in-amazon-eks-using-cncf-falco/


---

## 2021-02-10


### MC

Lorenzo Fontana ([@fntlnz](https://github.com/fntlnz))

### Who joined

- Leonardo Di Donato ([@leodido](https://github.com/leodido))
- POP ([@danpopsd](https://github.com/danpopsd))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Jonah Jones ([jonahjon](https://github.com/jonahjon))
- Loris Degioanni ([@ldegio](https://github.com/ldegio))
- Magno Logan ([@magnologan](https://github.com/magnologan))
- Stefan Uygur ([ostendali](https://github.com/ostendali))
- Massimiliano Giovagnoli ([maxgio92](https://github.com/maxgio92))


### This week highlights

- Contributor of the Month!


### Agenda

- [leodido] create a `falcosecurity/awesome-falco` repository?
  - goal: list all the projects regarding Falco disregarding they are in the falcosecurity organization or not
  - leodido to setup it!
- [Thomas] ask for incubation of [falcosidekick-ui](https://github.com/falcosecurity/evolution/issues/47)
  - goal: migrate the repo into main organization
  - [fjogeleit](https://github.com/fjogeleit) accepts to become official maintainer of UI
- [POP] end user/adopters community meeting
- [Lore] What's next for aarch64/armv7 releases?
  - [jonah] there are still some issues
  - We aim for 0.28
- Bintray migration
  - [leogr] volunteered
- [Magno] SIG-Security Meeting: MITRE for Containers today at 1pm EST
- [Magno] SANS CloudSecNext Summit CFP - https://survey.sans.org/jfe/form/SV_9EnNOTSmh0wv12J
- [Stefan] RedHat involvement in Falco community

---

## 2021-02-03

### MC

- POP ([@danpopsd](https://github.com/danpopsd))

### Who joined

- POP ([@danpopsd](https://github.com/danpopsd))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Loris Degioanni ([@ldegio](https://github.com/ldegio))
- Magno Logan ([@magnologan](https://github.com/magnologan))
- Leonardo Di Donato ([@leodido](https://github.com/leodido))
- Bala ([@balasu](https://github.com/balasu))
- Scott Nichols [@n3wscott](https://github.com/n3wscott)
- Spencer Krum [@nibalizer](https://github.com/nibalizer)
- Néstor Salceda [@nestorsalceda](https://github.com/nestorsalceda)
- Jonah Jones [@jonahjon](https://github.com/jonahjon)
- Lorenzo Fontana [@fntlnz](https://github.com/fntlnz)

### This week highlights

- APAC friendly community meeting timings
- Follow ups from 01-27 Meeting
  - Bring up potential Fedora builds in the future
  - Stefan work with RHEL for integration
  - VS Code, Nestor and new member of team to work on this and provide status
  - Status from Scott's PR
    - Merged. Time to follow up some cleaning and documentation.
- Contributor of the Month Voting!


### Agenda

- (leodido) update on technical docs:
  - we now have falcosecurity.dev thanks to the CNCF
  - will use to complete [PR 1513](https://github.com/falcosecurity/falco/pull/1513)
- (Issif) Falcosidekick UI (POC)
  - Link?
- bpf probe deployment strategies, co-re and porting to libbpf
- EBPF Colocated day for Kubecon NA (working with Cillium, kinvolk) (stay tuned)
- Open Floor

---

## 2021-01-27

### MC

- Jonah Jones ([jonahjon](https://github.com/jonahjon))

### Who joined

- Jonah Jones ([jonahjon](https://github.com/jonahjon))
- Magno Logan ([magnologan](https://github.com/magnologan))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Leonardo Di Donato ([leodido](https://github.com/leodido))
- Rajakavitha Kodhandapani ([Rajie](https://github.com/Rajakavitha1))
- Néstor Salceda ([@nestorsalceda](https://github.com/nestorsalceda))
- Stefan Uygur ([ostendali](https://github.com/ostendali))
- POP ([danpopsd](https://github.com/danpopsd))
- Domenico Chirabino ([domenicochi](https://github.com/domenicochi))
- Daniele Di Vito([danieledivito](https://github.com/danieledivito))
- Radhika Puthiyetath([radhikapc](https://github.com/radhikapc))
- Lorenzo Fontana ([fntlnz](https://github.com/fntlnz))
- kris nóva ([kris-nova](https://github.com/kris-nova))
- Bala ([bala](https://github.com/balasu))

### This week highlights

- @Bala is working with microK8s for a Falco add-on (https://github.com/ubuntu/microk8s/pull/1922)
- @Rajie and @Jonah Jones working on DCO Signoff fix (having go build issues): https://github.com/jonahjon/dco-plugin/pull/1/files.
  - TODO
    - Validate DCO steps in Readme and the fix
      - To add a 'DCO signoff' to your commit:
          1. Ensure that you have a local copy of your branch by [checking out the pull request locally via command line](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/checking-out-pull-requests-locally).
          2. Head to your local branch and type the following:
             ```git commit --amend --no-edit --signoff```
          3. Now your commits will have your signoff. Push the commit with the DCO signoff:
          ```git push --force-with-lease origin <branch_name>```
          Details of the Developer Certificate of Origin can be found at [developercertificate.org]         (https://developercertificate.org/).
    **The list of commits missing DCO signoff**:
    - Reach out to Leo and Kris about Go build issue
- Please review and maybe even test
- ***VICTORY LAP*** Falco Sidekick 300k downloads!
- [falco-exporter](https://github.com/falcosecurity/falco-exporter/releases/tag/v0.5.0) v0.5.0 now exports metrics about drops
- [driverkit](https://github.com/falcosecurity/driverkit) v0.3.0 now ubuntu-generic builders supports GKE kernels too
- [driverkit] stats and future supported distros

### Agenda

- Status of operating systems support in driverkit
  - Lorenzo's speech: Got stats RHEL top download miss
  - Google OS 2nd miss for GKE, TODO fix script for this
  - Bring up potential Fedora builds in the future
  - Stefan work with RHEL for integration
  - WishList item Preflight checks for Falco drivers
- Maybe once a month APAC friendly community meeting timings (to meet the localization team)
  - Dates/Times (Ask Apac people what day works best Still Weds?)
  - Put together Doodle in Slack for Day/Time/Cadence
  - Put to vote once have proposed
- Go to https://download.falco.org/?prefix=driver/5c0b863ddade7a45568c0ac97d037422c9efb750/ and look for "gke" substrings
- Take a look at Scott's PR https://github.com/falcosecurity/falcosidekick/pull/169
- Nestor -- VS code plugin status? :heart:
  - Nestor and new member of team to work on this and provide status next meeting.
- Note on rules for CVEs (CVE-2021-3156) https://github.com/falcosecurity/falco/issues/1540
  - Get Rule out for this, and market it!
  - Can we seperate rules from version release, to catch big ticket CVE's quickly?
  - Discuss about website changes to highlight CVEs news / blog posts

---

# Falco Community Call

[More Information](https://github.com/falcosecurity/community)
[Zoom Link](https://zoom.us/my/cncffalcoproject)
[Recording](https://)

## 2021-01-20

### MC

- POP

### Who joined

- Thomas Labarussias ([@Issif](https://github.com/Issif))
- POP ([@danpopsd](https://github.com/danpopsd))
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Rajakavitha Kodhandapani([@Rajie](https://github.com/Rajakavitha1))
- Scott Nichols ([n3wscott](https://github.com/n3wscott))
- Spencer Krum ([nibalizer](https://github.com/nibalizer))
- Leonardo Di Donato ([leodido](https://github.com/leodido))
- Loris Degioanni ([ldegio](https://github.com/ldegio))
- Jonah Jones ([jonahjon](https://github.com/jonahjon))
- Stefan Uygur ([ostendali](https://github.com/ostendali))
- Magno Logan ([magnologan](https://github.com/magnologan))
- Radhika Puthiyetath ([radhikapc](https://github.com/radhikapc))
- Lorenzo Fontana ([fntlnz](https://github.com/fntlnz))
- Angelo Puglisi ([deepskyblue86](https://github.com/deepskyblue86))
- Balasundaram ([balasu](https://github.com/balasu))

### This week highlights

- Falco 0.27.0 is out!
  - [Blog post](https://falco.org/blog/falco-0.27.0-a.k.a.-the-happy-2021-release/)
  - [Helm chart](https://github.com/falcosecurity/charts/tree/falco-1.7.1/falco) updated
  - New website :point_right: https://falco.org/
    - with versioned documentation (e.g. https://v0-26.falco.org/)!

- Libraries and drivers' sources donation
  - https://github.com/falcosecurity/falco/pull/1530

- Falcosidekick:
  - blog pos about Falcosidekick + Kubeless
  - Scott has improved his PoC with Knative
- Helm for Falco + Falcosidekick:
  - Falcosidekick is now a dependency in Falco Helm chart, we can deploy them together. If Falcosidekick is not enabled, a message is printed for promoting it.
- Falco+Sidekick demoed at Red Hat Openshift Commons.
  - [youtube](https://www.youtube.com/watch?v=K0qZW_xf2ew), demo at the end (~:52)
  - This is in the homepage now!

### Agenda

- (leodido) Driverkit 0.3.0 is out
  - Build Falco drivers for GKE 4.15 and 5.4 kernels using the ubuntu-generic builder
  - Fixes for (debian) kernels 5.10

- (leodido) Doxygen docs
  - https://github.com/falcosecurity/falco/pull/1513
  - falcosecurity.dev as perhaps a place for this
  - improve CONTRIBUTING guidelines
  - Leo/POP show you how to contribute to Falco (youtube)
