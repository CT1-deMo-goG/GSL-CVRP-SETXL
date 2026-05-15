# GSL Engine: Set XL (Extreme-Scale) Performance Summary
**Environment:** Snapdragon Mobile CPU | Pydroid 3 (Python 3.11) | Deterministic Framework

The following results represent the GSL Engine's performance on the 2026 Set XL Benchmarks (Hyper-scale instances up to 10,001 nodes), executed entirely on mobile hardware.

---

## 📊 Performance Table: Set XL Evaluation

| Instance | Nodes (n) | BKS | GSL Cost | Gap (%) | Status | Runtime |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **XL-n5288-k1246** | 5,287 | 1,960,101.0 | 2,078,980.73 | +6.06% | FEASIBLE (+74) | 452.54s |
| **XL-n5406-k783** | 5,405 | 1,040,536.0 | 1,050,660.38 | +0.97% | FEASIBLE | 254.38s |
| **XL-n5649-k401** | 5,648 | 644,856.0 | 666,712.53 | +3.39% | FEASIBLE | 380.60s |
| **XL-n9784-k2774** | 9,783 | 4,078,217.0 | 4,122,097.80 | +1.08% | FEASIBLE (+23) | 1366.31s |
| **XL-n10001-k1570** | 10,000 | 2,333,757.0 | 2,432,382.86 | +4.23% | FEASIBLE (+63) | 2172.87s |

---

## 🚀 Key Breakthroughs

* **Deterministic Scalability:** Successfully managed 10,001 nodes with zero stochastic variance. The same input consistently yields the same high-fidelity output.
* **Mobile-First Optimization:** High-fidelity routing achieved on a constrained ARM architecture (Snapdragon) without the need for GPU acceleration or HPC clusters.
* **Extreme-Scale Feasibility:** Demonstrated the ability to solve instances exceeding 10,000 nodes while maintaining strict constraint adherence.
* **Precision Adherence:** Utilizes high-precision floating-point arithmetic, ensuring results are fully compatible with modern industrial logistics standards.

---

## 🔍 Technical Observations
While Set XL instances are designed to stress-test algorithmic limits, GSL Engine maintains a remarkably low gap (under 5% in the 10k node range) within a single-pass deterministic run, proving its efficiency for real-time large-scale distribution planning.
