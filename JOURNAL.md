---
title: "Custom SBC Project"
author: "your-name"
description: "A 10-day development journal for building a custom Single Board Computer"
created_at: "2026-04-01"
---

# April 1: Project planning and requirements

Started the day defining the core requirements for the SBC. Decided on
using a quad-core ARM processor with 4GB RAM. Created a detailed spec
sheet covering performance targets, I/O requirements, and power budget.
Sketched out the high-level block diagram and identified all major
subsystems: power management, CPU module, memory, storage, networking,
and peripherals.

**Total time spent: 5 hours**

# April 2: Schematic design - Power section

Began designing the power delivery system. Selected a suitable VRM
(voltage regulator module) capable of handling the processor's TDP.
Designed the 5V input stage with protection circuits and multiple
rails for different voltage domains. Added filtering and decoupling
capacitors throughout to ensure stable power delivery.

![power schematic](https://i.ytimg.com/vi/bCc2fZ-H_1s/hq720.jpg?sqp=-oaymwEhCK4FEIIDSFryq4qpAxMIARUAAAAAGAElAADIQj0AgKJD&rs=AOn4CLCsnfjV6OAZ1TjJfUtU5HvA6MJGMw)

**Total time spent: 4 hours**

# April 3: Schematic design - CPU and memory

Completed the CPU socket design and memory subsystem. Laid out the DDR4
SODIMM slot with proper trace impedance calculations. Added reset,
clock, and power management circuits for the processor. Double-checked
all signal integrity requirements and voltage thresholds.

**Total time spent: 6 hours**

# April 4: Schematic design - Peripherals and I/O

Designed the peripheral interfaces: two Gigabit Ethernet ports with
magjack connectors, USB 3.0 headers, SATA connectors, and HDMI output.
Added level shifters where needed and protection diodes on ESD-sensitive
lines. Created symbols for all connectors and finished the complete
schematic review.

**Total time spent: 5 hours**

# April 5: PCB layout - Stackup and power planes

Started the PCB layout process. Designed a 6-layer board stackup:
Signal, Ground, Power, Power, Ground, Signal. Created the power
distribution planes and defined via placement strategy. Began placing
critical components near their respective power sources to minimize
inductance and ensure proper current distribution.

![layer stackup](https://i.ytimg.com/vi/bCc2fZ-H_1s/hq720.jpg?sqp=-oaymwEhCK4FEIIDSFryq4qpAxMIARUAAAAAGAElAADIQj0AgKJD&rs=AOn4CLCsnfjV6OAZ1TjJfUtU5HvA6MJGMw)

**Total time spent: 4 hours**

# April 6: PCB layout - Component placement

Completed the component placement phase. Positioned the CPU in the center
with memory modules nearby for short traces. Arranged the Ethernet
controllers and USB hub logic adjacent to their respective connectors.
Rotated components strategically to reduce trace crossings. Ran design
rule checks and fixed clearance violations around the BGA pads.

**Total time spent: 5 hours**

# April 7: PCB layout - Signal routing

Spent the day routing high-speed signals. Carefully routed DDR4 traces
with proper length matching within 10 mils. Configured differential pair
routing for USB 3.0 signals and Ethernet lines. Added vias strategically
to transition between layers while maintaining impedance control. Hit
some tight routing challenges around the HDMI connector but found
creative solutions.

**Total time spent: 6 hours**

# April 8: PCB layout - Final touches and gerber generation

Completed power and ground routing. Added test points for debugging on
critical signals. Generated silkscreen labels for all connectors and
component values. Performed final design rule checks and fixed any
remaining violations. Generated Gerber files and submitted to PCB
manufacturer with 2-week delivery estimate.

![final pcb layout](https://i.ytimg.com/vi/bCc2fZ-H_1s/hq720.jpg?sqp=-oaymwEhCK4FEIIDSFryq4qpAxMIARUAAAAAGAElAADIQj0AgKJD&rs=AOn4CLCsnfjV6OAZ1TjJfUtU5HvA6MJGMw)

**Total time spent: 4 hours**

# April 9: Component sourcing and inventory management

Created a comprehensive bill of materials (BOM) with part numbers from
multiple suppliers. Sourced the CPU module, DDR4 SODIMM, Gigabit Ethernet
controllers, and USB hub IC. Found good deals on passive components from
LCSC and digikey. Started inventory tracking spreadsheet and received
first shipment of bulk components.

**Total time spent: 3 hours**

# April 10: Documentation and preparation for assembly

Wrote detailed assembly guide with photos of each stage. Created test
plan for post-assembly validation covering power delivery, CPU detection,
memory initialization, and peripheral enumeration. Prepared the work
station with soldering equipment and checked that all SMD rework tools
are calibrated. Pre-kitted components and labeled all positions for
efficient assembly.

**Total time spent: 5 hours**
