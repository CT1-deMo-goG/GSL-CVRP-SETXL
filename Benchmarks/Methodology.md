# Hyper-Scale Performance Report: Set XL (1,000 - 10,000 Nodes)

This folder documents the performance of the GSL Engine in hyper-scale environments, comparing its deterministic efficiency against **Clarke-Wright (CW)** and **LNS (Iteration-bounded)** baselines.

## ⚙️ Benchmarking Methodology & Environment
At the hyper-scale level (up to 10,001 nodes), computational endurance, memory management, and time-to-solution are the critical metrics.

* **Hardware:** Native execution on a mobile processor (Snapdragon via Pydroid 3).
* **LNS Constraint:** Bounded to **300 iterations**. In 10,000-node environments, stochastic metaheuristics (LNS) suffer from "search space explosion," where 300 iterations are insufficient to find high-quality solutions within a real-time window.
* **CW Baseline:** Standard Clarke-Wright savings heuristic (constructive).
* **GSL Engine:** Operates under a **Deterministic Structured Framework**. It utilizes precise decomposition to maintain feasibility and quality even when stochastic methods fail to converge within the same time constraints.

## 📊 Hyper-Scale Benchmark Table (Performance Sample)
Performance results for 1,000 to 10,000-node instances, focusing on the Gap to BKS and operational feasibility.

| Instance | Nodes (n) | BKS | GSL Gap | CW Gap | LNS Gap (300 Iter) | GSL vs LNS Winner |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| XL-n1094-k157 | 1,094 | 112431.0 | **+2.77%** | +2.86% | +12.33% | **GSL** |
| XL-n2121-k186 | 2,121 | 283211.0 | **+3.19%** | +4.11% | +18.52% | **GSL** |
| XL-n5406-k783 | 5,405 | 1040536.0 | **+0.97%** | +1.34% | +24.40% | **GSL** |
| XL-n10001-k1570 | 10,001 | 2333757.0 | **+4.23%** | +5.31% | +38.10% | **GSL** |

## ⚡ Scalability Insights

* **10,000 Node Threshold:** GSL successfully processes 10,001 nodes on mobile hardware, maintaining a low single-digit gap where metaheuristics struggle to stay competitive within real-time limits.
* **Deterministic Stability:** Unlike search-based methods, GSL's structured logic ensures that quality remains robust and predictable as node counts increase.
* **Zero-Reversal Feasibility:** 100% of the solutions in this set are verified for feasibility, ensuring strict adherence to vehicle capacity (K) and demand constraints at scale.
* 
