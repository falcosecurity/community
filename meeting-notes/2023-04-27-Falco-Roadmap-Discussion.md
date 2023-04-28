# 2023-04-27 Falco Roadmap Discussion

Refs:
    - [Proposal](https://github.com/falcosecurity/evolution/issues/259#issuecomment-1480040846)

## Who joined

- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Jason Dellaluce ([@jasondellaluce](https://github.com/jasondellaluce))
- Thomas Labarussias ([@Issif](https://github.com/Issif))
- Mauro Moltrasio ([@molter73](https://github.com/Molter73)
- Massimiliano Giovagnoli ([@maxgio92](https://github.com/maxgio92))
- Melissa Kilby ([@incertum](https://github.com/incertum))
- Andrea
- Mark
- Gregz

## Agenda

- [leogr] Managing development cycles
    - Proposal: splitting Falco's release cycle
      - 8 weeks of development, 4 weeks of stabilization, 4 weeks of release prep 
    - Release dates of dependencies should be reverse-engineered from the main roadmap
        - For example, a libs release (or pre-release) should happen during each development iteration
   - Release preparation
       - [same as libs](https://github.com/falcosecurity/libs/blob/master/release.md#release-phases)
       - We will have release branches in libs (following up Mark's question)
   - Defining priorities for next release at the beginning (before) the dev phase
        - Urgent fixes can come anytime
        - New features will likely not be merged outside of the dev phase, but will require case-by-case discussion among maintainers going with lazy consensus
- [leogr] Regular maintainers meetings
    - Monthly meeting (around the first week of each month)
    - We can skip Mar, Jul, Nov (so just 9 meetings per year)
    - [andrea] We need to have an agenda prepared before the meeting to make sure time is not wasted, and we should have a private or public channel to have preliminary discussions among maintainers
- [leogr] Testing release or pre-release
    - [andrea] not sure if we want a real release
    - let's experiment 
- [leogr] Using GitHub Projects
    - https://github.com/orgs/falcosecurity/projects/5/views/7
    - [thomas/leogr] add more labels
        - high level goal
        - performances
        - blockers
        - improvement vs. feature
    - [jason] not add PRs, just issues
- [leogr] Would we kick-off a Project management WG?
    - balance tecnical people and non-techical people
- [incertum] Discuss Top Priorities / High Level Features
    - 5 top features to carry on across releases
        - Performance
        - Stability
        - Documentation
        - Usability
    - Distinguish between features that push capabilities vs make Falco easier to use (balance both)
        - e.g. modern_bpf is a huge win to make Falco easier to use
        - another good example is gVisor or arm64 support ensuring we continue having visibility into systems
        - on the other hand `exe_upper_layer` really made a difference in terms of better detections that scale
    - 2 examples for improved capabilities to catch bad stuff
        - Better, stronger and more trustworthy kernel signals, e.g LSM hooks, symlink resolution, other bypasses
        - Anomaly detection
- [incertum] Discuss Procedures to "move faster while improving stability"
    - try anticipating issues as per new roadmap planning
    - define testing and QA procedures
    - need more people and maintainers
    - criteria for rules? -> discuss
    - criteria for everything
        - another good task for the WG
- where to discuss feature proposal?
    - slack
    - gh issues
    - gh discussion
    - WG should solve this


## Action items

- [ ] [leogr] finish to write the proposal
- [ ] [leogr] Schedule a monthly meeting
    - same time, same day of the week
- [ ] [leogr] working group
    - [ ] [andrea] communication channel for proposal
- [ ] [melissa] criteria maker!
- [ ] [thomas] help with GH project and labels

Things to add to the roadmap:
    - process documentation

## Closing

- Do we agree on trying the new process starting with Falco 0.36 development cycle?
    - all agree!!!
