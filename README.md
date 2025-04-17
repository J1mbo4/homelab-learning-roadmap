
[Homelab_Learning_Roadmap.md](https://github.com/user-attachments/files/19797577/Homelab_Learning_Roadmap.md)

# Homelab Learning Roadmap Checklist
*From beginner to wizard*

## LEVEL 0: Foundation
**Goal:** Get familiar with Raspberry Pi and running containers
- [x] Set up Raspberry Pi OS
- [x] Install Docker
- [x] Install Portainer
- [x] Deploy containers (Pi-hole, Grafana, Homarr, etc.) using guides
- [ ] Use basic Docker commands: `docker ps`, `docker logs`, `docker exec`
- [ ] Restart a container manually (`docker restart <name>`)
- [ ] Explore Portainer and what it's doing behind the scenes

## LEVEL 1: Networking Basics
**Goal:** Understand core networking concepts used in homelabs
- [ ] Understand IP addresses & subnets (e.g., 192.168.x.x/24)
- [ ] Learn how DNS works (e.g., Pi-hole logs, hostnames)
- [ ] Learn what DHCP is and who provides it (check your router)
- [ ] Understand what ports are (e.g., 80 for web, 53 for DNS)
- [ ] Explore NAT and how port forwarding works
- [ ] Learn what firewalls do and basic rules
- [ ] Understand what VLANs are (conceptual only for now)
- [ ] Use `ip a` or `ifconfig` to see your IPs and interfaces
- [ ] Log into your router and explore DHCP & IP reservations

## LEVEL 2: Build a Safe Playground Network
**Goal:** Set up a VLAN-friendly lab that doesn’t interfere with family internet
- [ ] Get a VLAN-aware router or flash one with OpenWRT/pfSense/OPNsense
- [ ] Connect new router to ISP modem using double NAT
- [ ] Create an isolated LAN/VLAN for your lab devices
- [ ] Move Raspberry Pi and laptop into the isolated lab VLAN
- [ ] Write basic firewall rules (e.g., block all outbound except updates)
- [ ] Break stuff, reboot stuff, learn — safely!

## LEVEL 3: Level Up Containers
**Goal:** Go deeper into Docker and container orchestration
- [ ] Learn Docker Compose
- [ ] Convert your Pi-hole container to a Compose file
- [ ] Learn about Docker volumes and bind mounts
- [ ] Explore Docker networks (bridge, host, custom)
- [ ] Use environment variables in your Compose files
- [ ] Install and test Watchtower for auto-updates
- [ ] Set up NGINX Proxy Manager or Traefik to access apps via subdomains

## LEVEL 4: Monitoring & Observability
**Goal:** See and understand what's happening in your lab
- [ ] Set up Uptime Kuma to monitor services
- [ ] Create a Grafana dashboard (use Pi-hole as a data source)
- [ ] Learn Prometheus basics (scraping metrics)
- [ ] Add simple alerts (e.g., service offline, disk usage high)
- [ ] Explore centralized logging with Loki or similar

## LEVEL 5: Automation & Configuration
**Goal:** Automate installs, configs, and system states
- [ ] Learn Ansible basics: inventory + playbook
- [ ] Write a playbook to install Docker + deploy Pi-hole
- [ ] Write bash scripts to monitor/restart containers
- [ ] Use cron jobs for automation (e.g., backups, reports)
- [ ] Learn Git basics (init, commit, push, pull)
- [ ] Start tracking your dotfiles and config files in Git

## LEVEL 6 (Bonus): GitHub Portfolio
**Goal:** Document your progress and show off your skills
- [ ] Create a GitHub profile README
- [ ] Create a public repo for each project
- [ ] Write markdown READMEs with:
  - [ ] Project overview
  - [ ] Setup instructions
  - [ ] Problems encountered / lessons learned
- [ ] Share screenshots and diagrams
- [ ] (Optional) Set up GitHub Pages as a personal portfolio site
