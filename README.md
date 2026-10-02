# Learning Networking Basics (Cisco)

Going through Cisco's Networking Basics course (Skills for All /
NetAcad) with Packet Tracer 9.0.1. Writing up each module as I go so
I actually remember it. End goal is DevOps, so I care about real
fundamentals, not just collecting a certificate.

## What's here

- [`modules/`](modules/) - my notes, one file per module
- [`labs/`](labs/) - Packet Tracer `.pkt` files + a short note per lab
  on what I did and what broke

## Notes

- [Module 00 - Meeting Packet Tracer](modules/module_00.md): first
  look at the app.

- [Labs](labs/) will have some notes of my progress too.

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
