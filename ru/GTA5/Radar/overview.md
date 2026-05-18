---
title: External Radar
description: Proof-of-concept external radar для GTA5 Majestic RP, собранный через EyeAuras API.
published: true
date: 2026-05-19
order: 40
---

# External Radar

> **Скачать POC/source:** [GTA 5 RP Majestic External Radar rev.3 v1.9.9572.0](<https://s3.eyeauras.net/packs/S20260518123211DwtEcGoQR6ut/6922019586935714832/GTA_5_RP_Majestic_External_Radar_[poc,_source]_rev.3_v1.9.9572.0.zip>)

Эта страница описывает proof-of-concept External Radar для GTA 5 Majestic RP, собранный через EyeAuras API.

Цель была проверить, насколько реально с помощью только EyeAuras API написать или отреверсить External Radar и получить полную информацию о педах из двух источников:

- `stream meta` из `majestic-client.dll`
- native-информация из `GTA5.exe`

## Что использовалось

- [ReProcess](https://dev.eyeauras.net/share/S20260422083348SIiNglgRSqSJ), встроенный в Radar
- [IMemory / IProcess](https://wiki.eyeauras.net/ru/scripting/memory-api/backends/local-process) из документации EyeAuras
- OpenAI Codex в связке с:
  - ReProcess
  - [Agent Guidance](https://wiki.eyeauras.net/en/features/ai-assistant)

## Немного про DMA

Для DMA нужна плотная оптимизация.

В этом proof-of-concept такая оптимизация не делалась: DMA-подход не был фокусом итогового результата, а единственная доступная DMA-плата вышла из строя.

Со всеми остальными способами доступа к процессу радар работает хорошо. Основное исключение - пропы, для них нужна отдельная обработка.

## Первый прототип

На первый прототип ушло примерно 1 час.

Что было использовано:

- карта с wiki Majestic RP
- иконки с wiki Majestic RP
- signatures и offsets из публичной темы на UC

## Результат

Спустя 48 часов, из которых 0 часов было потрачено на ручной код, получился рабочий результат.

[Видео результата](https://youtu.be/z43l5XC8NCI?si=4_ijOCJRrGKFMTNs)
