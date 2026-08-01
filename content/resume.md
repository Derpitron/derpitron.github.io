---
title: Resume
---
I’m an undergraduate Electronics and Computer Engineering student at Vellore Institute of Technology. I’m interested in all things programming, systems design, and building out the infrastructure to make cool things.
# Contact
Git Forge: [https://codeberg.org/Derpitron](https://github.com/Derpitron)  
LinkedIn: https://www.linkedin.com/in/b328dy67ss53a69b321/  
Email: aadhithyanm[at]protonmail[dot]com
# Education
## B.Tech in Electronics and Computer Engineering
at *Vellore Institute of Technology, Chennai*, ongoing (2024-2028)
Current CGPA: 7.61
## 12th Standard  
*BVM Global Perungudi*, 2024  
Board Exam Marks: 90%
## 10th Standard  
*Navadisha Montessori School*, 2022  
Board Exam Marks: 88.2%
# Work Experience
## Linux User Group, VIT Chennai
### Technical Team Member
2024-2026
#### Event Management
- Helped manage the club's Cyber-0-Day 3.0 and 4.0 CTF events through on-site technical support and pre-planning:
	- Live technical support for players facing network or challenge issues using Bash commandline
	- ParrotOS Linux installation for players across various laptop hardware, in Bare-metal and Virtualbox VM settings.
#### Projects
- [Whats4Linux](https://github.com/lugvitc/whats4linux)
	- A third-party WhatsApp client for Linux Desktop OSes, built with native technologies.
	- I designed the app icon, promotional material, and contributed some feature documentation
	##### Tools:
	- Figma, Inkscape
	##### Skills
	- Graphic Design
		- App Icon Design, Vector Art, Typography
	- Program Documentation
### Technical Lead
*2026-present*
#### Projects
- [LUGVITC Webring](https://github.com/lugvitc/webring)
	- I set up a Webring for LUGVITC members to join.
		- I drafted user-friendly instructions for club members to add their personal websites to the list and integrate them in.
		- This involved drafting a *soft* privacy policy for users, to inform them about where and how their data would be shared across the internet.
	- I helped integrate it with the [VIT Webring](https://webring-vit.vercel.app). 
		- This involved initiating outreach, deliberation, and consensus on a common format to use for sharing our webring member lists to them. Including technical support on both our ends.
		- **Tools:** Github Actions,  HTML5, JSON
	- Integrated [our club's blog website](https://blog.lugvitc.tech) into the webring
		- **Tools:**  Astro, CSS3
## Mafkin Robotics
### Software and ROS Engineer
*May-December, 2025*
I worked with fellow interns to create, develop, and test a semi-autonomous differential drive robot prototype for 3d mapping, integrating sensor fusion across odometers, IMU sensors, and a Zed 2i Depth Camera, using industry-standard ROS 2 technologies such as `rviz2` and `ORB-Slam`. I created a unified control and analysis plane using `tmux`.

I have experience doing thorough audits across our robot's codebase, gaining a deep understanding of the system, and using that knowledge to refactor for correctness, terse code, and maintainability. This involved an intimate sense of "code smell" and code organisation, as well as documenting and formalising our commands using Makefiles. Further details are under NDA.

I set up user-friendly control scripts for robot control using Bash scripting, allowing team members to operate and test the robot and its' tools in a few short clicks.
#### Tools
ROS 2 "Humble", Python 3, Arduino IDE/CLI, Ubuntu Linux 22.04, `udev` for USB, IPv4 private networking, Gstreamer, GNU make, Bash shell, Git, Github.
#### Hardware
##### Compute
Nvidia Jetson Orin Nano, Raspberry Pi 4b, Arduino, ESP32
##### Networking
Ethernet
##### Sensors
Optical Rotary Encoder,  Inertial Measurement Unit, Zed 2i Stereo Camera, Time of flight Camera
##### Actuators
Heavy-duty Motor Driver
#### Skills
- Designing and integrating software across Python, Arduino, Linux OS, and local network as part of a unified robot operation system.
- Profiling and optimising sensor data and video feed transmission network usage for real-time latency
- Documentation and formalisation of engineering knowledge and product requirements by uncovering assumptions and gaps in team knowledge.
- Instituted usage of code version control for maintenance ease down the road
- Designing interfaces/dashboards for my teammates to use, to quickly start and understand robot operation in as few steps as possible.
# Papers
## [Beyond Copyright Enforcement - Technological Protection Measures and User Rights in India](https://28litermicrowave.com/paper.pdf)
An analysis of Technological Protection Measures (DRM) in software products and practices associated with the enforcement of TPMs, and their implications for user rights, software competition, and digital sovereignty in the Indian context. My co-authors presented the paper at [ISDD 2026](https://www.bits-pilani.ac.in/event/isdd-2026/)
- Co-authored with [Sabarigirish Manikandan](https://28litermicrowave.com) and [Akash S.](https://www.linkedin.com/in/akash-s-101b6a297/).
- This conference was held at BITS Pilani, sponsored by the Ministry of Youth Affairs and Sports, Government of India, in January 2026.
# Projects
## [[WIP] Derp's Sense of Speed Camera for BeamNG.Drive](https://codeberg.org/derpitron/BeamNG-Speed-Camera/src/branch/hawaii)
A physics-based third-person custom camera effects mod for the BeamNG.Drive vehicle physics game. Utilises vehicle driving dynamics values from the game's physics engine to convey a violent sense of speed and momentum to the player's camera, visually inspired by arcade racing games. I created a method-chaining based API for expressing 3D vector and quaternion transformations in a legible format in code, implemented a small shim integration in the game engine to tap out physics values for processing, and a small visualisation/debug library for aiding me in effects construction.
**Technologies:** Lua, BeamNG.Drive, Signal Processing, Vehicle Dynamics, Visual Effects programming, API Design, 3D Vector and Quaternion Algebra, Game Feel
**Preview:**
Before:
![](https://www.youtube.com/watch?v=ktM3qMj4JmY)


After:
![](https://www.youtube.com/watch?v=qRc3TTb5zes)
## [[WIP] Homelab](https://codeberg.org/derpitron/tutu-nixos)
NixOS configuration for my home server. Auto-configured with Secure Boot, Immutability, User/file ACLs, secrets management, encrypted ZFS/BTRFS disk pool configurations, and SFTP fileserver. Provides multiple users for my family. Integrated closely with my Home Networking setup.

**Technologies:** Linux System Administration, NixOS, SystemD, Alpine Linux, Devops, Basic system security auditing, Service and User management, Bash, Git

## [WIP] Home Networking
I manage my home network with my router running OpenWRT, and have dumped the firmware of my ISP-provided ONT. I manage software security, firewall rules, network uptime, and Ethernet cabling for my house. I keep up to date with various router/embedded device modification techniques for Indian ISPs across broadband consumer forums. Integrated closely with my Homelab.

**Technologies:** Busybox, Embedded Linux, nftables Firewall, Embedded Device Analysis, Firmware Analysis, IPv4/IPv6 networking, DNS, Basic PPPoE usage skill

## [Discord OTP Forcer](https://codeberg.org/Discord-OTP-Forcer/Discord-OTP-Forcer)
A user-friendly program to help people attempt to recover their [Discord](https://discord.com) accounts, if they lost their TOTP authenticator keys. Written in strongly typed Python, using Selenium web driver (Chromium), and web scraping techniques. I read IETF RFC 6238 in an unsuccesful attempt to find vulnerabilities in the TOTP standard which I could use. I implemented configurable program timing to keep the program within respectful service limits, multiple configuration options for diverse user situations requested over the years, and implemented automatic error detection and recovery for a user-friendly experience.  Over time, users have reported success in account recovery with this program, or have turned into contributors/maintainers to the program, building a sort of community.

**Technologies:** Typed Python, Pyrefly, Selenium, Web Scraping, YAML, Discord API

## [ICSE Tamil Translations](https://icse-tamil-translations.github.io)
Built a website with my school classmates to translate ICSE's 9th and 10th standard Tamil language syllabus texts into English, for easy study and reference. Continues to recieve traffic through the years.

**Technologies:** Github Pages, Github Actions, Jekyll Static Site Generator, HTML, CSS, Google Analytics

# Other Skills
C, Rust, Java, basic web dev, basic C++, PC Building/Hardware maintenance, Android rooting, MySQL, Windows Desktop power usage, Docker, Media file management,

# Interests
Common Lisp, Functional Programming, Type Systems, 3D Geometry, Robot/Vehicle telemetry, Vehicle cosmetics/facelift design, Self-hosted software and community self-sufficiency, General purpose computing freedom
