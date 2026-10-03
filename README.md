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

## Labs

- [Create a Simple Network](labs/create-simple-network.md): one PC and
  one laptop wired up - addressing table and DHCP notes.
- [Packet Tracer Quiz](labs/packet-tracer-quiz.md): intro-course final,
  100% first try, plus what a default gateway actually is.

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
