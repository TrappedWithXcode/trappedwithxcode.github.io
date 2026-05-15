---
layout: home
title: Attic Admin - The HomeLab Journey
---

> This GitHub page serves as a guide, tutorial, and documentation hub for my homelab setup. Welcome to the journey!

# Introduction: A New Home

The whole idea was born when I found my new home—a small, multi-story flat with its own garden. There was nothing inherently crazy about it, but the unique layout sparked a thought: **I should make it smart.**

What started as a simple plan for smart lighting, smart locks, and cameras quickly snowballed. From basic smart home tech, I went straight down the rabbit hole. Now, I’m basically building out a small hosting company (that's a joke, in case humor wasn't on the menu today). 

Here are the main concepts you can find and struggle through together with me during this journey:

*   **Kubernetes (k3s):** Clusters for automated orchestration. Deep dives into containerization and clusterization.
*   **Proxmox VE:** For bulletproof virtualization. Because why should I leave my work at the office?
*   **Mac Mini:** Pulling duty as a high-efficiency media and AI server.
*   **NAS:** Storage holding a massive library of *legally* obtained movies and series oh, and also backups and stuff.
*   **Corporate-Worthy Networking:** Complete with multiple access points (because dropping to 300Mbps just because I walked into the next room is simply not an option).
*   **Home Assistant:** The open-source home automation platform that integrates with almost anything you throw at it.
*   **Ikea Smart Home Appliances:** Because why should I pay Philips Hue prices when Ikea gives me meatballs every time I visit?

# 📊 Current Cluster State

| Service / Node | Status | Role | Host Hardware |
| :--- | :--- | :--- | :--- |
| `k3s-master-node` | 🟢 Online | Control Plane | Raspberry PI 2GB RAM |
| `k3s-worker-node-1` | 🟢 Online | Worker (Apps) | Raspberry PI 8GB RAM |
| `pve`    | 🟢 Online | Hypervisor | Threadripper 2950x 64GB RAM |
| `mac-mini` | 🟢 Online | Jellyfin Server/ Ollama Server | Apple Macmini M4 16GB RAM |
| `nas-storage`   | 🟠 Bought/awaiting | NFS / Media | 9TB Array |
| `home-assistant`| 🟢 Online | Automation | Lenovo Mini PC|

*Last manually updated: May 2026*

# Table of Contents

Explore the different sections of my documentation hub:

*   📚 [**Tutorials**](/tutorials/) – Step-by-step guides on how I built things.
*   📋 [**Inventory**](/inventory/) – Hardware manifests, network maps, and currently running services.
*   🛠️ [**Templates**](/templates/) – My Kubernetes Manifest files, scripts, and configurations.
*   🧠 [**Opinions & Notes**](/opinions/) – My thoughts on self-hosting, architecture, and tech.

# Current Try Harding 

* [ ] Migrating a raw disk to Proxmox server and testing slow VM (This is work related Investiagetion)
* [ ] Make a HomeAssistant use a Ikea Button to dim lights or brighten a lamp
* [ ] Follow the Firewall zone matrix on actual Firewall device

# 📜 My Homelab Rules of Engagement

1.  **The "Wife/Partner Approval Factor" (WAF):** If the internet drops while I'm tweaking a VLAN, and the smart lights stop working, I have failed. Redundancy is mandatory.
2.  **No Cloud Allowed:** If a smart device requires an internet connection to talk to a server in Virginia just to turn on a lightbulb in my living room, it gets blocked at the firewall. 
3.  **Assume Breach:** Even though it’s a home network, everything is segmented. The IoT devices don't get to talk to the Kubernetes cluster, and the cluster doesn't get to talk to my personal laptop.

# 🧰 The Attic Stack

![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)
![Proxmox](https://img.shields.io/badge/Proxmox-E74C3C?style=for-the-badge&logo=Proxmox&logoColor=white)
![Home Assistant](https://img.shields.io/badge/homeassistant-%2341BDF5.svg?style=for-the-badge&logo=home-assistant&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Ollama](https://img.shields.io/badge/ollama-%23000000.svg?style=for-the-badge&logo=ollama&logoColor=white)
![Next Cloud](https://img.shields.io/badge/Next%20Cloud-0B94DE?style=for-the-badge&logo=nextcloud&logoColor=white)
![Ubiquiti](https://img.shields.io/badge/ubiquiti-%230559C9.svg?style=for-the-badge&logo=ubiquiti&logoColor=white)
![Apple](https://img.shields.io/badge/Apple-%23000000.svg?style=for-the-badge&logo=apple&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![nVIDIA](https://img.shields.io/badge/nVIDIA-%2376B900.svg?style=for-the-badge&logo=nVIDIA&logoColor=white)