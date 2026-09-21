## 2026-07-15

### MC

- [Gerald Combs](https://github.com/geraldcombs)

### Who joined

- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Mauro Moltrasio](https://github.com/molter73)
- [Alessandro Cannarella](https://github.com/c2ndev)

## Agenda

- Proposed libs feature: [Raw block support](https://github.com/falcosecurity/libs/pull/3038)
- Serve forced hot reload requests

## 2026-06-17

### MC

- [Leonardo Di Giovanna](https://github.com/ekoops)

### Who joined

- [Alessandro Cannarella](https://github.com/c2ndev)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Gerald Combs](https://github.com/geraldcombs)

## Agenda

- Falco 0.44.x released
  - Blog post - https://falco.org/blog/falco-0-44-0/
  - Falco 0.44.1 released - https://github.com/falcosecurity/falco/releases/tag/0.44.1
- Falco Operator [0.4.0](https://github.com/falcosecurity/falco-operator/releases/tag/v0.4.0) release and Chart [0.3.0](https://github.com/falcosecurity/charts/blob/master/charts/falco-operator/CHANGELOG.md) release
    - Falco default version bumped to 0.44.1 - [#352](https://github.com/falcosecurity/falco-operator/pull/352)
    - Exclude label propagation to to generated Falco resources - [#351](https://github.com/falcosecurity/falco-operator/pull/351)
    - Introduced [Version Matrix](https://github.com/falcosecurity/falco-operator/blob/main/docs/version-matrix.md) documentation page
    - Other minor fixes

## 2026-05-06

### MC

- [Jonas Rosland](https://github.com/jonasrosland)

### Who joined

- [Jonas Rosland](https://github.com/jonasrosland)
- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Libby Schulze](https://github.com/libbyschulze1)
- [Dylan Lee](https://github.com/atleticomadrid07)

## Agenda

- [Prempti](https://prempti.falco.org) launch last week, comments and feedback
- Falco Operator Helm Chart v0.1.0 release:
    -  [Official Installation guide](https://github.com/falcosecurity/falco-operator/blob/main/docs/installation.md)
    -  [Helm chart repo](https://falcosecurity.github.io/charts)

## 2026-05-06

### MC

- [Gerald Combs](https://github.com/geraldcombs)

### Who joined

- [Leonardo Grasso](https://github.com/leogr)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Jonas Rosland](https://github.com/jonasrosland)
- Libby Schulze
- [Mauro Moltrasio](https://github.com/Molter73)

## Agenda

- https://github.com/falcosecurity/prempti (a.k.a coding-agents-kit):
    -  moved into `falcosecurity`
    -  [v0.2.0](https://github.com/falcosecurity/prempti/releases/tag/v0.2.0) released!
- Delivered fix for lack of UTF-8 sanitization
    - [Incosistent string sanitization and missing UTF-8-awareness](https://github.com/falcosecurity/libs/issues/2965)
- Upcoming releases (Libs 0.25.0 and 0.26.0, and Falco 0.44.0)
- Falco Sidekick: we are cooking something cool!
- Let's meet at KCD New York https://kcdnewyork.com/
- CNCF webinar May 12th!
    - [Cloud Native Live: Falco's Nest & the Evolution of Runtime Security
](https://community2.cncf.io/events/details/cncf-cncf-online-programs-presents-cloud-native-live-falcos-nest-amp-the-evolution-of-runtime-security/)
- [Falco Virtual Workshop May 12th!](https://go.sysdig.com/Falco-Virtual-Community-Workshops.html)

## 2026-04-22

### MC

- [Leonardo Grasso](https://github.com/leogr)

### Who joined

- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Jonas Rosland](https://github.com/jonasrosland)
- Libby Schulze
- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Gerald Combs](https://github.com/geraldcombs)

## Agenda

- `coding-agents-kit`
  - [Proposal](https://github.com/falcosecurity/evolution/issues/512)
  - https://github.com/leogr/coding-agents-kit
- Helm Chart for Falco Operator
- [Inconsistent string sanitization and missing UTF-8-awareness](https://github.com/falcosecurity/libs/issues/2965)
- Survey result will be published soon!

## 2026-04-08

### MC

- [Iacopo Rozzo](https://github.com/irozzo-1A)

### Who joined

- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Leonardo Grasso](https://github.com/leogr)

## Agenda

- KubeCon + CloudNativeCon EU 2026 debrief
- Update on [multi-thread initiative](https://github.com/falcosecurity/falco/issues/3749)
- [Falco Operator 0.2.0](https://falco.org/blog/falco-operator-0-2-0/)

## 2026-03-11

### MC

- [Leonardo Di Giovanna](https://github.com/ekoops)

### Who joined

- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Leonardo Grasso](https://github.com/leogr)
- [Gerald Combs](https://github.com/geraldcombs)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Jonas Rosland](https://github.com/jonasrosland)
- Libby Schulze

## Agenda

- BPF iterator Support updates
    - [Tracking issue](https://github.com/falcosecurity/libs/issues/2879)
-  Multi-thread Support updates
    -  Iacopo is evaluating his PoC:
        -  libs code: https://github.com/irozzo-1A/agent-libs/tree/experiment/folly-concurrent-hashmap
        -  falco code: https://github.com/irozzo-1A/falco/tree/experimental/multi-thread
- Falco Operator
    - Repository: https://github.com/falcosecurity/falco-operator
    - Release expected for the next week
- Join us at KubeCon + CloudNativeCon 2026 - Amsterdam, 23-26 March
    - Event link: https://events.linuxfoundation.org/kubecon-cloudnativecon-europe/
    - No community call on 25 March
    - Falco Workshop on Monday March 23: https://sysdig.pathfactory.com/kceu26-falco-workshop
- Falco survey - last day March 13!
    - https://forms.gle/6o6AaWCVa8UAgMcWA

## 2026-02-25

### MC

- [Alessandro Cannarella](https://github.com/c2ndev)

### Who joined

- [Jonas Rosland](https://github.com/jonasrosland)
- [Gerald Combs](https://github.com/geraldcombs)
- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Marko Zbirka]
- [John Bain]
- [Libby Schulze]
- [Kapil Agrawal]


## Agenda

- Multi-thread Support updates: Iacopo will share the latest progress on [multi-thread support for Falco](https://github.com/falcosecurity/falco/issues/3749) 
- Falco Operator: project update and roadmap
- Falco Ecosystem: introducing [falco-lsp](https://github.com/falcosecurity/falco-lsp)
    - Falco Rules VSCode Extension: Alessandro will demo the new VSCode extension for Falco rules
    - Language Server Protocol
- [Falco survey blog post](https://github.com/falcosecurity/falco-website/pull/1533)


## 2026-02-11

### MC

- [Gerald Combs](https://github.com/geraldcombs)

### Who joined

- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Brandt Keller](https://github.com/brandtkeller)
- [Mauro Moltrasio](https://github.com/molter73)
- [Alessandro Cannarella](https://github.com/c2ndev)


## Agenda

- [Libs and plugins changes required for Stratoshark](https://docs.google.com/presentation/d/1NBusHGgGM8DAOLAT8w5fls_Vw7DU_DCw0C6JjR6Igm8/edit?usp=sharing)
- [Offline Documentation and Zarf](https://github.com/zarf-dev/zarf)


## 2026-01-28

### MC

- [Iacopo Rozzo](https://github.com/irozzo-1A)
 
### Who joined

- [Jonas Rosland](https://github.com/jonasrosland)
- [Gerald Combs](https://github.com/geraldcombs)
- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Leonardo Grasso](https://github.com/leogr)
- [Alessandro Cannarella](https://github.com/c2ndev)
- Libby Schulze
- Rui Zhao
- Wajih UI Hassan


## Agenda

- Update about Falco release 0.43.0
    - https://falco.org/blog/falco-0-43-0/
- Rui Zhao to present [Nitro](https://dartlab.org/assets/pdf/nitro.pdf) a tamper-evident logging system built on eBPF
- Community initiatives (Jonas & Libby)
    - [Contributor stipends, feature grants, and technical writer stipend](https://crowdfunding.lfx.linuxfoundation.org/projects/falco)
    - During the next 6 months, we would like to:
    - Go over [OpenSSF Best Practices](https://www.bestpractices.dev/en/projects/2317/passing) and update as needed
    - Go over [Scorecard.dev](http://scorecard.dev/viewer/?uri=github.com/falcosecurity/falco) and update as needed
        - See what, if anything, we would like to improve
    - Updates to the Falco website
        - Updated to Hugo 0.154.5, NPM 11.8.0, and Node 24.13.0
        - Next step is to update the Docsy theme from 0.3.0 to 0.13.0, using the modern [Hugo module method](https://www.docsy.dev/docs/updating/convert-site-to-module/)
        - I see references to a future MITRE ATT&CK page, is that still something you want to have?
        - Potential for documentation on how to run Falco in air-gapped environments using [Zarf](https://zarf.dev)
    - Present Falco and Falcosidekick to other OSS communities
    - Review CNCF membership benefits and contributions available to Falco quarterly/annually
- Multi-thread Support: A request for feedback on the [high-level proposal for multi-threading](https://github.com/irozzo-1A/falco/blob/falco-multi-thread-proposal/proposals/20251205-multi-thread-falco-design.md).


## 2026-01-14

### MC

- [Leonardo Grasso](https://github.com/leogr)
 
### Who joined

- [Mauro Moltrasio](https://github.com/Molter73)
- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Alessandro Cannarella](https://github.com/c2ndev)
- [Gerald Combs](https://github.com/geraldcombs)

## Agenda

- Welcome back and happy new year!
- GPG Key Rotation for Falco Packages (2026)
    - https://falco.org/blog/gpg-key-rotation-2026/
    - Rotation complete
    - Old revokation to be published soon
- Falco 0.43 RC1
    - https://github.com/falcosecurity/falco/releases/tag/0.43.0-rc1
    - https://github.com/falcosecurity/falco/issues/3770
- WIPs on falcoctl
- https://github.com/takaosgb3/falco-plugin-nginx 


## 2025-12-17

### MC

- [Leonardo Di Giovanna](https://github.com/ekoops)
 
### Who joined

- [Jonas Rosland](https://github.com/jonasrosland)
- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Gerald Combs](https://github.com/geraldcombs)
- [Leonardo Grasso](https://github.com/leogr)
- [Mauro Moltrasio](https://github.com/Molter73)

### Agenda

- Deprecation proposal for legacy probe, gVisor libscap engine and gRPC output
    - Proposal: https://github.com/falcosecurity/falco/pull/3755
    - More info: https://www.youtube.com/watch?v=5JoNk7_Sors (KubeCon North America 2025 Maintainer track recording)
- Upcoming libs 0.23.0 release. Major changes:
    - Bump drivers minimum required kernel version to 3.10 -> https://github.com/falcosecurity/libs/pull/2722
    - Default to sched/sched_process_exec tracepoint on all architectures -> https://github.com/falcosecurity/libs/pull/2726
    - Add filename parameter to PPME_SYSCALL_EXECVE_19_X -> https://github.com/falcosecurity/libs/pull/2735
- Jonas introduced himself and shared he's working on a funding initiative for Falco


## 2025-12-03

### MC

- [Iacopo Rozzo](https://github.com/irozzo-1A)
 
### Who joined

- [Ari Rubinstein](https://github.com/arirubinstein)
- [Leonardo Grasso](https://github.com/leogr)
- [Brenno Oliveira](https://github.com/brennoo)
- [Gerald Combs](https://github.com/geraldcombs)

### Agenda

- Maintenance tasks
    - Kernel testing matrices update https://github.com/falcosecurity/kernel-testing/pull/101
    - Refresh of the GPG signing key for RPM and DEB packages https://hackmd.io/KZ_mKNS0T26pRiH2s1igZg
- Multi-threaded Falco? https://github.com/falcosecurity/falco/issues/3749
- Container plugin NPEs [GH issue](https://github.com/falcosecurity/plugins/issues/1076)
- fuzzing!

## 2025-11-19 No community call!

**This week community call has been cancelled!**

See you at the next one, scheduled for Dec 3rd. 


## 2025-11-05

### MC

- [Leonardo Grasso](https://github.com/leogr)
 
### Who joined

- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Vicente J. Jiménez Miras](https://github.com/vjjmiras)
- [Angelo Puglisi](https://github.com/deepskyblue86)

### Agenda

- Falco 0.42 Capture feature overview
  - https://falco.org/blog/falco-0-42-0/
- Hotfix coming soon! (ie. 0.42.1)
  - Upgrade to libs [0.22.2](https://github.com/falcosecurity/libs/releases/tag/0.22.2)
  - Upgrade to container plugin [v0.4.1](https://github.com/falcosecurity/plugins/blob/main/plugins/container/CHANGELOG.md#v041)
- KubeconNA 2025: see you in Atlanta next week!
    - ⚡️ [Lightning Talk](https://lnkd.in/dVGCQfHd) 👉 "When Falco Spots Trouble, The Shark Swims In" 🦈 
    - ☁️ [Maintainer Track](https://lnkd.in/dqjAHZVk) 👉 Beyond the Cloud(s): Falco’s Ascent in Performance and Deep Visibility 🔥 
    - ...and if it happens to you to be in Atlanta, 
    feel free to stop by the **Falco Project Kiosk 13A** in the Solutions Showcase and say hi in person 



## 2025-10-22

### MC

- [Gerald Combs](https://github.com/geraldcombs)
 
### Who joined

- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Leonardo Grasso](https://github.com/leogr)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Iacopo Rozzo](https://github.com/irozzo-1A)


### This week highlights

- Falco 0.42 is out!
  - https://falco.org/blog/falco-0-42-0/

### Agenda

- Stratoshark demo


## 2025-10-08

### MC

- [Iacopo Rozzo](https://github.com/irozzo-1A)

### Who joined

- [Iacopo Rozzo](https://github.com/irozzo-1A)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Leonardo Grasso](https://github.com/leogr)
- [Angelo Puglisi](https://github.com/deepskyblue86)
- [Ari Rubinstein](https://github.com/arirubinstein)
- [Andres Orbe](https://github.com/AOrps)

### Latest news

- Falco 0.42 release status
    - https://github.com/falcosecurity/falco/issues/3677

### Lightning Talk

- [Plugin event schema version proposal](https://github.com/falcosecurity/libs/blob/master/proposals/20250923-plugin-system-event-schema-versioning.md)


## 2025-09-24

### MC

- [Leonardo Di Giovanna](https://github.com/ekoops)

### Who joined

- [Leonardo Grasso](https://github.com/leogr)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Iacopo Rozzo](https://github.com/irozzo-1A)

### Latest news

- Welcome to new falcosecurity/libs maintainers/reviewers!
    - [deepskyblue86](https://github.com/deepskyblue86) (maintainer)
    - [terror96](https://github.com/terror96) (reviewer)
    - [irozzo-1A](https://github.com/irozzo-1A) (reviewer)
- Updates on drop enter events initiative
    - Completed drop of system call enter events generation, parsing and testing code (tracked in https://github.com/falcosecurity/libs/issues/2588)
        - drivers do not generate anymore enter events!
    - WIP on enter event deprecation at multiple levels:
        - WIP on scap-converter to seamless handle enter events coming from old scap-files
        - WIP on internal parsing layers to avoid propagation of TOCTOU mitigation enter events to upper layers
        - WIP on `event.dir='>'` deprecation
- Release postponed to 15 Oct due to drop enter events initiative
    - [Release Tracking issue](https://github.com/falcosecurity/falco/issues/3677)
    - Release managers:
        - [Leonardo Di Giovanna](https://github.com/ekoops)
        - [Leonardo Grasso](https://github.com/leogr)
    - Shadow:
        - [Iacopo Rozzo](https://github.com/irozzo-1A)
    

## 2025-09-10 No community call!

See you at the next one, scheduled for Sept 24th. 

## 2025-07-30

### MC

- [Federico Di Pierro](https://github.com/fededp)

### Who joined

- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Mauro Moltrasio](https://github.com/Molter73)

### Latest news

- Updates on the multiple Falco 0.41.x issues -> https://docs.google.com/presentation/d/1TF_BwKaQDkkqFPz5KUXJgqVmiiSoeHdwxJq6jhuUOxA/edit?usp=sharing
- Next community call canceled for holidays! 

## 2025-07-16

### MC

- [Leonardo Di Giovanna](https://github.com/ekoops)

### Who joined

- [Mauro Moltrasio](https://github.com/Molter73)
- [Leonardo Grasso](https://github.com/leogr)
- [Phil Porada](https://github.com/pgporada)
- [Ari Rubinstein](https://github.com/arirubinstein)

### Latest news

- Updates on the "Extend syscall exit events with syscall enter events parameters" initiative: https://github.com/falcosecurity/libs/issues/2427
    - Original proposal: https://github.com/falcosecurity/libs/blob/master/proposals/20240901-disable-support-for-syscall-enter-events.md
- Discussing configuration issue reported recently: https://github.com/falcosecurity/falco/issues/3642

### Discussion

- falcosidekick/falcosidekick-ui discussion with Phil
    - Some redis output changes for both falcosidekick and falcosidekick-ui
    - A PR with a proposal to store web assets embedded in the falcosidekick-ui binary rather than on the filesystem adjacent to the binary.
    - When storing events in redis and using falcosidekick/falcosidekick-ui, configure falcosidekick with the `webui` output and falcosidekick-ui to store in redis.
    - ```
        [falco] --[event]--> [falcosidekick] --> [falcosidekick-ui] --> [redis]
      ```



## 2025-07-02

### MC

- Leonardo Grasso

### Who joined

- [Leonardo Grasso](https://github.com/leogr)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Ari Rubinstein](https://github.com/arirubinstein)
- [Mauro Moltrasio](https://github.com/Molter73)

### Latest news

- Falco [0.41.3](https://github.com/falcosecurity/falco/releases/tag/0.41.3) released!
    - This release just upgrades the container plugin to v0.3.1 in order to fix a [potential crash when the healthcheck probe args are null](https://github.com/falcosecurity/falco/issues/3626)
- Status update about the syscall exit events extension initiative supporting the syscall enter events drop initiative
    - [new(proposal): disable support for syscall enter events](https://github.com/falcosecurity/libs/pull/2068)
    - [[Tracking] Extend syscall exit events with syscall enter events parameters](https://github.com/falcosecurity/libs/issues/2427)




## 2025-06-18

### MC

- Leonardo Di Giovanna

### Who joined

- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Ari Rubinstein](https://github.com/arirubinstein)
- [Carlos Enamorado](https://github.com/fath3rl0s)


### Latest news

- Falco 0.41.2 released!

### Lightning Talk

- Status update about the syscall exit events extension initiative supporting the syscall enter events drop initiative
- Resources:
    - [new(proposal): disable support for syscall enter events](https://github.com/falcosecurity/libs/pull/2068)
    - [[Tracking] Extend syscall exit events with syscall enter events parameters](https://github.com/falcosecurity/libs/issues/2427)
    - [FR: Configuration flag support to disable enter event generation](https://github.com/falcosecurity/libs/issues/2408)
    - [FR: TOCTOU mitigation without userspace enter events](https://github.com/falcosecurity/libs/issues/2407)


## 2025-06-04

### MC

- 

### Who joined

- [Your Name](https://github.com/your-handle)


### Latest news

- This community call is cancelled. Sorry for the short notice. See you in two weeks!

### Lightning Talk

-
