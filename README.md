# Sentinel-Forensics: Regulatory-Grade Market Surveillance

[![Hackathon](https://img.shields.io/badge/Hackathon-DECODE%20X-red)](https://www.nldalmia.in/)
[![Achievement](https://img.shields.io/badge/Achievement-2nd%20Runner--Up-gold)](https://www.nldalmia.in/)
[![Participants](https://img.shields.io/badge/Participants-4000%2B-blue)](https://www.nldalmia.in/)

---

## Overview

This project was developed for the **DECODE X 24-Hour Hackathon Finale** hosted by the **N. L. Dalmia Institute of Management Studies and Research (NLDIMSR)**.

Our team, **Coding Chimps**, secured the **2nd Runner-Up** position among **4,000+ participants**.

**Case SENTINEL** addresses the challenge of isolating market manipulation in a *“universe of noise.”*

We acted as an **Independent Surveillance Analytics Advisory Team** to validate suspicious activity across:

- **1,294,422 orders**
- **254,984 master trades**

---

## The Problem

The objective was to detect sophisticated market manipulation while minimizing false positives — specifically distinguishing malicious actors from legitimate **High-Frequency Traders (HFTs)** to avoid:

- Regulatory overreach  
- Litigation exposure  
- Reputational damage  

---

## The Solution: The Synthesis Engine

We developed a **three-stage forensic framework** to classify and rank entities based on manipulative signatures.

---

### 1. Mechanism Classification

The engine detects and distinguishes between:

- **Circular Trading**  
  Identified via closed loops (L2 pairs and L3 rings) that lack economic rationale.

- **Pump & Dump**  
  Coordinated volume surges combined with artificial price movement.

- **Wash Orders**  
  Trades where buyer and seller are effectively the same entity, indicating fabricated liquidity.

---

### 2. Composite Risk Scoring (S)

We synthesized evidence across four dimensions to compute a final risk score:

**Score = S_motif (30%) + S_conc (25%) + S_network (25%) + S_sync (20%)**

- **S_motif (30%)**  
  Loop count and mechanism severity.

- **S_conc (25%)**  
  HHI concentration and wash-order rate.

- **S_network (25%)**  
  Network centrality metrics (PageRank, Betweenness).

- **S_sync (20%)**  
  Rapid-fire orders (<60 seconds) and synchronized trading pairs.

---

### 3. False Positive Firewall

To maintain high precision, we implemented a three-layer validation gate:

- **Gate L1 — Evidence Breadth**  
  Activity must trigger ≥ 2 independent dimensions.

- **Gate L2 — Statistical Outlier Check**  
  Z-score ≥ 2.0 relative to market distribution.

- **Gate L3 — HFT Filter**  
  Reclassified 376 suspects as legitimate traders based on high counterparty diversity and absence of persistent loops.

---

## Key Results

- **Critical Discovery**  
  Identified **Client L16WN** as a structural network hub with **24.9M+ sync pair events**, positioned **12.73 standard deviations** from the mean.

- **Escalation List**  
  Prioritized **12 high-risk entities** for regulatory action.

- **Award**  
  Received a **₹25,000 cash prize** for the proposed forensic framework.

---

## Team: Coding Chimps

- **Jugal Lachhwani** (23AIML033)
- **Hriday Patel** (23AIML052)
