---
title: "Introducing Voltii: A 1973 BMW 2002tii Goes Electric"
description: "Why this numbers-matching tii is going electric instead of an EFI restoration or a modern engine swap — and the technical plan so far."
date: 2026-08-29
tags: ["intro", "backstory", "technical overview"]
---

## The Car

This is a 1973 BMW 2002tii — chassis 2751676, right-hand drive, manufactured in Germany and originally delivered to a dealership in London. How and when it made its way to Australia isn't clear yet — still a gap in the car's history. It was delivered new in Inca Orange, and was repainted a deep navy blue at some point along the way. It also came factory-fitted with a Getrag 235/5 close-ratio dogleg 5-speed and a limited-slip differential — a combination fewer than 2,000 cars ever left the factory with. The original invoice confirms it. That dogleg gearbox is lost to time — gone before I owned the car. The car currently has a Getrag 245/10 five-speed overdrive gearbox fitted, likely from a later replacement or upgrade. That'll be coming out too, and will either go into storage or get sold on as a complete five-speed conversion setup for someone else's car. In its place, a Getrag 245/4 four-speed — the gearbox fitted to most 2002s of this era — will go in as part of the EV conversion.

## The Backstory: Why EV, Not EFI, Not K24

The tii's numbers-matching M10 engine, complete with its Kugelfischer mechanical injection, isn't going anywhere. It's coming out, and it's going into storage — cleaned, protected, and kept exactly as it is. If someone down the track wants to put this car back to original spec, they'll have everything they need to do it properly. I'm not cutting it up, I'm not selling it off, and I'm not pretending it doesn't matter. It matters. It's just not going to be doing the driving anymore.

So why not restore the Kugelfischer setup, or drop in a modern engine swap and call it a day?

Honestly — because neither of those excite me the way this does. A sympathetic EFI restoration is a beautiful thing on the right car, but it's still an M10 doing what M10s have always done, just with better fuel delivery. An engine swap — a K24, an M42, a 3S-GE, whatever the flavour of the month is in the 2002 community — brings its own learning curve and its own headaches, and I don't doubt it'd be a satisfying project in its own right. But it's also still, fundamentally, another engine in a bay that's had a few different engines in it over the decades. Neither path is *new* to me. Neither one asks me to learn anything I don't already half-know.

An EV conversion does. It's a genuinely different engineering problem — power delivery, packaging, weight distribution, compliance, all of it rebuilt from first principles instead of following someone else's shop manual. That's the appeal. I want to build something, not just install something.

And to be upfront about the elephant in the room: yes, I know some people think converting a numbers-matching tii to electric is close to sacrilege. I understand where that comes from, and I'm not going to pretend the car isn't collectible. But it's my car, I've kept the engine intact, and I'm not chasing anyone else's approval on this one. If that's not your cup of tea, that's completely fine — there are plenty of beautifully restored tiis out there doing exactly what people expect a tii to do. This one's going to do something else for a while.

**On reversibility:** I'm keeping chassis modifications to a minimum wherever I can. The engine, gearbox, and all the associated hardware will be preserved, and the goal is to avoid anything irreversible to the shell itself. That means a return to stock is technically on the table for a future owner. Realistically? I don't think it'll happen. But I'd rather leave the door open than slam it shut for no reason.

## The Technical Overview

**Powertrain**
The heart of the conversion is a Nissan Leaf EM57 motor and inverter — the standard 80kW/250Nm unit, not the higher-output e+ variant, chosen deliberately to stay within the limits of the BMW's small-case differential and rear axle hardware. Controller-side torque limiting is there as a backstop if needed.

Rather than keeping the Leaf's internal reduction gearset, this is a full transaxle delete. A coupler mounts directly to the EM57's raw output shaft, and drive goes straight into a Getrag 245/4 four-speed gearbox — the period-correct 4-speed for this era of 2002, replacing the car's current 245/10 five-speed — via an adapter system. The BMW diff — targeting a 4.10:1 ratio — does the only reduction work in the driveline.

Keeping a gearbox in the chain at all is a compromise, not the ideal outcome — most RWD EM57 conversions end up doing the same thing, running the box clutchless as a single-gear pass-through rather than eliminating it entirely. A cleaner direct-drive setup, or a simple 2:1 reduction unit, would be the neater solution on paper. Neither is a viable option for this build right now — the parts and reference builds for either just aren't there yet for a RHD 2002 — so the 245/4 stays in the driveline as the practical answer, even though the EM57's torque curve means the clutch and shifting will rarely, if ever, get used in daily driving.

**Brakes**
The RHD-specific remote servo brake booster is a known pain point — expensive and difficult to rebuild, and outside the coverage of the usual LHD-focused suppliers. The current plan is a Bosch iBooster, using factory RHD-specific part numbers sourced from Tesla platforms, which should sidestep the pedal box and clevis orientation issues that plague a straight LHD-to-RHD adaptation. It's CAN-free — just 12V ignition-switched power, 12V battery, and ground. OEM calipers and rear drums stay, pending engineering sign-off.

**Battery, BMS, and controller**
Still open. The battery pack decision — stock Leaf pack, reconfigured Leaf modules, or new EVE prismatic LFP cells — hasn't been locked in yet, with a rough target of 30–40kWh for around 150km of real-world local-area range. Controller and BMS selection is leaning toward an openinverter/Zombieverter setup paired with an Orion Jr2 or REC BMS, largely for the compliance credibility they bring to the table.

**Charging**
Standalone Elcon/TC-style OBC leaning, since the Leaf's factory unit is tied to its stock pack and BMS.

**Compliance**
This is going through Queensland's NCOP LV1 pathway, with a local TMR signatory engaged for sign-off. Battery restraint will be handled as an engineering calculation against NCOP g-ratings rather than destructive testing.

More posts to come as the gearbox adapter gets finalised and the tunnel gets opened up for inspection.
