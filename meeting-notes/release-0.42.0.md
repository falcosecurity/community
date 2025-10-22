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
