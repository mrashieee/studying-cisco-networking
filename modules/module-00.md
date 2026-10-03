# Module 00 - Meeting Packet Tracer

First time opening the app. This is just me mapping the interface so
I stop clicking around blindly.

## What it is

Packet Tracer is Cisco's network simulator. You drag in routers,
switches, PCs and cables, wire them up, configure them in a fake CLI,
and watch packets move. No real hardware involved, so nothing can
break. Fun to mess with.

## The interface

**Menu bar** - normal stuff. File handles `.pkt` files. Activity
Wizard is under Extensions, that's what makes graded labs.

**Toolbar** - icons under the menu. Zoom, drawing tools, and the
packet tools:
- Closed envelope = simple PDU. Fires one packet, tells you pass/fail.
- Open envelope = complex PDU. Same thing but you pick the details.
- Delete and Inspect are there too.

**Logical / Physical tabs** - top left.
- Logical is the topology. Who connects to who. Placement means
  nothing. Almost all work happens here.
- Physical is the map view: city, building, wiring closet. Rack holds
  the big gear, Table holds PCs, Shelf holds spares. Moving stuff
  here changes nothing about the network. It's just organizing.

**Device box** - bottom left, the parts shelf. Pick a category on the
left, pick a model on the right. The lightning bolt is cables:
console, straight-through, crossover, fiber, serial. Early labs are
half about picking the right cable.

**Workspace** - the middle. Drag stuff in, click a cable, click two
devices. Green dot means the link is up, red means down.

**Realtime / Simulation** - bottom right.
- Realtime just runs like the real thing.
- Simulation freezes time so you can step a packet hop by hop and
  open it up to see the layers. This is where you actually learn.

**Clicking a device** gives you tabs:
- Physical - the box itself. Power switch, slots, modules.
- Config - point-and-click settings.
- CLI - the fake IOS terminal. Same commands as real gear.
- Desktop - only on PCs. Has IP config, terminal, browser, etc.
- Services - only on servers. Where you turn on stuff like HTTP,
  DHCP, DNS so the rest of the network can use it.

## Takeaway

Build in Logical, check it in Realtime, understand it in Simulation,
configure it in CLI. Config tab is training wheels - if I can do it
in CLI, I actually know it. Stuck on anything: go to Simulation,
send one packet, open it at each hop.
