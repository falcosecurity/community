# Falco Community Call

[More Information](https://github.com/falcosecurity/community)
[Zoom Link](https://zoom.us/my/cncffalcoproject)
[Recording](https://youtube.com/playlist?list=PLgVVUpW8NIJAaZtszf1_nxB2y6mQrlY4s)


## 2022-11-16

### MC

- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))

### Who joined

1. - Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
1. - Thomas Labarussias [Issif](https://github.com/Issif)
1. - Leonardo Grasso [leogr](https://github.com/leogr)
1. - Adao Oliveira Junior ([junior](https://github.com/junior))
1. - Stanley Chan [happy-dude](https://github.com/happy-dude)
1. - Aldo Lacuku ([alacuku](https://github.com/alacuku))
1. - Teryl Taylor ([terylt](https://github.com/terylt))
1. - Mauro Moltrasio ([Molter73](https://github.com/Molter73))
1. - Jacqueline Salinas ([jsalinas29](https://github.com/jsalinas29))
1. - Federico Di Pierro ([@fededp](https://github.com/FedeDP))
1. - Vicente JJ. Miras ([vjjmiras](https://github.com/vjjmiras))
1. - Fred Araujo ([@araujof](https://github.com/araujof))
1. - Massimiliano Giovagnoli ([@maxgio92](https://github.com/maxgio92))

### This week highlights

- Falco applied for graduation 🚀
    - https://github.com/cncf/toc/pull/956
        - Please share it on the social media platform you like, and
        - We would love a 👍, ❤️, or 🚀 on that PR
        - Read the [blog](https://falco.org/blog/falco-applies-for-graduation/)
    - We already got two sponsors: Emily Fox, Justin Cormack
        - https://docs.google.com/document/d/1jpoKT12jf2jTf-2EJSAl4iTdA7Aoj_uiI19qIaECNFc/edit
        - https://github.com/cncf/toc/pull/956#issuecomment-1315561052

### Agenda

- [Andreagit97] Publish Falco pre-release packages for the modern BPF probe
    - pre-release coming next week with a bin package and docker image for x86_64 and aarch64
    - useful for testing compatibility
    - a blogpost is in the works as well to detail the probe and how to use it
    - https://github.com/falcosecurity/falco/pull/2282
- [Jacque] Oracle mtg next week & they can help w/documentation 
    - where do we need help?
    - [teryl] a lot of questions in the Falco community are releated to compatibility, it would be good to start from there
    - [fred] questions related to the drivers and kernel headers
    - [aldo] managed cluster deployment, people might be using wrong parameters, would be better if the doc were more consistent and comprehensive
        - values.yaml might be different from documentation
- [LucaGuerra] Proposing a 0.33.1 release for a quick fix on gVisor and k8s
- [leogr] Proposal: Use GitHub Projects to manage the Falco roadmap
- [jacque] graduation: we need 5 - 7 adopters for the TOC to interview. Lmk if you know someone who uses Falco and would be willing to get interviewed
- [leogr] Cancelling calls during holidays
    - Usually we canceled during Thanksgiving and Christmas break
    - cancel next week's call
    - last Falco call of the year on dec 14th, first call of 2023 on jan 11th


## 2022-11-09

### MC

- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))

### Who joined

1. - Leonardo Grasso ([@leogr](https://github.com/leogr))
1. - Jacque Salinas([@jsalinas32](https://github.com/jsalinas32))
1. - Federico Di Pierro ([@fededp](https://github.com/FedeDP))
1. - Lorenzo Susini ([@loresuso](https://github.com/loresuso))
1. - Aldo Lacuku ([alacuku](https://github.com/alacuku))
1. - Michele Zuccala ([@zuc](https://github.com/zuc))
1. - Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
1. - Teryl Taylor ([terylt](https://github.com/terylt))

### This week highlights

- Falco applied for graduation 🚀
    - https://github.com/cncf/toc/pull/956
        - Please share it on the social media platform you like, and
        - We would love a 👍, ❤️, or 🚀 on that PR
        - Read the [blog](https://falco.org/blog/falco-applies-for-graduation/)
    - We already got two sponsors: Emily Fox, Justin Cormack
        - https://docs.google.com/document/d/1jpoKT12jf2jTf-2EJSAl4iTdA7Aoj_uiI19qIaECNFc/edit


### Agenda

- [leogr] Proposal: Use GitHub Projects to manage the Falco roadmap
- Cancelling calls during holidays
- Postponing the same topics to the next week since not so many folks joined
    (probably because they have not noticed the call time is in UTC)

### Closing



## 2022-11-02

### MC

### Who joined

1. - David Windsor ([@dub](https://github.com/dwindsor))
1. - Logan Bond ([@EXONER4TED](https://github.com/exoner4ted))
1. - Federico Di Pierro ([@fededp](https://github.com/FedeDP))
1. - Mauro Moltrasio ([Molter73](https://github.com/Molter73))
1. - Matthew White ([matthewjwhite](https://github.com/matthewjwhite))
1. - Aldo Lacuku ([alacuku](https://github.com/alacuku))
1. - Lorenzo Susini ([@loresuso](https://github.com/loresuso))
1. - Vicente JJ. Miras ([vjjmiras](https://github.com/vjjmiras))
1. - Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
1. - Jacqueline Salinas ([jsalinas32](https://github.com/jsaslinas32))
1. - Teryl Taylor ([terylt](https://github.com/terylt))
1. - Fred Araujo ([@araujof](https://github.com/araujof))
1. - Michele Zuccala ([@zuc](https://github.com/zuc))
1. - Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
1. - Angelo Puglisi [@deepskyblue86](https://github.com/deepskyblue86)
1. - Leonardo Grasso ([@leogr](https://github.com/leogr))
1. - Sumit Bindal ([@sumitb](https://github.com/sumitb))

### This week highlights

- [fededp] Syscalls-bumper job is now active! https://github.com/falcosecurity/libs/pull/693
- [fededp] Bundled libelf library https://github.com/falcosecurity/libs/pull/686

### Agenda

- [dub] Propose logan for driverkit maintainer
- [jacque/leo] graduation [doc](https://hackmd.io/Hqoew7jMQ7qcZVXA8h14nQ)

### Closing

## 2022-10-19

### MC
- [Issif](https://github.com/Issif)

### Who joined

1. - Federico Di Pierro [@fededp](https://github.com/FedeDP)
1. - Mauro Moltrasio [Molter73](https://github.com/Molter73)
1. - Leonardo Grasso [@leogr](https://github.com/leogr)
1. - Fred Araujo [@araujof](https://github.com/araujof)
1. - [matthewjwhite](https://github.com/matthewjwhite)
1. - Vicente JJ. Miras [vjjmiras](https://github.com/vjjmiras)
1. - Teryl Taylor [terylt](https://github.com/terylt)
1. - Lorenzo Susini [@loresuso](https://github.com/loresuso)
1. - Jason Dellaluce [@jasondellaluce](https://github.com/jasondellaluce)
1. - Mahé Tardy
1. - [Stanley Chan](https://github.com/happy-dude)
1. - Angelo Puglisi [@deepskyblue86](https://github.com/deepskyblue86)


### This week highlights

- Falco 0.33 has been released! 🎉 https://falco.org/blog/falco-0-33-0/
    - 1 hour ago (5 minutes ago actually)!


### Agenda

- [leogr/aldo] Helm chart to support Falco 0.33 will be relased soon
    - https://github.com/falcosecurity/charts/pull/409
- [lore/aldo/luca/leogr] We are going to release a beta version of [falcoctl](https://github.com/falcosecurity/falcoctl) this week
    - Artifacts already published! https://github.com/orgs/falcosecurity/packages
- [Issif] A plugin to consume K8S audit logs from EKS clusters will be released soon
- Who's going to the Kubecon NA next week?
- Canceling next week's call because of KubeCon NA 

### Closing
- 
