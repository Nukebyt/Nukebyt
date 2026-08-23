# Priyanuj Boruah

Electronics engineer (VLSI Design, VIT Chennai) working outward from silicon into the systems that sit on top of it - currently focused on **low-latency infrastructure, quantitative/financial engineering, and applied AI**, with **data analytics** as a recurring thread across all of it. GATE 2026 AIR 1626 (Instrumentation Engineering).

The common problem across these projects: something has to be fast, correct, and observable under real constraints - clock cycles, network round-trips, or a warehouse floor. VLSI is where I learned to think that way; the projects below are where I'm applying it.

---

## Currently building

**Low-latency systems & market microstructure**
Simulated exchange infrastructure in C++ — matching engine, order book, risk engine - with the hot path kept in-process and everything else (Kafka, Postgres, Redis, gRPC/REST/WebSocket APIs, Prometheus/Grafana) decoupled so it can fail independently. Benchmarks are measured against the running system, not estimated.

**Applied AI**
Local-first tooling - an offline meeting summarizer (Whisper + a local LLM, no cloud calls) and ML models compressed to run on a RISC-V microcontroller with 16 KB of SRAM. The constraint I keep choosing is "make it work without a GPU or an API key."

**Data analytics & BI**
SQL-first analytics work - star-schema warehouses, Tableau and Power BI dashboards, and a couple of forecasting/classification models (Prophet, Random Forest) layered on top for prediction rather than just reporting.

**VLSI & embedded systems** *(where this started)*
RTL design, FPGA pipelines, RISC-V, and the Reva Solar Racing team I led through a 20+ person build-and-compete cycle.

---

## Featured projects

### Low-latency & financial engineering
| Project | What it is | Stack |
|---|---|---|
| [low_latency_trading_infra](https://github.com/Nukebyt/low_latency_trading_infra) | Simulated distributed trading infrastructure — matching engine, order book, risk engine, Kafka streaming, chaos-tested for failure modes (a real 25s Redis failure-detection bug and a Postgres silent-data-loss bug were found and fixed, not hypothetical) | C++, Kafka, PostgreSQL, Redis, gRPC, Docker, Kubernetes, Prometheus/Grafana |

### Applied AI
| Project | What it is | Stack |
|---|---|---|
| [meeting_summarizer](https://github.com/Nukebyt/meeting_summarizer) | Fully offline meeting-to-transcript-to-action-items pipeline — no API keys, no cloud | Python, FastAPI, Streamlit, faster-whisper, Ollama (Llama 3.1) |
| [EdgeAI_RISCV](https://github.com/Nukebyt/EdgeAI_RISCV) | ML classifiers trained in Python, quantized to under 20 KB, and deployed on a SiFive FE310 RISC-V core with no FPU | Python, scikit-learn, C, SiFive Freedom Studio |
| [ML-Powered-Netlist-Partitioner](https://github.com/Nukebyt/ML-Powered-Netlist-Partitioner) | GNN-guided circuit partitioning — a graph neural net predicts better starting partitions for the Fiduccia–Mattheyses algorithm, cutting net-cut size 15–25% | Python, PyTorch Geometric, NetworkX, Streamlit |

### Data analytics & BI
| Project | What it is | Stack |
|---|---|---|
| [WarehouseIQ](https://github.com/Nukebyt/WarehouseIQ) | Warehouse ops analytics over 126K orders / $185M revenue — Power BI dashboard plus Prophet demand forecasting and a Random Forest model isolating the primary driver of dispatch delays | Python, Power BI, Prophet, scikit-learn, SQL |
| [IPL_Data_Analytics](https://github.com/Nukebyt/IPL_Data_Analytics) | Tableau dashboards on IPL ball-by-ball data — death-overs finishers, venue scoring patterns, toss advantage | SQL, Tableau |
| [food_delivery_analytics](https://github.com/Nukebyt/food_delivery_analytics) | Star-schema analysis of ~450K delivery orders — cancellation drivers, rider efficiency, demand peaks | MySQL, SQL, Tableau |

### VLSI, embedded & hardware *(foundation)*
| Project | What it is | Stack |
|---|---|---|
| [cfar-sar-ship-detection-fpga](https://github.com/Nukebyt/cfar-sar-ship-detection-fpga) | Pipelined 2D CFAR radar-detection datapath for maritime SAR ship detection, targeting a Cyclone IV FPGA | Verilog/SystemVerilog, MATLAB |
| [Quantum_RISC-Processor](https://github.com/Nukebyt/Quantum_RISC-Processor) | A RISC-V-inspired instruction set adapted for quantum hardware, with a qubit-aware scheduler and noise simulation | Python, Qiskit |
| [Reva-Solar-Racing](https://github.com/Nukebyt/Reva-Solar-Racing) | Founder & team captain — led a 20+ engineer team building a solar electric vehicle for competition | — |

---

## Stack

`C++` `Python` `TypeScript` `SQL` `Verilog / SystemVerilog`
`Kafka` `PostgreSQL` `Redis` `Docker` `Kubernetes`
`PyTorch` `scikit-learn` `Prophet`
`Tableau` `Power BI`

---

## Contact

- Email: [priyanuj.bx5@gmail.com](mailto:priyanuj.bx5@gmail.com)
- LinkedIn: [priyanuj-boruah](https://linkedin.com/in/priyanuj-boruah-997ba5231)
- Portfolio: _add your live site URL here_
