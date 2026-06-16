# Fleet Management System (FMS) — Core Application

An enterprise-grade iOS application designed to bridge the gap between real-time vehicle logistics, workshop technician execution, and smart inventory management. 

Traditional fleet solutions are purely reactive. This platform uses a workflow-driven architecture coupled with on-device AI to shift logistics into a proactive state.

## The Problem Statement:

Fleet maintenance ecosystems routinely struggle with fragmented communication, delayed spare parts pipelines, and a lack of real-time visibility into active repairs. When a vehicle undergoes critical breakdown:
1. **Technicians** waste time searching inventory databases manually or deciphering handwritten service history.
2. **Parts Managers** struggle with reactive reordering, resulting in critical parts hitting zero stock during high-volume periods.
3. **Operations Managers** lose track of vehicle trip constraints, leading to dispatching errors and extended fleet downtime.

## The Solution: FMS Integration:

This application consolidates the entire fleet lifecycle into an interconnected, 7-group architectural map:

* **🔒 Secure Operations (Group 1):** Role-based secure authentication ensuring data privacy and auditable entry logs.
* **📋 Task Management & Execution (Groups 2 & 3):** Centralized high-priority alert queues linked directly to a live digital workspace where technicians capture visual evidence, parse diagnostic fault codes, and log active labor.
* **📦 Smart Supply Chain (Group 4):** Live inventory tracking that connects active work orders with parts consumption logs to automatically adjust quantities.
* **💬 Barrier-Free Logistics (Group 5 & 8):** Multi-language communication channels enabling automated translation between cross-functional teams alongside active trip tracking.
* **📊 Performance Metrics (Group 6):** Searchable, audit-ready digital maintenance logs visualizing fleet health trends for long-term operational optimization.

---

## Core Engineering: On-Device Apple Intelligence:

FMS leverages Apple's native `FoundationModels` framework to run secure, local Large Language Models (LLMs) on-device. This allows the system to compute mission-critical logistics without external cloud dependencies:

1. **Predictive Maintenance:** Monitors real-time vehicle telemetry and logs anomalies to predict parts failures before an on-road breakdown occurs.
2. **Smart Restocking Forecasts:** Automatically reviews historical parts consumption against the upcoming work order pipeline to suggest order velocity and flag critical bottlenecks.
3. **Strategic Warehouse Insights:** Evaluates warehouse usage history to provide managers with immediate, actionable operational tips to improve space and storage layouts.

---

## Technology Stack & Dependencies:

* **UI Framework:** SwiftUI (State & Observation Architecture)
* **Intelligence:** FoundationModels Framework (Apple Intelligence, iOS 18+ / macOS 15+ SDK)
* **Location Services:** CoreLocation & Geocoding Engine
* **Mapping UI:** MapKit / GoogleMaps SDK (Polyline tracking for live trips)
