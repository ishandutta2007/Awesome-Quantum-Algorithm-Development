# Awesome-Quantum-Algorithm-Development

Here’s a clean, GitHub-style README.md focused primarily on open-source tools while keeping the two sections strictly separate, matching the format style used previously for similar lists.

Markdown
Copy
# Top Quantum Algorithm Development Tools

A curated list of leading platforms and frameworks for designing, optimizing, and executing quantum algorithms.  
**Primary focus: open-source software.**

Commercial / hosted platforms are listed separately for completeness. Open-source alternatives and community tools are emphasized throughout.

---

## SaaS / Hosted Platforms

| Platform | Description | Key Focus |
|----------|-------------|-----------|
| **[Classiq](https://www.classiq.io/)** | High-level quantum algorithm design platform. Users describe functional models; the synthesis engine automatically generates optimized circuits for multiple backends. | Algorithm synthesis, resource estimation, multi-hardware compilation |
| **[Zapata Orquestra](https://zapataquantum.com/)** | Unified platform for building, validating, and deploying hybrid quantum-classical applications. Includes use-case database, AI-assisted development, and QuantumOps tooling. | Enterprise application development & benchmarking |
| **[Q-CTRL](https://q-ctrl.com/)** (Fire Opal / Boulder Opal) | Infrastructure software for error suppression, automated performance optimization, and hardware control. Fire Opal provides turnkey error mitigation for algorithms. | Error suppression, control systems, algorithmic acceleration |
| **[QC Ware Forge / Promethium](https://www.qcware.com/)** | Enterprise quantum software platform with turnkey algorithms for optimization, ML, and chemistry. Promethium focuses on GPU-accelerated quantum chemistry. | Quantum ML, optimization, computational chemistry |
| **[Strangeworks](https://strangeworks.com/)** | Unified compute platform providing access to quantum hardware, simulators, and classical/quantum-inspired solvers through a single interface and Python SDK. | Multi-backend access, hybrid workflows |
| **[BlueQubit](https://www.bluequbit.io/)** | Cloud platform for high-performance simulation (CPU/GPU/MPS/Pauli-path) and access to leading QPUs (IBM, Quantinuum). Includes AI assistant for circuit design. | Large-scale simulation & quantum advantage experiments |
| **[Pasqal](https://www.pasqal.com/)** | Full-stack neutral-atom platform with cloud access, solvers for optimization/graph ML, and managed execution. | Neutral-atom algorithms, industrial optimization |
| **[IBM Qiskit Runtime](https://quantum.cloud.ibm.com/)** | Cloud-native execution service for Qiskit. Provides primitives (Sampler, Estimator), sessions, error mitigation, and efficient hybrid loops. | Production-grade execution on IBM hardware |
| **[D-Wave Leap](https://cloud.dwavesys.com/)** (with Ocean) | Cloud access to quantum annealers and hybrid solvers. Ocean SDK is the open-source companion. | Quantum annealing & hybrid optimization |
| **[Quantinuum InQuanto](https://www.quantinuum.com/products-solutions/inquanto)** | Proprietary quantum computational chemistry platform built on TKET. Tailored for molecular and materials simulations with industry collaborations. | Quantum chemistry on Quantinuum hardware |

---

## Open-Source Softwares

These tools form the core ecosystem for quantum algorithm research and development. Most integrate with multiple hardware backends and simulators.

### Core Frameworks & SDKs

| Project | Description | License | Notes |
|---------|-------------|---------|-------|
| **[Qiskit](https://github.com/Qiskit/qiskit)** | IBM’s full-stack open-source SDK. Circuit construction, transpilation, primitives, algorithms, and extensive ecosystem. | Apache 2.0 | Most widely used; pairs with Qiskit Runtime |
| **[Cirq](https://github.com/quantumlib/Cirq)** | Google’s framework for NISQ circuits. Strong hardware-aware design and integration with Google quantum processors. | Apache 2.0 | Excellent for research-level circuit manipulation |
| **[PennyLane](https://github.com/PennyLaneAI/pennylane)** | Differentiable programming for quantum ML, chemistry, and hybrid algorithms. Device-agnostic with automatic differentiation. | Apache 2.0 | Best-in-class for quantum machine learning |
| **[CUDA-Q](https://github.com/NVIDIA/cuda-quantum)** | NVIDIA’s open-source hybrid quantum-classical platform. Kernel-based model with GPU acceleration and multi-QPU support. | Apache 2.0 | High-performance simulation & GPU-QPU workflows |
| **[Ocean SDK](https://github.com/dwavesystems/dwave-ocean-sdk)** | D-Wave’s complete open-source suite for formulating and solving problems on quantum annealers and hybrid solvers. | Apache 2.0 | Industry standard for annealing |
| **[pytket / TKET](https://github.com/Quantinuum/tket)** | Quantinuum’s high-performance, hardware-agnostic quantum compiler and toolkit. Excellent circuit optimization and multi-backend support. | Apache 2.0 | Powers many commercial tools (including InQuanto) |
| **[Pulser](https://github.com/pasqal-io/Pulser)** | Pasqal’s open-source library for pulse-level / analog control of neutral-atom devices. Includes simulation via QuTiP. | Apache 2.0 | Primary interface for Pasqal hardware |
| **[Qadence](https://github.com/pasqal-io/qadence)** | Pasqal’s higher-level digital-analog programming interface, focused on quantum machine learning. | Apache 2.0 | Complements Pulser |

### Specialized Libraries

| Project | Description | Focus Area |
|---------|-------------|------------|
| **[OpenFermion](https://github.com/quantumlib/OpenFermion)** | Framework for compiling and analyzing quantum algorithms for electronic structure problems. | Quantum chemistry |
| **[QuTiP](https://github.com/qutip/qutip)** | Quantum Toolbox in Python – dynamics of open quantum systems, master equations, and pulse-level simulation. | Open-system dynamics & control |
| **[Qualtran](https://github.com/quantumlib/Qualtran)** | Google’s library for expressing and analyzing fault-tolerant quantum algorithms. | Fault-tolerant algorithm design |
| **[Stim](https://github.com/quantumlib/Stim)** | High-performance stabilizer circuit simulator and analysis tool. | Error correction & Clifford circuits |
| **[Qiskit Nature / Algorithms / Finance / etc.](https://github.com/Qiskit)** | Domain-specific application modules built on Qiskit. | Chemistry, optimization, ML, finance |
| **[PennyLane Lightning / Catalyst](https://github.com/PennyLaneAI)** | High-performance simulators and just-in-time compilation for PennyLane. | Accelerated hybrid workflows |
| **[MQT (Munich Quantum Toolkit)](https://github.com/munich-quantum-toolkit)** | Collection of design-automation tools for quantum computing (decision diagrams, ZX-calculus, benchmarking, etc.). | Compilation, verification, benchmarking |
| **[ffsim](https://github.com/Qiskit/ffsim)** | Specialized high-performance fermionic circuit simulator (IBM). | Quantum chemistry simulation |
| **[ProjectQ](https://github.com/ProjectQ-Framework/ProjectQ)** | Modular open-source framework with a focus on compilation and hardware backends. | General-purpose SDK |
| **[Qrisp](https://github.com/eclipse-qrisp/qrisp)** | High-level quantum programming language with automatic uncomputation and resource-efficient constructs. | Algorithm abstraction |

### Additional Notable Open-Source Tools

- **[qBraid SDK & tools](https://github.com/qBraid)** – Transpilation, QIR support, and unified environments.
- **[Bloqade](https://github.com/QuEraComputing/Bloqade)** – Analog programming for neutral-atom arrays (QuEra).
- **[Strawberry Fields](https://github.com/XanaduAI/strawberryfields)** – Photonic quantum computing (Xanadu).
- **[Q# + Quantum Development Kit](https://github.com/microsoft/qsharp)** – Microsoft’s quantum language and toolchain.
- **[Guppy](https://github.com/Quantinuum/guppylang)** – Quantinuum’s Pythonic quantum-classical language.
- **[Open Quantum Design (equilux)](https://github.com/OpenQuantumDesign)** – Full-stack open-source trapped-ion efforts.
- **[Quandary](https://github.com/llnl/quandary)** – Optimal control for open/closed quantum systems (LLNL).

---

## Quick Start Recommendations

| Goal | Recommended Starting Point |
|------|---------------------------|
| General algorithm development | **Qiskit** or **PennyLane** |
| Quantum machine learning | **PennyLane** |
| Chemistry / materials | **OpenFermion** + **Qiskit Nature** or **InQuanto** (commercial) + **TKET** |
| Neutral-atom / analog | **Pulser** + **Qadence** |
| Annealing / optimization | **Ocean SDK** |
| High-performance hybrid / GPU | **CUDA-Q** |
| Circuit optimization & multi-backend | **pytket** |
| Error suppression research | **Q-CTRL** tools (commercial) + open simulators |

---

## Contributing

Contributions, corrections, and new open-source projects are welcome.  
Please open an issue or pull request.

---

**Last updated:** August 2026  
Emphasizing open-source tools while documenting the major commercial platforms for context.

You can copy the entire block above into a file named README.md. It keeps SaaS/Hosted and Open-Source sections cleanly separated and prioritizes open-source coverage as requested.
