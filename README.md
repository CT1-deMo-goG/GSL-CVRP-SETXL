# GSL Engine: Set XL Performance Portfolio
**Hyper-Scale Deterministic Solver for CVRP (1,000 - 10,000 Nodes)**

## Overview
GSL Engine is a proprietary, high-performance solver specifically engineered for **Extreme-Scale** Capacitated Vehicle Routing Problems (CVRP). It utilizes a **Deterministic Structured Framework** to ensure 100% reproducible, stable, and **Real-time** solutions, even when processing instances exceeding 10,000 nodes on mobile hardware.

---

## 📊 Benchmark Validation (Set XL)
Evaluated against all 100 instances of CVRPLIB Set XL (Hyper-scale). This benchmark compares GSL Engine's deterministic efficiency against standard heuristic baselines: **Clarke-Wright (CW)** and **Large Neighborhood Search (LNS - 300 Iterations)**.

### Performance Summary
* **Instances:** 100 / 100 (Full Coverage)
* **Feasibility:** 100% Guaranteed Feasible Routes (Verified via CVRPLib Checker)
* **Win Rate vs LNS (300 Iter):** 82% (GSL demonstrates superior scalability as stochastic methods struggle with search space explosion at this scale)
* **Hardware:** Verified on Mobile Snapdragon Architecture (via Pydroid 3)
* **Max Scale:** Successfully resolved 10,001 nodes (`XL-n10001-k1570`) within a single-pass deterministic run.

---

## 📂 Repository Structure

All detailed benchmark results, including execution times, gap percentages, and head-to-head comparisons, are stored in CSV format for industrial analysis:

* 📦 **[Solution Files Archive](./GSL_SetXL_Verified_Solutions.zip)**: A compressed archive containing all verified `.sol` output files for the XL suite.
* 📁 **[Benchmarks](./Benchmarks)**: 
  * 📊 [`Cw_setxl_benchmark_result.csv`](./Benchmarks/Cw_setxl_benchmark_result.csv) (GSL vs. Clarke-Wright)
  * 📊 [`Lns_setxl_benchmark_result.csv`](./Benchmarks/Lns_setxl_benchmark_result.csv) (GSL vs. LNS 300-Iter)
  * 📝 [`Methodology.md`](./Benchmarks/Methodology.md) (Hyper-scale environment and constraints)

---

## 🔍 Operational Characteristics

### **Core Strengths**
* **Deterministic Scalability:** Engineered to maintain logic consistency from 1,000 to 10,000+ nodes. The same input consistently yields the same output, eliminating the risks associated with stochastic variance.
* **Mobile-Native Optimization:** High-fidelity routing achieved on ARM architecture, proving the engine's efficiency in resource-constrained or edge-computing scenarios.
* **Operational Integrity:** Prioritizes strict adherence to vehicle capacity (K) and demand constraints, ensuring every solution is "Deployment-Ready."

---

## GSL-Solver Platform

**The Enterprise Route Optimization Portal**
Access the production-ready deterministic engine here:  
[**https://gsl-solver.com**](https://gsl-solver.com)

---

## Professional Contact

**Independent Researcher:** Chonmapoohm Thamsuwan (CTSuwan)  
**Email:** [ctsuwan@proton.me](mailto:ctsuwan@proton.me)  

---

## Services & Collaboration

Open to professional engagement in the following areas:
- **Logistics-as-a-Service (LaaS):** Real-time route optimization for hyper-scale enterprise fleets.
- **Custom Algorithmic Development:** Tailored solutions for complex supply chain constraints.
- **Large-Scale Network Audit:** Stress-testing and optimization of massive distribution networks.
- 
