# 2023-11-02 Falco Core Maintainers (monthly)

## MC
- Melissa Kilby [@incertum](https://github.com/incertum)

## Who Joined
- Melissa Kilby [@incertum](https://github.com/incertum)
- Federico Di Pierro [@fededp](https://github.com/fededp)
- Mauro Moltrasio [@Molter73](https://github.com/Molter73)
- Grzegorz Nosek [@gnosek](https://github.com/gnosek)
- Jason Dellaluce [@jasondellaluce](https://github.com/jasondellaluce)
- Luca Guerra [@LucaGuerra](https://github.com/LucaGuerra)

## Highlights

- Technical debt cleanup discussion
- k8s client and k8s user
- CountMinSketch Probabilistic Counting and Filtering discussion
- Official builder containers need a revamp -> plus toturials or website build instructions need to be updated accordingly

## Agenda

Notes:

- Status on CNCF Licensing
    - https://github.com/cncf/foundation/issues/629
    - https://github.com/cncf/foundation/issues/645
- Status on memleaks / segfaults etc, what else can we do? https://github.com/falcosecurity/libs/issues/1468   
  - Reject raw pointers? We should still replace them with smart pointers whenever possible. This will make ownership more clear and transparent in libsinsp.
  - Pass by parameter or by reference when possible.
  - Remove things that are not needed from the core code base first. Removing udig and mesos is more difficult because they are more tangled than removing the old k8s client code base. @jasondellaluce volunteered to tackle this (mesos + k8s client removal after we have the new k8s client implementation -> coordinate with @Andreagit97).
  - Consider prioritizing removing the respective code lines in `sinsp next` first. (@gnosek comment)
- Check in on k8s client refactor https://github.com/falcosecurity/libs/pull/1377#discussion_r1344311159 (-> Andrea shared ETA end of November 2023)
  - [luca] see: https://github.com/falcosecurity/evolution/issues/335
  - Related to above briefly discuss new proposal https://github.com/falcosecurity/falco/issues/2895 to inject Kubernetes user information into Falco logs
  - Is also related to some older ask to expose more k8s metadata fields that are static on a per host basis https://github.com/falcosecurity/falco/issues/1704 such as cluster name, region, account id etc
- Melissa to provide some updates re https://github.com/falcosecurity/libs/pull/1453 CountMinSketch Powered Probabilistic Counting and Filtering, see broader Falco proposal https://github.com/falcosecurity/falco/pull/2655 
    - No one said it's a bad idea, this means a yes for the Falco use case
    - Jason said it appears to be possible as CPP plugin as it does not fall outside the capabilities we support today in the CPP plugin
- Official builder containers for adopters? Update and provide new ones for modern BPF ...
- Modern builder containers?
    - Seems we have lost a universal builder container adopters can pull? https://github.com/falcosecurity/falco/tree/master/docker/builder
    - If adopters cannot build because of outdated instructions, let's add what we need here https://github.com/falcosecurity/falco-website/issues/1091 
- Some items to check in from last time (see notes from 2023-10-05):
    - CNCF TAG Environmental Sustainability, Green Review WG -> in progress, no new items to discuss (Melissa)
    - When do we do the big code removals in libs re udig and mesos?
    - LSM hooks for open* syscall replacement -- seems to come up again and again (longer term maybe once we reach Falco 1.x), also fo interest for execve* use case
    - falcoctl as driver loader -> in flight
    - Falco configs for partial rules overrides in flight / assigned
    - libsinsp metrics extension -> PRs already up
    - ia32 emulation done (wohoo)
    - Make exceptions more user-friendly -> TBD 
    - Work on DNS refactor? -> TBD
    - Improve docs for rules onboarding and always try to improve guides in general https://github.com/falcosecurity/falco-website/issues/1177, plus provide more clarity around k8s plugin especially now that it will be refactored
