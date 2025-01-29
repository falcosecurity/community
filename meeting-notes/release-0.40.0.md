# Falco Community Call (bi-weekly)

Welcome! We’re excited to have you here. Before we get started, please note:

1. **CNCF Code of Conduct:** Let’s keep this space welcoming by treating each other respectfully and kindly.  
2. **Recording Notice:** This call is recorded and may be shared publicly. Please turn off your camera or microphone if you prefer not to be seen or heard.  
3. **Attendee List:** Please add your name under the **_Who Joined_** section below so we know you stopped by!

Thank you for joining us and contributing to the Falco community!

[More Information](https://github.com/falcosecurity/community) - [Zoom Link](https://zoom.us/my/cncffalcoproject) - [Recordings](https://youtube.com/playlist?list=PLgVVUpW8NIJAaZtszf1_nxB2y6mQrlY4s)

## 2025-01-22

### MC

- [Thomas Labarussias](https://github.com/Issif)

### Who joined

- [Mauro Moltrasio](https://github.com/Molter73)
- [Angelo Puglisi](https://github.com/deepskyblue86)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Andrea Terzolo](https://github.com/Andreagit97))
- [Aldo Lacuku](https://github.com/alacuku)

### Latest news

- New playlist on YT for the past Communty Calls (2025): https://www.youtube.com/playlist?list=PLgVVUpW8NIJCZrAvytqtsMMC9_OqYERMk
- New plugin for the `K8s Audit logs` (source `k8s_audit`) from the managed K8s at OVH (French Hosting Provider): https://github.com/falcosecurity/plugins/pull/554 thanks to Aurelie Vache
- Stratoshark is out: https://stratoshark.org/
- Maintainers are finalizing Falco 0.40, expected to be released by the end of Jan. Issue to follow: https://github.com/falcosecurity/falco/issues/3456

### Lightning Talk

- **Syscall captures in Talon (live demo)** by Thomas

### Agenda / Open Discussion

## 2025-01-15

### MC

- [leogr](https://github.com/leogr)

### Who joined

- [fededp](https://github.com/fededp)
- [ekoops](https://github.com/ekoops)
- [alacuku](https://github.com/alacuku)
- [LucaGuerra](https://github.com/LucaGuerra)

### Latest news

- From now, the community call will be bi-weekly (i.e. every 2 weeks)!
- [falco-exporter](https://github.com/falcosecurity/evolution/issues/420) entered in deprecation mode in favor of [Falco built-in metrics](https://falco.org/docs/metrics/falco-metrics/): [dashboard on test-infra](https://monitoring.prow.falco.org/dashboards/f/ae4q6q75v1h4wc/)
- Recently adopted sub-projects:
    - https://github.com/falcosecurity/falco-actions
    - https://github.com/falcosecurity/plugin-sdk-rs
- Maintainers are finalizing Falco 0.40, expected to be released by the end of Jan

### Lightning Talk

- **Upcoming Release Sneak Peek (Falco 0.40)** by leogr
    - https://docs.google.com/presentation/d/1oPzExYYHh3q1r9Vq4_ENgRPWGYx03OSraHzz6-zAvvE/edit#slide=id.p

### Agenda / Open Discussion

- [thomas] DevRel activities
    - work more on the website
    - increase FAQs and move them to a different section, and make them searchable
    - [leogr] this alings to the ongoing restructuring https://github.com/falcosecurity/falco-website/issues/1365
    - Feed the FAQ using slack questions
- [luca] KB on stackoverflow?
    - we need a place for questions with specific answers



## 2024 Holidays notice

**NOTE**
**Community Calls will pause for the holidays, The next call is on January 15, 2025.**


## 2024-12-11

### MC

- 

### Who joined

- [leogr](https://github.com/leogr)
- [molter73](https://github.com/molter73)

### Weekly highlights

- [Falcosidekick 2.30](https://falco.org/blog/falcosidekick-2-30-0/) is out
- [Falco Talon 0.2.1](https://github.com/falcosecurity/falco-talon/releases/tag/v0.2.1) is out, this is a bug fix release (fix missing prom metrics)


### Agenda

- Community Calls will pause for the holidays starting next week
    - The next call is on January 15, 2025.
- WIP for the Grafana dashboards (for Prometheus metrics) for falco, falcosidekick and talon, reviews are welcome


## 2024-12-04

### MC

- [Thomas Labarussias](https://github.com/Issif)

### Who joined

- [Mauro Moltrasio](https://github.com/Molter73)
- [Aldo Lacuku](https://github.com/alacuku)
- [Thomas Labarussias](https://github.com/Issif)
- [Leonardo Di Giovanna](https://github.com/ekoops)

### Weekly highlights

### Agenda

* No topic, call cancelled

## 2024-11-27

### MC

[Federico Di Pierro](https://github.com/FedeDP)

### Who joined
- [Federico Di Pierro](https://github.com/FedeDP)
- [Roberto Scolaro](https://github.com/therealbobo)
- [Leonardo Di Giovanna](https://github.com/ekoops)
- [Mauro Moltrasio](https://github.com/Molter73)
- [Luca Guerra](https://github.com/LucaGuerra)
- [Aldo Lacuku](https://github.com/alacuku)
- [Thomas Labarussias](https://github.com/Issif)

### Weekly highlights
* Libs 0.18.2: https://github.com/falcosecurity/libs/releases/tag/0.18.2
    * 2 modern ebpf fixes
* Libs 0.19.0: https://github.com/falcosecurity/libs/releases/tag/0.19.0
* Falco 0.39.2: https://github.com/falcosecurity/falco/releases/tag/0.39.2
    * libs 0.18.2 + small falcoctl fix (patch release v0.10.1)
* Falco talon 0.2 :rocket: https://github.com/falcosecurity/falco-talon/releases/tag/v0.2.0
    * integration with google cloud, export to google storage

### Agenda

* Drop elfutils libelf in libs and switch to https://sourceforge.net/p/elftoolchain/wiki/Home/
    * [LucaG] I have a prototype branch, will port it upstream for review



