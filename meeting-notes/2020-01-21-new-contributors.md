# Falco New Contributor Onboarding Call

### Attendees 

 - Kris Nova - Sysdig @krisnova @nova (Interested in C/C++/Go/Build)
 - Leonardo Di Donato - Falco maintainer - @leodido (github/twitter) (C/C++/Go/Rust)
 - Lorenzo Fontana - Falco maintainer - @fntlnz ()
 - Zachary Estrella - Veracode - @rephric/@zestrells (github/twitter) (Interested in Go/Build/Infrastructure)
 - Tamjid Ahmed - Toptal - @DeshErBojhaa (github + twitter) (interested and experienced in Go and anything that uses Go)
 - Brian Wagner - Mediacurrent github/briwagner (Go)
 - Peter Matseykanets @pmatseykanets (Interested in Go/Build/CI)
 - Amit Shirodkar - IBM - @shirodkara(github) (Interested in port to Linux on ppc64le)
 - Logan Davis - @brainsnail (github/twitter) - Interested in Go and better understanding container security 
 - Holden Karau @holdenkarau mostly Python interest some C fun
 - Nitya Dhanushkodi - VMWare @ndhanushkodi (github) (Interested in Go/eBPF/C++)
 - Shubhendu Poothia - Independent @poothia(github) (Interested in Go/eBPF)
 - Ayush Priya - Appsecco - @ayushpriya10 @Ayush (https://ayushpriya.tech)(Knows Python, Interested in learning Go)
 - Bhaarat Sharma - Raft (https://goraft.tech/) , @bhaaratcrckt, Interested in Container Runtime Security (C++,Go,Scala)
 - Barak Stout - Raft (https://gorafth.tech/), @barakstout (github) Container Security and open-source contributions 
 - Patrick Asata - Raft (https://goraft.tech/) , @PatrickGoRaft(twitter), Interested in Container Runtime Security(Go,Scala)
 - Raj Krishnamurthy - ContiNube - @rajkrishnamurthy - Go. New to Falco. Interested in Rules.
 - Pierre Lacerte - @palacerte (Interested in the build system, Golang, grpc, learning about bpf)
 - Yusuf Kanchwala - Red Hat github: kanchwala-yusuf (Know Go, Python well, Interested in C/C++ stuff as well)
 - Vikash - OC - @Vikash082 (intereste in container security, go, build, c++)
 - Akhil Thampy @athampy C++,Go,eBPF   
 - Sunil Botre - IBM - @sunil1783(interested in C++, porting falco with eBPF on ppc64le platfrom)
 - Bharath Thiruveedula Independent @bharaththiruveedula(Github) (Interested in Go/eBPF)
 - Dan Stough, Product Owner at Keysight Technologies Twitter-@DevStough Github-DanStough; C++, Go, Build and Docs
 - Teea Alarto - teeaa @ github, teeatime @ twitter - Intermediate with Go, want to start contributing to open source stuffs
 - Joshua L. -ClevelandJosh @ github, novice contributor, used to write up filter sets for open hids, would lile to map some of that to rule/module sets, if that aligns.
 - Bala - balasu@github , Bala35542522@Twitter,part of docker community Bangalore(interested in container security,Linux,infrastructure)
 - Melina B - olivebay/olivebay (github/slack) (Interested in Go(Beginner), build, grpc, CI, learning bpf) 
 - Arjun - Twitter @arjunsahasranam Pramati Technologies 
familiar with Golang and eBPF.
 - Chandrika - Worked with C/C++, also familiar with Go. chandrikamutalik@GitHub
 - Natch Ruengsakulrach @natchaphon-r Interested in eBPF
 - Frederick Kautz - NSM Maintainer - (gh: fkautz, tw: ffkiv) - Looking to contribute around grpc APIs and networking observability.
 - Girish Kumar - @zkmrgirish(github/twitter) - (Intermidiate with go, interested in falcoctl, falcosidekick)
 - Deepak - @deepakprasanna(github), Interested in build


### Action 
 
 - [Nova] Understanding the main areas of the project folks are interested in working on
     - Prometheus (3rd party projects)
     - Build
         - Kris Nova - Will start an OSS call focused specifically on the build
             - We need to do a demo of our current infrastructure to capture the state of the world 
         - Pierre Lacerte
         - Deepak
         - CNCF CI access - request (accepted) [here](https://github.com/cncf/cluster/issues/123)
         - We have access (Leo) to the CNCF infrastructure, we just need a plan (see issue above)
         - Release process in the open
             - Mechanism to store the kernel probes
             - Documenting the release process
             - Currently focusing on 0.19
         - eBPF
             - Kris Nova
             - Leo Di Donato
         - Engine (C/C++)
             - Kris Nova
             - Leo Di Donato
    - Go tools
        - https://github.com/falcosecurity/falcoctl
        - https://github.com/falcosecurity/client-go
        - https://github.com/falcosecurity/falcosidekick
    - [Cloud Native Security Hub](https://securityhub.dev)
        - [Repository](https://github.com/falcosecurity/cloud-native-security-hub)
 - [Nova] Context for Wed calls 
     - MC for each call
     - Notes for each call
 - [Nova] Good first Issues
     - Kris Nova adding good first issues as we groom 1.0.0 
     - Kris Nova add first issues to [falcoctl](https://github.com/falcosecurity/falcoctl)
     - Add goals/direction to falcoctl 
     - Falcoctl is tightly coupled with the new gRPC APIs
 - [Nova] Schedule a build call
 - [Nova] Homework! 
     - Take falco for a test drive, and document any rough areas
     - If you need resources feel free to message Nova/Falco Maintainers
     - 
 - [Holden] Good people to ping on first PRs for review?
     - Bot makes suggestions try them first, otherwise try Leo, Lorenzo, or Kris and try them
 - [Yusuf] Loki? (3rd party project) similar to Prometheus for log aggregation https://github.com/grafana/loki
    - [Falco sidekick](https://github.com/falcosecurity/falcosidekick) has it
 - [Nova] Add issues to falco sidekick about adopting the output API
 - [Pierre] Roadmap for Falco vs Sysdig Secure
 - Link to contributors call
     

  ### Wednesday Calls
  
  Links, zoom, cal => 
  https://github.com/falcosecurity/community
  
  # Closing
  
  A [closing note was sent by Kris Nova to the mailing list](https://lists.cncf.io/g/cncf-falco-dev/topic/update_from_new_contributor/69964948) to summarize the call.
  The [recording can be found here](https://www.youtube.com/watch?v=ueBRvu_SR0k).

