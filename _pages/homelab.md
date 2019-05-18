---
permalink: /projects/homelab
layout: single
title: "Home Network & Servers"
---

<img src="https://media.darkwire.com/homelab/full_rack.jpg">

Top to bottom:

Coax patch panel<br/>
Blank panel insert with coax splitter<br/>
Cat 6 patch panel<br/>
Edimax GS-1026 V2 Gigabit switch

4 x Ubiquiti PoE Injectors<br/>
Ubiquiti EdgeRouter-X

Google Home Mini<br/>
HP ML310e v2 running VMware

APC Back-UPS ES 550

<img src="https://media.darkwire.com/homelab/pre_install.jpg">
This was my starting point. The in-wall wiring was done but it was up to me to deal with termination at both the wall jacks and the head end in my garage.

<img src="https://media.darkwire.com/homelab/initial_pull.jpg">
I've always liked using 3/4" plywood as a backer board as it's sturdy enough to mount any kind of gear. I opted to move the wire runs up near the top as they don't change much once everything is in place. I also wanted to leave space to mount my server if possible. This initial setup was just enough to get me online.

<img src="https://media.darkwire.com/homelab/patch_panels.jpg">
Each room has one or more wall plates with one coax and two Ethernet runs that connect back to this set of patch panels. The in-wall wiring is all quad-shielded RG-6 coax and Cat 6 Ethernet in order to support any present day needs as well as provide a reasonable level of future-proofing. Some people will suggest pulling optical fiber in the walls but I just don't think it's justified for home use, particularly with 2.5 and 5 gigabit options over Cat 6 becoming available.

<img src="https://media.darkwire.com/homelab/fiber_feed.jpg">
This is the inside of the telecom box used to provide CenturyLink fiber service. The black line running from the top of the box is the fiber feed from the telephone pole. The gray Cat 5e and black power cables run through the middle conduit to my garage.
 
<img src="https://media.darkwire.com/homelab/adtran_router.jpg">
The box actually contains an Adtran Total Access 352 ONT that converts the fiber into a pair of Ethernet ports and a pair of phone lines.
