---
title: External Radar
description: Proof-of-concept external radar for GTA5 Majestic RP built with the EyeAuras API.
published: true
date: 2026-05-19
order: 40
---

# External Radar

> **Download POC/source:** [GTA 5 RP Majestic External Radar rev.3 v1.9.9572.0](<https://s3.eyeauras.net/packs/S20260518123211DwtEcGoQR6ut/6922019586935714832/GTA_5_RP_Majestic_External_Radar_[poc,_source]_rev.3_v1.9.9572.0.zip>)

This page describes a proof of concept for an External Radar for GTA 5 Majestic RP built through the EyeAuras API.

The goal was to check how realistic it is to build or reverse an External Radar using only the EyeAuras API and collect complete ped information from two sources:

- `stream meta` from `majestic-client.dll`
- native data from `GTA5.exe`

## What Was Used

- [ReProcess](https://dev.eyeauras.net/share/S20260422083348SIiNglgRSqSJ), built into Radar
- [IMemory / IProcess](https://wiki.eyeauras.net/ru/scripting/memory-api/backends/local-process) from the EyeAuras documentation
- OpenAI Codex together with:
  - ReProcess
  - [Agent Guidance](https://wiki.eyeauras.net/en/features/ai-assistant)

## DMA Notes

DMA requires tight optimization.

This proof of concept does not include that optimization, because the DMA approach was not the focus of the final result and the only available DMA board failed.

With other process access methods, the radar works well. Props are the main exception and require separate handling.

## First Prototype

The first prototype took about 1 hour.

It used the following sources:

- map from the Majestic RP wiki
- icons from the Majestic RP wiki
- signatures and offsets from a public UC topic

## Result

After 48 hours, including 0 hours spent on manual coding, a working result was assembled.

[Result video](https://youtu.be/z43l5XC8NCI?si=4_ijOCJRrGKFMTNs)
