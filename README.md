# dual-regulated-dc-power-supply-via-transformer
Design and implementation of a transformer-based dual regulated DC power supply providing stable 9V and 12V outputs using bridge rectification, capacitor filtering, and LM7809/LM7812 voltage regulators.
# Transformer-Based Dual Regulated DC Power Supply

A transformer-based dual-output regulated DC power supply designed to provide stable **9V and 12V DC outputs** for electronic circuits, embedded systems, communication modules, sensors, and laboratory applications.

## 📌 Project Overview

This project converts **230V AC mains** into regulated low-voltage DC using a step-down transformer, bridge rectifier, filter capacitor, and linear voltage regulators.

The system provides two regulated outputs:

- **9V DC** using LM7809
- **12V DC** using LM7812

LED indicators are provided to visually indicate the availability of the regulated outputs.

## ⚙️ System Block Diagram

```text
230V AC
   │
   ▼
12-0-12V Step-Down Transformer
   │
   ▼
Bridge Rectifier
(4 × 1N4007)
   │
   ▼
Filter Capacitor
   │
   ▼
 ┌───────────────┐
 │               │
 ▼               ▼
LM7809          LM7812
 │               │
 ▼               ▼
9V DC           12V DC
 │               │
 ▼               ▼
LED Indicator   LED Indicator
