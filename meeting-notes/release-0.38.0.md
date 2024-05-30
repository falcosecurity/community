# Falco Community Call

[More Information](https://github.com/falcosecurity/community)
[Zoom Link](https://zoom.us/my/cncffalcoproject)
[Recording](https://youtube.com/playlist?list=PLgVVUpW8NIJAaZtszf1_nxB2y6mQrlY4s)


## 2024-05-29

### MC

- Federico Di Pierro ([fededp](https://github.com/fededp))

### Who joined

- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))


### Weekly highlights

- libs 0.17.1
    - https://github.com/falcosecurity/libs/releases/tag/0.17.1
- Falco 0.38.0 shaping up good
    - https://github.com/falcosecurity/falco/issues/3197

### Agenda

## 2024-05-22

### MC

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))

### Who joined

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Fred Araujo ([araujof](https://github.com/araujof))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))

### Weekly highlights

- Libs release 0.17.0
          - Improvements to filterchecks, now we support rhs "proc.name != val(proc.pname)"
          - possible fix for modern ebpf page fault https://github.com/falcosecurity/falco/issues/3181
          - https://github.com/falcosecurity/libs/pull/1857
      - Target date for 0.17.0 and drivers 7.2.0+driver May 23rd (https://github.com/falcosecurity/libs/commit/d67ff09199687d93b2fb2d45ae234dedf56212b0)
          - PPC64LE fixes
- Falco 0.38.0

### Agenda

## 2024-05-15

### MC

- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))

### Who joined

- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Fred Araujo ([araujof](https://github.com/araujof))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))

### Weekly highlights

### Agenda

- Falco 0.38.0 https://github.com/falcosecurity/falco/issues/3197
  - [lg] proposing myself as a release manager
      - call for release team (contact me)
      - libs 0.17.0
          - Improvements to filterchecks, now we support rhs "proc.name != val(proc.pname)"
          - possible fix for modern ebpf page fault https://github.com/falcosecurity/falco/issues/3181
          - https://github.com/falcosecurity/libs/pull/1857
      - Target date for 0.17.0 and drivers 7.2.0+driver May 23rd (https://github.com/falcosecurity/libs/commit/d67ff09199687d93b2fb2d45ae234dedf56212b0)
          - PPC64LE fixes
  - Driver loader logic and integration

- libs CI musl tests: https://github.com/falcosecurity/libs/blob/master/.github/workflows/ci.yml#L63

## 2024-05-08

### MC

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))

### Who joined

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Fred Araujo ([araujof](https://github.com/araujof))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Leonardo Grasso ([leogr](https://github.com/leogr))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))

### Weekly highlights

- we released libs 0.16.0
    - https://github.com/falcosecurity/libs/releases/tag/0.16.0
    - https://github.com/falcosecurity/libs/releases/tag/7.1.0%2Bdriver
- Falco release 0.38.0 soon
    - libs release 0.17.0
        - filtercheck support on expression rhs
            - "proc.name != val(proc.pname)"
            - https://github.com/falcosecurity/libs/issues/1789
- Plugin integration with Kafka
    - https://github.com/falcosecurity/plugins

### Agenda


## 2024-04-24

### MC


### Who joined

- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Thomas Labarussias ([Issif](https://github.com/Issif))

### Weekly highlights

- libs release 0.16.0 -> in progress, some bugs
    - libs 0.16.0-rc1 is out but we have some issues that we are fixing
    - https://github.com/falcosecurity/libs/pull/1813
    - https://github.com/falcosecurity/libs/pull/1812
    - https://github.com/falcosecurity/libs/pull/1811
- filtercheck support on expression rhs for Falco 0.38.0
    - https://github.com/falcosecurity/libs/issues/1789

### Agenda

- [Teryl] Is it possible to use falcoctl to load drivers in projects that are not Falco?
    - We never did but it is a possibility. falcoctl active owners (Fede, Aldo) might share some insights
- [Teryl] We may have located another issue with users
    - Please let us know / open an issue once you find a way to reproduce or any hints

## 2024-04-17

### MC

- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))

### Who joined

- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- GLVS Kiriti ([GLVS Kiriti](https://github.com/GLVSKiriti))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Kapil Sharma ([h4l0gen](https://github.com/h4l0gen))

### Weekly highlights

- libs release 0.16.0 -> early next week
    - container runtime improvements
    - performance fixes
    - filtercheck support on expression rhs
        - "proc.name != val(proc.pname)"
        - https://github.com/falcosecurity/libs/issues/1789
    - testing with Falco

### Agenda

- Work to include Prometheus Metrics
    - https://github.com/falcosecurity/falco/issues/1772
    - https://github.com/falcosecurity/falco/pull/3140

## 2024-04-10

### MC

- Federico Di Pierro ([fededp](https://github.com/fededp))


### Who joined

- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- Thomas Labarussias ([Issif](https://github.com/Issif))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Kapil Sharma ([h4l0gen](https://github.com/h4l0gen))

### Weekly highlights

- Falco split configuration file: https://github.com/falcosecurity/falco/pull/3024
- Chisels deprecation / cleanup PR is up :https://github.com/falcosecurity/libs/pull/1785

### Agenda

- **Remember: libs 0.16.0 scheduled to be released on 19th April** (with a driver tag too!)

## 2024-04-03


### MC

- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))

### Who joined

- Federico Di Pierro ([fededp](https://github.com/fededp))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Thomas Labarussias ([Issif](https://github.com/Issif))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))

### Weekly highlights

- 

### Agenda

- [Roberto Scolaro]: removing the chisels from libs proposal
    - https://github.com/falcosecurity/libs/issues/1743

## 2024-03-27

### MC

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))

### Who joined

- Aldo Lacuku ([alacuku](https://github.com/alacuku))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Thomas Labarussias ([Issif](https://github.com/Issif))
- Teryl Taylor ([terylt](https://github.com/terylt))
- GLVS Kiriti ([GLVS Kiriti](https://github.com/GLVSKiriti))
- Fred Araujo ([araujof](https://github.com/araujof))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- Kapil Sharma 
([h

4l0gen](https://github.com/h4l0gen))

### Weekly highlights

- 

### Agenda

- [Aldo Lacuku]: I would like to propose myself as maintainer for charts and falcoctl
- [Thomas (no mic)] AUR packages: falco/falcoctl/driverkit are up to date in AUR repo, falcosidekick is now available too:
    - https://aur.archlinux.org/packages/falco-bin
    - https://aur.archlinux.org/packages/falcoctl
    - https://aur.archlinux.org/packages/driverkit
    - https://aur.archlinux.org/packages/falcosidekick
- 

## 2024-03-13

### MC

- Thomas Labarussias ([Issif](https://github.com/Issif))


### Who joined

- Samuel Gaist ([SGaist](https://github.com/sgaist))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- Luca Guerra ([LucaGuerra](https://github.com/LucaGuerra))
- Aldo Lacuku([alacuku](https://github.com/alacuku))
- Mike Coleman([mikegcoleman](https://github.com/mikegcoleman))
- Teryl Taylor ([terylt](https://github.com/terylt))

### Weekly highlights

- No Community call next week: See you at Kubecon
 
### Agenda

- [Samuel] Documentation (developer wise) improvement
    - [Samuel] to open a long-standing issue for areas of improvement

## 2024-03-06

### MC

- Federico Di Pierro

### Who joined

- Federico Di Pierro ([fededp](https://github.com/fededp))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- Samuel Gaist ([sgaist](https://github.com/sgaist))
- Mike Coleman ([mikegcoleman](https://github.cmo/mikegcoleman))
- Teryl Taylor ([terylt](https://github.com/terylt))
- Aldo Lacuku([alacuku](https://github.com/alacuku))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Thomas Labarussias ([Issif](https://github.com/Issif))

### Weekly highlights

- **Falco graduated in the CNCF** -> https://falco.org/blog/falco-graduation/

### Agenda

- 

## 2024-02-28

### MC

- Federico Di Pierro

### Who joined

- Thomas Labarussias ([Issif](https://github.com/Issif))
- Federico Di Pierro ([fededp](https://github.com/fededp))
- Mike Coleman ([mikegcoleman](https://github.cmo/mikegcoleman))
- Vicente J. Jiménez Miras ([vjjmiras](https://github.com/vjjmiras))
- Roberto Scolaro ([therealbobo](https://github.com/therealbobo))
- Luca Guerra([LucaGuerra](https://github.com/LucaGuerra))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))
- Fawziyah Nabeelah ([ftnabeelah])(https://github.com/vmfarms/falco-root-container-notification)

### Weekly highlights

- 

### Agenda

- [Thomas] New shareable links to rules in falco.org. try it: https://falco.org/docs/reference/rules/default-rules/#Write_below_etc
- [Thomas] Switch to the scarf gateway has been done 10d ago, no glitch since. We now collect anonymous metrics about the downloads of packages/drivers by os/kernel/arch/versions/...

## 2024-02-21

### MC

- Thomas Labarussias ([Issif](https://githb.com/Issif))

### Who joined

- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Aldo Lacuku([alacuku](https://github.com/alacuku))
- Teryl Taylor ([terylt](https://github.com/terylt))

### Weekly highlights

- 

### Agenda

- No topic

## 2024-02-14

### MC

- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))

### Who joined

- Teryl Taylor ([terylt](https://github.com/terylt))
- Mauro Moltrasio ([Molter73](https://github.com/Molter73))
- Thomas Labarussias ([Issif](https://githb.com/Issif))
- Andrea Terzolo ([Andreagit97](https://github.com/Andreagit97))

### Weekly highlights

- Falco 0.37.1 is out
    - https://falco.org/blog/falco-0-37-1/

### Agenda
