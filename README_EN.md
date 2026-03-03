# 🅿️ ParkSafe — AI Parking & Safety Assistant

**ParkSafe** is a hybrid B2B and B2C platform that leverages Edge AI for real-time parking spot monitoring with a strict commitment to privacy (Privacy-by-Design).

## 📌 Project Overview
The project addresses the problem of inefficient parking searches ("cruising") and vehicle safety concerns. It provides drivers with precise navigation to specific spots while offering operators automation tools without legal risks.

## 🛠 Tech Stack
* **Computer Vision:** YOLOv8 on NVIDIA Jetson (Edge processing).
* **Backend:** FastAPI (Python), PostgreSQL + PostGIS.
* **Mobile:** React Native + Mapbox SDK + CarPlay Integration.
* **Architecture:** JSON-only data transfer (no video streaming to the cloud).

---

## 👥 User Personas

### 👔 Mike (B2B Operator)
* **Role:** Operations Manager at a large mixed-use development in San Jose.
* **Goal:** Automate monitoring for 1,500 spots and implement dynamic pricing.
* **Pain:** Fear of lawsuits due to illegal video surveillance (CCPA).
* **Solution:** Edge AI that transmits only numerical data (JSON) instead of video.

### 🏎 Alex (B2C Driver)
* **Role:** Senior Software Engineer, BMW M5 owner.
* **Goal:** Quickly find a secure spot (Safety Score) via CarPlay.
* **Pain:** ADHD-factor (difficulty concentrating), "ghost spots" in Google Maps.
* **Solution:** "Last Mile" navigation directly to an available slot.

---

## 🎯 Job-To-Be-Done (JTBD)

**For Alex:**
> **When** I'm rushing to a meeting in a congested downtown area in my BMW M5, **I want to** instantly find an available and secure spot via CarPlay, **so I can** arrive on time without wasting nerves on "cruising" through parking levels.

**For Mike:**
> **When** my parking lot gets congested and legal teams block traditional cameras, **I want to** implement anonymous AI monitoring **so I can** optimize traffic and free up patrols without violating privacy laws.

---

## 🌳 Opportunity Solution Tree (OST)

Development is structured around a core goal: **Reduce average cruising time by 30% while maintaining 100% privacy.**

* **Opportunities:**
    * Alex Vector: Speed and Safety (CarPlay, Safety Score).
    * Mike Vector: Legal Compliance and ROI (Edge AI, JSON-only).
* **Solutions:** Native CarPlay interface, architecture without cloud video streaming.
* **Experiments:** Launching data simulations for the Dashboard, user interviews on navigation prototypes.

---

## 💡 Product Hypotheses (Core Solution)

**Selected Hypothesis:**
> If we implement **"Last Mile"** navigation (Variant: **Slot Highlighter** — selecting a single ideal spot), then we will change driver behavior from "chaotic searching" to "direct following," resulting in a decrease in *cruising time*.

**Rationale:**
1.  CarPlay interface must be as simple as possible.
2.  Accounting for the ADHD-factor of users (minimum choice — maximum result).
3.  No need for complex infrastructure work (no fiber optic trenching required).

---

## 📊 Market Analysis
The repository includes a detailed `parksafe-competitive-analysis.html` file comparing ParkSafe with market leaders (**SpotHero, Parquery, Parkinto**).
**Our Uniqueness:** Combining B2B infrastructure (Edge AI) with a unique B2C experience (in-garage navigation to the slot).
