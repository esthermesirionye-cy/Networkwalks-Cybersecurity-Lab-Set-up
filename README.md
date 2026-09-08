 NETWORKWALKS-WK1-CYBERSECURITY-LAB

---

## 📌 Project Information

### Overview

This repository covers my Week 1 setup for the Networkwalks Cybersecurity Internship. The main goal was to build a secure virtual lab on my laptop using *Oracle VirtualBox* and *Kali Linux* so I have a dedicated environment for future testing and practice.

---

### 🎯 Objectives

The main objectives of this project are to:

* Install and configure VirtualBox.
* Create a private *NAT Network* (10.0.0.0/24) for the cybersecurity lab.
* Install/import Kali Linux as a virtual machine.
* Configure network connectivity for Kali Linux using the NAT Network adapter.
* Assign a consistent IP address to the Kali VM (10.0.0.2/24).
* Enable shared clipboard, drag-and-drop, and host /downloads folder sharing.
* Verify network connectivity and DNS resolution.
* Take a clean VM snapshot for recovery.
* Document the complete setup process.
* Prepare the environment for future cybersecurity projects.

---

### 📋 Purpose of the Lab

The lab provides an isolated environment to execute security testing, traffic monitoring, and ethical hacking exercises safely without impacting the host machine or external production networks.

---

### ⚙️ Implementation Steps

#### 1. VirtualBox Installation

* Downloaded and installed the latest binary release of Oracle VirtualBox on Windows.
* Configured core global hypervisor settings.

![VirtualBox Installation](Screenshot%202026-09-08%20033850.png)

  
#### 2. NAT Network Configuration (10.0.0.0/24)

* Created a private *NAT Network* profile inside VirtualBox before launching the VM.
* Scoped the network subnet to 10.0.0.0/24.

#### 3. Kali Linux Setup

* Extracted the downloaded Kali Linux image file using local extraction tools (Winamp).
* Imported Kali Linux into VirtualBox and configured the RAM.
* Attached Adapter 1 directly to the newly created *NAT Network*.
* Configured guest integration setting * *Shared Folder:
* * Mapped the host /downloads folder to Kali Linux.
* Booted Kali Linux and set the static IP address to 10.0.0.2/24.

![Kali Linux Setup](Screenshot%202026-09-08%20033928.png)

#### 4. Testing & VM Snapshot

* Ran ping commands inside the Kali Linux terminal to confirm internet access and DNS resolution.
* Created a clean *VM Snapshot* to easily restore the base state at any time.

![Testing & VM Snapshot](./Screenshot 2026-09-08 020034004.png)

---

### 🚨 Challenges Faced & Solutions

* *Downloaded Extension Pack Instead of Main File:*
* Challenge: Initially downloaded the VirtualBox Extension Pack file instead of the base VirtualBox installer for Windows.
* Solution: Re-reviewed the Networkwalks tutorial recording, identified the correct executable, and installed the main VirtualBox application.


* *Order of Network Setup:*
* Challenge: Ensuring the network subnet was created before launching Kali Linux.
* Solution: Configured the NAT Network (10.0.0.0/24) in VirtualBox preferences prior to starting up and mapping the Kali VM adapter.


* *Large File Extraction Time:*
* Challenge: Extracting the Kali Linux virtual disk archive took considerable processing time.
* Solution: Allowed the extraction process to complete fully before importing the image into VirtualBox.


---

### ✅ Verification Summary

* *NAT Network:* Configured to 10.0.0.0/24.
* *Kali IP Address:* Set to 10.0.0.2/24.
* *Connectivity:* Outbound internet and DNS verified.
* *Snapshot:* Baseline VM snapshot saved.

---

## 🛠️ Tools & Resources

* *7-Zip:* [https://7-zip.org/download.html](https://7-zip.org/download.html)
* *VirtualBox:* [https://virtualbox.org/wiki/Downloads](https://virtualbox.org/wiki/Downloads)
* *Kali Linux:* [https://kali.org/get-kali](https://www.google.com/search?q=https://kali.org/get-kali)
* *Networkwalks Academy:* [https://networkwalks.com](https://networkwalks.com)

---

## 👤 Author

Esther Mesirionye

Networkwalks Cybersecurity Intern

LinkedIn: [https://www.linkedin.com/in/esthermesirionye/](https://www.google.com/search?q=https://www.linkedin.com/in/esthermesirionye/)
