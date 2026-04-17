# Kampanos Clock App

> Real-time BLE data streaming interface for IoT clock devices — built remotely for a European client.

[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![React Native](https://img.shields.io/badge/React%20Native-61DAFB?style=flat-square&logo=react&logoColor=black)](https://reactnative.dev/)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)](https://firebase.google.com/)

## Overview

Mobile application that streams real-time data from Bluetooth Low Energy (BLE) devices — specifically IoT clock hardware — into a live dashboard. Built as a remote contractor for **Kampanos**, a European tech company.

Data flows from physical BLE hardware → React Native → Firebase Realtime Database → live UI update, with no polling — fully event-driven.

## Features

- Real-time BLE device discovery and connection
- Live data ingestion via Firebase Realtime Database
- Event-driven architecture — no polling
- Cross-platform mobile (iOS / Android)

## Tech Stack

| Layer | Technology |
|---|---|
| Mobile | React Native |
| Language | TypeScript |
| BLE | react-native-ble-plx |
| Realtime DB | Firebase Realtime Database |
| Auth | Firebase Auth |

## Architecture

```
BLE Hardware Device
       │
       ▼ (Bluetooth Low Energy)
React Native App
       │
       ▼ (Firebase SDK)
Firebase Realtime Database
       │
       ▼ (onValue listener)
Live UI — real-time updates
```

## Context

This project was developed **fully remote** for Kampanos (Europe). It was part of a broader IoT ecosystem integrating physical hardware with a mobile-first interface.

---

*Part of the Kampanos product ecosystem — [kampanos.pt](https://kampanos.pt)*
