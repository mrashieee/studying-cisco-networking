# Learning Networking Basics (Cisco)

Going through Cisco's Networking Basics course (Skills for All /
NetAcad) with Packet Tracer 9.0.1. Writing up each module as I go so
I actually remember it. End goal is DevOps, so I care about real
fundamentals, not just collecting a certificate.

## What's here

- [`modules/`](modules/) - my notes, one file per module
- [`labs/`](labs/) - Packet Tracer `.pka` files + a short note per lab
  on what I did and what broke

## Notes

- [Module 00 - Meeting Packet Tracer](modules/module-00.md): first
  look at the app.
- [Module 01 - Communications in a Connected World](modules/module-01.md):
  network types, data and bits, bandwidth vs throughput vs latency.
- [Module 02 - Network Components, Types, and Connections](modules/module-02.md):
  clients and servers, P2P, network components, ISP services.
- [Module 03 - Wireless and Mobile Networks](modules/module-03.md):
  GSM to 5G, Wi-Fi, Bluetooth, NFC, GPS, connecting phones.
- [Module 04 - Build a Home Network](modules/module-04.md):
  router ports, wired and wireless tech, Wi-Fi settings, home lab.
- [Checkpoint Exam 1](modules/checkpoint-exam-1.md): modules 1-4
  review questions.
- [Module 05 - Communication Principles](modules/module-05.md):
  protocols, message rules, standards, OSI and TCP/IP models.
- [Module 06 - Network Media](modules/module-06.md): copper, coax,
  fiber, picking the right cable.
- [Module 07 - The Access Layer](modules/module-07.md): Ethernet
  frame fields, encapsulation, switches and MAC tables.
- [Checkpoint Exam 2](modules/checkpoint-exam-2.md): modules 5-7
  review questions.

## Labs

- [Create a Simple Network](labs/create-simple-network.md): one PC and
  one laptop wired up - addressing table and DHCP notes.
- [Packet Tracer Quiz](labs/packet-tracer-quiz.md): intro-course final,
  100% first try, plus what a default gateway actually is.
- [Configure a Wireless Router and Clients](labs/module-4-setup-home-router.md):
  wired a house, router GUI setup, wireless LAN, all online.

## Progress

- [x] Enrolled, Packet Tracer running
- [x] Course 1: Getting Started with Cisco Packet Tracer
- [ ] Course 2: Networking Basics

## Linux parallels

After each module I redo the same idea natively on Linux, since that's what
actually matters for me:

- addressing → `ip -brief address`
- connectivity → `ping -c4`, `tracepath`
- listening ports → `ss -tlnp`
- name resolution → `getent hosts <name>`
- HTTP → `curl -v <url>`
