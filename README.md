# GSL Engine: Set XL Performance Portfolio

**Deterministic CVRP Routing Framework for Hyper-Scale Benchmarks (1,000–10,000+ Nodes)**

---

# Overview

GSL Engine is a proprietary deterministic routing framework engineered for large-scale Capacitated Vehicle Routing Problems (CVRP). The framework emphasizes reproducible routing behavior, deterministic feasibility validation, and scalable execution under constrained mobile-edge environments.

This repository documents benchmark evaluations conducted on the CVRPLIB Set XL benchmark family.

---

# 📊 Benchmark Evaluation (Set XL)

The framework was evaluated across all 100 instances of the CVRPLIB Set XL benchmark suite.

Comparative experiments were conducted against commonly used heuristic baselines:

- Clarke-Wright Savings (CW)
- Large Neighborhood Search (LNS – 300 Iterations)

---

## Evaluation Summary

* **Benchmark Coverage:** 100 / 100 Instances
* **Observed Feasibility:** All reported solutions satisfied CVRP feasibility constraints under the tested configuration
* **Observed Win Rate vs LNS (300 Iterations):** 82%
* **Execution Environment:** Mobile Snapdragon Architecture via Python/Pydroid 3
* **Largest Evaluated Instance:** `XL-n10001-k1570`

> **Note:**  
> Comparative results reflect the execution settings and runtime constraints documented in this repository and should not be interpreted as universal solver rankings.

---

# 📂 Repository Structure

Detailed benchmark data, execution logs, gap measurements, and comparative outputs are provided in CSV format for transparency and reproducibility.

## Included Resources

* 📦 **[Solution Files Archive](./GSL_SetXL_Verified_Solutions.zip)**  
  Archive containing verified `.sol` routing outputs for the Set XL benchmark suite.

* 📁 **[Benchmarks](./Benchmarks)**

  * 📊 [`Cw_setxl_benchmark_result.csv`](./Benchmarks/Cw_setxl_benchmark_result.csv)  
    Comparative evaluation against Clarke-Wright Savings

  * 📊 [`Lns_setxl_benchmark_result.csv`](./Benchmarks/Lns_setxl_benchmark_result.csv)  
    Comparative evaluation against LNS (300 Iterations)

  * 📝 [`Methodology.md`](./Benchmarks/Methodology.md)  
    Benchmark execution conditions and evaluation methodology

---

# 🔬 Research Focus

This repository explores:

- deterministic hyper-scale CVRP execution
- reproducible routing behavior
- large-scale mobile-edge optimization experiments
- feasibility-oriented routing systems
- constrained-runtime routing evaluation
- scalability behavior under massive search spaces

---

# ⚙️ Execution Environment

* **Platform:** Android (Mobile Edge)
* **Runtime:** Python via Pydroid 3
* **CPU Architecture:** Snapdragon (ARM-based)
* **Execution Style:** Deterministic routing execution
* **Constraint Handling:** Deterministic feasibility validation

---

# 🔍 Operational Characteristics

## Observed Framework Characteristics

- deterministic routing reproducibility
- stable execution behavior across scaling ranges
- mobile-native execution capability
- feasibility-oriented route construction
- large-scale routing under constrained hardware environments

> **Technical Note:**  
> This repository focuses on deterministic execution behavior and feasibility-oriented routing evaluation under constrained mobile-edge conditions. Reported benchmark outcomes should be interpreted within the documented execution configuration.

---

# GSL-Solver Platform

## Deterministic Routing Platform

Access the routing platform here:

🔗 [https://gsl-solver.com](https://gsl-solver.com)

---

# Professional Contact

**Independent Researcher:**  
Chonmapoohm Thamsuwan (CTSuwan)

📧 [ctsuwan@proton.me](mailto:ctsuwan@proton.me)

---

# Services & Collaboration

Open to collaboration and professional engagement in areas including:

- Logistics-as-a-Service (LaaS)
- Deterministic routing systems
- Hyper-scale CVRP experimentation
- Constraint-based logistics optimization
- Mobile-edge optimization research
- Large-scale routing stress testing
- Research and industrial collaboration
