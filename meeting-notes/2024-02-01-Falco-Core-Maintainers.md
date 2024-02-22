# 2024-02-01 Falco Core Maintainers (monthly)

## MC

- leogr

## Who Joined

- Andrea Terzolo ([@Andreagit97](https://github.com/Andreagit97))
- Leonardo Grasso ([@leogr](https://github.com/leogr)) 
- Grzegorz Nosek ([@gnosek](https://github.com/gnosek))
- Melissa Kilby ([@incertum](https://github.com/incertum))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Luca Guerra ([@LucaGuerra](https://github.com/LucaGuerra))

## Agenda

- CNCF **Licensing issues** update (graduation blockers):
    - Requests status:
        - We are ok with libcurl and uthash
            - Governing Board should formalize in mid-Feb
        - For libelf, we have to switch to dinamic linking
            - https://github.com/falcosecurity/evolution/issues/359
        - For the [kernel module](https://github.com/cncf/foundation/issues/645) we have pinged several times, but there's no update yet 
    - N.B. If these requests aren't unblocked by the end of February, we won't be able to announce the Falco Graduation at Kubecon.
        > Within 2 weeks of the event [Kubecon]
        > 
        > Even if a project has passed a vote, if they have not announced and officially moved levels, they will not be included as an incubating or graduated project.
        > 
        > source: https://github.com/cncf/toc/blob/main/process/project_proposals.md#timelines
- Kick-off discussion about **Falco 1.0 roadmap**
    - Focus on stability (ie reduce adopter burderns when operating Falco)
        - Features adoption and deprecation policies 
            - In the making https://github.com/falcosecurity/falco/pull/2986
        - Notable deprecations and clean-ups must happens before 1.0
        - Naming consistency
    - eBPF first approach
    - Falco distrubution
        - Falco is missing or (out-to-date) in most marketplaces (ie. GCP, AWS, Azure)
        - Falco packages are currently not shipped by common Linux distros. Getting them included will allow us to reach more users and simplify the installation/upgrade process.
            - Talking about packages: Consider removing DKMS dependency from the official RPM package, a common blocker for many adopters who really just want to use Falco w/ eBPF 
        - [Package checksums](https://github.com/falcosecurity/falco/issues/2950) are not published
        - Integration with artifacthub.io is poor (eg. [rules](https://artifacthub.io/packages/search?kind=1&ts_query_web=falco&sort=relevance&page=1) are not curated)
        - Try to attract SRE talent to the project to make "deployment" easier and more robust
    - Rule systax
        - We have a list of long-standing issues that require the introduction of significant breaking changes and feature additions as well.
        - Condition syntax needs to be stabilized so that we can support it in the long term
    - Extensive Kubernetes Integration
        - We may lack helpful Kubernetes information for detection (for example, [[PROPOSAL] Inject Kubernetes Control Plane users into Falco syscalls logs for kubectl exec activities](https://github.com/falcosecurity/falco/issues/2895)). We need to investigate
        - K8s Audit Log plugin seems to be [actively used](https://github.com/orgs/falcosecurity/packages?repo_name=plugins), however it is not really curated and we miss intregration with cloud providers  (i.e. [AKS integration](https://github.com/falcosecurity/plugins/issues/368) and [GKE integration](https://github.com/falcosecurity/plugins/issues/243))
    - Cloud providers' integrations
        - Enhancing events with metadata from cloud providers can boost the relevance of alerts. This is particularly beneficial for users with hybrid clouds, multi-tenant environments, or multiple clusters or regions. Aggregating these alerts in an SIEM enhances their effectiveness.
    - Integrated Metrics
        - [Brainstorming: integrate Prometheus /metrics handler in Falco](https://github.com/falcosecurity/falco/issues/1772)
        - [[TRACKING] Create a more coherent stats model for libs and consumer](https://github.com/falcosecurity/libs/issues/1463)
        - Distinguish between current `metrics:` in falco.yaml and metrics around Falco's rule (see [falcosidekick-prometheus](https://github.com/falcosecurity/falcosidekick#prometheus)) -> perhaps we can add anotehr category for rules metrics, but push to libs to for once have a unified `metrics_collector` living in libsinsp? candidate rules metrics: [counters per rule](https://github.com/falcosecurity/falco/issues/421#issue-362148563), [rule event source counters](https://github.com/falcosecurity/falco/issues/530#issue-409085139), related to the TODO syscalls counter
    - What are Falco's flagship top features?
        - Make flahship features even more robust -> for instance the container and k8s integration should be world-class and much more robust (we have a few libs PRs open in this regard and it is related to aboves "Extensive Kubernetes Integration" items)
        - Strong kernel version range support + multiple archs + multiple drivers
        - Open up Plugin system more
    - Branding of Falco beyond Kubernetes (a common misconception is that Falco ONLY works in Kubernetes -> it still seems not clear to many that it works on any Linux broadly speaking)
        - [leogr's question]: Do you mean Falco on hosts? May we need more host-specific detections?
    - Minor Important Enhancements -> 1.0.0
        - [Follow standard CLI args conventions](https://github.com/falcosecurity/falco/issues/3049)
        - Continued cleanup of legacy configs, e.g. [Refactor and simplify legacy syscall_event_drops](https://github.com/falcosecurity/falco/issues/3050)
        - ...
    - Re-evaluate default configs along with shipping a few best practice configs for certain environments -> related to the new Troubleshooting Guides
    - Most adopters' don't know what to do with Falco alerts, how to operationalize them, how to respond to them? What is the projects' roadmap in this regard (related to shipping and ditribute Falco more effectively)
    - Welcome to the world of machine intelligence
        - [docs(proposals): introduce on host anomaly detection framework](https://github.com/falcosecurity/falco/pull/2655) let's not miss the opportunity to push on this front as OSS security project
        - Discuss extension to self-monitoring and re-adjusting configs and settings
        - [leogr's question]: I like this, but I see this more like a parallel initiative than a 1.0 roadmap
    - Additional performance optimizations for high load servers -> see issues referenced at teh bottom of https://falco.org/docs/troubleshooting/dropping/
    - TODO:
        - create tracking issue
        - possibly announce the roadmap during the maintainer track
- **Falco 0.38 priorities**
    - Remove translation from the website for now
    - Items to be reviewed https://github.com/falcosecurity/falco/milestone/37
    - Extend Falco's rules condition syntax
        - https://github.com/falcosecurity/falco/issues/2403
        - compare fields
        - case (in)sensitive operators
        - transfomers/functions:
            - b64
            - tolower
            - toupper
    - Follow-up on the driver loader
        - Introduce a driver automatic selection mechanism
        - Possibly, decouple Falcoctl from Falco release cycles
        - Switch to modern probe by default (assuming a fallback to other drivers)?
            - Melissa yes
            - Andrea yes
            - Luca yes
            - Leo yes
    - Try to open up Plugin framework more
        - Missing API to access filter checks
        - Extend the state API
        - Rust SDK (nice-to-have)
    - Container engine robustness
    - Get Metrics into an acceptable state + light weight Prometheus support
        - https://github.com/falcosecurity/libs/pull/1652
    - UndefinedBehaviorSanitizer in libs, AddressSanitizer in Falco, better coverage
    - ... 

- Language syntax - ideas for the future:
     - TBD regexps
        - performance impact
        - support in bytebuffer only?
    - outputs
        - functions for concatenation?
        - functions for process hierarchy lookups?
        - macros?
        - plugins to extend features
    - Idea for the future https://github.com/google/cel-spec
