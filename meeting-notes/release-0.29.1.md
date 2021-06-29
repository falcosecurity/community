## 2021-06-23

### MC
- Stefan Uygur

### Who joined
- Michele Zuccala ([@zuc](https://github.com/zuc))
- POP ([POP](https://github.com/danpopsd))
- Alejandro Villanueva ([@seishinsha](https://github.com/seishinsha/))
- [Cash Williams](https://github.com/cashwilliams)
- Batuhan Apaydın (https://github.com/developer-guy)
- Leonardo Grasso ([@leogr](https://github.com/leogr))
- Domenico Chirabino ([@chirabino](https://github.com/chirabino))
- Tom Kelley ([@distortedsignal](https://github.com/distortedsignal))
- Daniele Divito ([@danieledivito](https://github.com/danieledivito))
- Pablo Lopez ([@pabloopez](https://github.com/pabloopez))
- Stefan Uygur ([@ostendali](https://github.com/ostendali))
- Furkan Türkal (https://github.com/Dentrax/)
- Yankee Maharjan [yankeexe](https://github.com/yankeexe)
- Stefano Chierici [@darryk10](https://github.com/darryk10)
- Leonardo Di Donato [@leodido](https://github.com/leodido)

### This week highlights

- Falco 0.29.0 is out!
    - https://falco.org/blog/falco-0-29-0/

### Agenda
- [Stefan] Logging question about 0.28.x
        - https://github.com/falcosecurity/falco/issues/1673 (Action Item:Domenico to provide @leogr details in slack on troubleshooting/debugging)
- [Stefan] falco install script and rules
    -  installation script obsoleted, would like to maintain as it is very useful (https://falco.org/script/install)  (Action Item: @chirabnio to merge a PR with a proposed update)
    -  we would like to contribute to falco rules as it is generating lots of alerts, we want to refine them with scoring etc. (anyone working on this?) Stefano to post the proposal and we join that proposal. here you can fine the mailing list message regarding the proposal and how to join https://lists.cncf.io/g/cncf-falco-dev/message/256. [Contributing Rules guidelines (commit)](https://github.com/falcosecurity/.github/blob/master/CONTRIBUTING.md#rule-type)
    -  Falco CPU consumption (https://falco.org/blog/falco-performance-testing/)  
- [alejandro] MITRE ATT&CK matrix for containers (rule tags)
    - https://docs.google.com/spreadsheets/d/1lK2luf4iuOHDJEZ9EGcv3DkuuHeyRJAfeBzQCu2AuUI/edit#gid=0
    - All contributors welcome.  Action Item: @chirabino and Stefan and team to look into contribution
    - Tag naming standarization discussion?
        - Proposal: `mitre_ID_short_name`
- [developer-guy] falco-hot-reloader: A Proof Of Concept project about adding hot-reloading support to Falco using sidecar container concept in Kubernetes environment: [Github Repository](https://github.com/developer-guy/falco-hot-reload-with-sidecar)
- [leodido] Proposal: Versioning & Release process for falcosecurity/libs
    - https://github.com/falcosecurity/libs/pull/44
    - A lot to do: a very cool contribution to libs!
    - Feel free to contact me over Slack for making this together, or guidance

### Closing

- **MC Next Call**: 
