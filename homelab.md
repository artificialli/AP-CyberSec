## October

* Staging build: software installation, configuration, and patching
Metrics tracked: use-case scenarios, safety notification protocols

- [ ] establish tailscale vpn for globall rdp (secure remote administration)
- [ ] Grafana
- [ ] Prometheus
- [ ] OT VLAN behind OPNsense
- [x] download kali linux software on local server
- [ ] custom kali linux distro search
- [ ] jellyfish custom ipv4 settings
- [ ] configure jellyseer, sonarr, lidarr, radarr, prowlarr
- [ ] arrange custom pull settings via jellyseer
- [ ] observe automated pull for accuracy
- [ ] tune retention settings and ot device delivery
- [ ] navadrone music app for music
- [ ] cloudflare for custom dns + ad blocking
- [ ] jelly bridge


## September 2026

* Monitoring Staging build: performance and hardware health
Metrics tracked: bandwidth, latency, false alarm rate, hardware temperatures

#### Incident 1: CPU overheating
- **Symptom:** CPU running at 60°C idle / 95°C under load, detected via AMD Ryzen Master.
- **Root cause:** AIO cooler failure (degraded thermal paste between the CPU and AIO cold plate, reducing heat transfer), causing sustained overheating.
- **Remediation:** Removed the AIO and CPU, applied fresh thermal paste, reinstalled both, and cleaned the cooler fans.
- **Follow-up:** Installed L-Connect 3 to manage fan RPM.
- **Result:** Temps now 35°C idle / 62°C load. Verified over 15 days.
- **Prevention:** Set an alert at 80°C in HWiNFO, the overheating threshold for my CPU.
- **Lesson learned:** Monitoring in staging caught a failing cooling component before production, where it could have caused system failure. Baselining temperatures and setting alerts are what make that early detection possible.
#### Incident 2: OT device failure
- **Symptom:** Camera observed offline on multiple occasions, high latency for live-monitoring observed via running ping. 
- **Root cause:** Network packet loss from suspected wireless interference and network congestion.
- **Remediation:** documentation in progress
- **Follow-up:** documentation in progress
- **Result:** Device remains online, lower latency and ping observed.
- **Prevention:** documentation in progress
- **Lesson learned:** documentation in progress
  

## August 2026

* Staging build: software installation and configuration
Metrics tracked: use-case scenarios, application processes, dependencies for progress

- [x] Home Assistant installation 
- [x] VirtualBox installation
- [x] connect iot devices such as smart lights, robot vacuum, pet feeder
- [x] custom ipv4 settings
- [sourcing] connect garage opener, home thermostat (electrician needed)
- [x] build out automations
- [sourcing] install motion sensors for inputs, heat sensors for interior monitoring
- [x] docker desktop


## Sources
* [reddit](https://www.reddit.com/r/sonarr/comments/17v6q01/making_sure_i_understand_what_sonarr_does/)
* [trashGuides](https://trash-guides.info/)
* [trueNAS](https://forums.truenas.com/t/help-sonarr-radarr-sabnzb-jellyfin-install-driving-me-crazy/58585)
* 


