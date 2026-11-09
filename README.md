# Submodular Optimization, POMDPs & Sequential Control: Portfolio Selection, Diminishing Returns & Partially Observable Systems
### *From Discrete Concavity & Greedy Bounds to Belief-State Planning, Restless Bandits & Quickest Change Detection*

Welcome to **Submodular Optimization, POMDPs & Sequential Control: Portfolio Selection, Diminishing Returns & Partially Observable Systems**. This curriculum provides a rigorous, principled bridge between combinatorial optimization, discrete convex geometry, and stochastic control theory for engineering distributed systems, CI/CD runner fleets, hardware testbeds, and automated failure detection.

Modern systems engineering confronts two interrelated optimization challenges:
1. **The Static / Combinatorial Frontier (Submodular Portfolio Selection):** Given thousands of candidate test suites, observability sensors, canary metrics, or verification probes, which subset maximizes diagnostic coverage under strict execution time, dollar cost, or compute budgets? Because each added probe partially overlaps with already collected information, information exhibits diminishing marginal returns (submodularity).
2. **The Dynamic / Sequential Frontier (Partially Observable Markov Decision Processes):** Operating systems and hardware nodes degrade silently over time. Physical sensors, flaky tests, and telemetry probes yield noisy, delayed observations. When should a controller run an expensive probe, when should it reset a worker node, and when should it route production traffic elsewhere?

---

## 🚗 Twin Companion Architecture

The curriculum is structured into **two synchronized 1-to-1 parallel tracks**:

* 📖 **[Conceptual Track (`conceptual/`)](conceptual/README.md)**: A deep reading edition focusing on mathematical proofs, discrete convexity, belief-space geometry, physical intuition, and rigorous systems trade-offs (The Diminishing Returns Dimple, Sufficient Statistic Belief Simplex, The Cost of Delayed Information, and Hysteresis Bands).
* 🐍 **[Python Laboratory (`python/`)](python/README.md)**: A hands-on computational lab manual implementing submodular greedy optimizers, CELF lazy evaluations, value iteration on belief simplexes, Whittle index calculators, and CUSUM change detectors from scratch using `numpy`, `scipy`, and `matplotlib`.

---

## 📚 Master Curriculum Syllabus (`00`–`11`)

| Ch | Conceptual Track | Python Lab | Part | Core Topics & Key Concepts |
| :--- | :--- | :--- | :--- | :--- |
| **00** | **[Ch 00](conceptual/00_START_HERE.ipynb)** | **[Ch 00 (Python)](python/00_START_HERE.ipynb)** | Foundations | **The Big Picture** — Diminishing Returns, Hidden States & The Mathematics of Sequential Resource Allocation |
| **01** | **[Ch 01](conceptual/01_knapsack_and_lagrangian_shadow_prices.ipynb)** | **[Ch 01 (Python)](python/01_knapsack_and_lagrangian_shadow_prices.ipynb)** | Part I | **Constrained Optimization** — Knapsack Problems, LP Relaxations, Dual Lagrange Multipliers as Shadow Prices, and Bang-for-Buck Ranking |
| **02** | **[Ch 02](conceptual/02_submodular_set_functions_and_diminishing_returns.ipynb)** | **[Ch 02 (Python)](python/02_submodular_set_functions_and_diminishing_returns.ipynb)** | Part I | **Submodularity** — Discrete Concavity, Marginal Gain $\Delta(i \mid S)$, Coverage Functions, and Mutual Information as a Submodular Function |
| **03** | **[Ch 03](conceptual/03_nemhauser_wolsey_greedy_guarantees.ipynb)** | **[Ch 03 (Python)](python/03_nemhauser_wolsey_greedy_guarantees.ipynb)** | Part I | **Greedy Optimization Bounds** — The Nemhauser-Wolsey $(1 - 1/e) \approx 63.2\%$ Theorem, Cost-Scaled Greedy (CELF), and Sequential Backward Elimination |
| **04** | **[Ch 04](conceptual/04_markov_decision_processes_and_bellman_optimality.ipynb)** | **[Ch 04 (Python)](python/04_markov_decision_processes_and_bellman_optimality.ipynb)** | Part II | **Markov Decision Processes** — Bellman Equations, Value/Policy Iteration, Discounted Horizons, and Average-Cost MDPs |
| **05** | **[Ch 05](conceptual/05_pomdps_and_belief_state_mdps.ipynb)** | **[Ch 05 (Python)](python/05_pomdps_and_belief_state_mdps.ipynb)** | Part II | **Partially Observable MDPs (POMDPs)** — Sufficient Statistic Belief States $b_t$, Piece-Wise Linear Convex (PWLC) Value Functions, and Value of Information |
| **06** | **[Ch 06](conceptual/06_optimal_stopping_and_hysteresis_control.ipynb)** | **[Ch 06 (Python)](python/06_optimal_stopping_and_hysteresis_control.ipynb)** | Part II | **Optimal Stopping & Switching Costs** — Wald's Sequential Boundaries, $(s, S)$ Hysteresis Bands, and Preventing Policy Chattering |
| **07** | **[Ch 07](conceptual/07_multi_armed_bandits_gittins_and_whittle_indices.ipynb)** | **[Ch 07 (Python)](python/07_multi_armed_bandits_gittins_and_whittle_indices.ipynb)** | Part III | **Restless Bandits** — Exploration vs. Exploitation, Gittins Index for Stopping Problems, and Whittle Index for Restless Monitoring Channels |
| **08** | **[Ch 08](conceptual/08_quickest_change_detection_cusum_and_shiryaev_roberts.ipynb)** | **[Ch 08 (Python)](python/08_quickest_change_detection_cusum_and_shiryaev_roberts.ipynb)** | Part III | **Quickest Change Detection** — Page's CUSUM, Shiryaev-Roberts Procedure, and Lorden's Asymptotic KL Delay Bound ($\frac{\ln \text{ARL}_0}{D_{\text{KL}}}$) |
| **09** | **[Ch 09](conceptual/09_mechanism_design_and_tragedy_of_the_commons.ipynb)** | **[Ch 09 (Python)](python/09_mechanism_design_and_tragedy_of_the_commons.ipynb)** | Part III | **Mechanism Design for Shared Infrastructure** — Tragedy of the Commons, Externalities, Pigouvian Congestion Pricing, and Incentive-Compatible Quotas |
| **10** | **[Appendix A](conceptual/10_appendix_optimization_and_control_rosetta_stone.ipynb)** | **[Appendix A (Python)](python/10_appendix_optimization_and_control_rosetta_stone.ipynb)** | Reference | **Rosetta Stone & Diagnostic Guide** — The Submodular Optimization, POMDP & Control Theory Mathematical Reference |
| **11** | **[Appendix B](conceptual/11_appendix_submodular_selection_and_pomdp_governance_of_flaky_tests.ipynb)** | **[Appendix B (Python)](python/11_appendix_submodular_selection_and_pomdp_governance_of_flaky_tests.ipynb)** | Reference | **Systems Case Studies** — Submodular Suite Selection, POMDP Venue Routing & Quickest Change Detection for Flaky Tests |

---

## 🚀 Getting Started

### Prerequisites

The curriculum runs on standard scientific Python 3.10+ environments:
* `numpy` (array operations, vectorization)
* `scipy` (linear programming `linprog`, dynamic programming, optimization)
* `matplotlib` (multi-panel state space visualizations)
* `jupyter` / `jupyterlab`

### Quick Start

1. Launch your Jupyter environment from the repository root:
   ```bash
   jupyter lab
   ```
2. Begin reading the foundational concepts in `conceptual/00_START_HERE.ipynb`.
3. Open `python/00_START_HERE.ipynb` alongside to execute the empirical coverage functions, belief filter updates, and state trajectory simulations.
