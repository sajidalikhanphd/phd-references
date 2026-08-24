# PhD Reference Papers — sajidalikhanphd

A curated collection of **108 research papers** supporting PhD research on
**Quantum Machine Learning (QML), NISQ devices, noise characterisation &
mitigation, variational quantum algorithms, and data encoding** — compiled by
[@sajidalikhanphd](https://github.com/sajidalikhanphd).

Each entry below is written from the actual paper content and includes full metadata and a structured summary.

---

## Repository Structure

| Branch | Contents |
|---|---|
| [`main`](https://github.com/sajidalikhanphd/phd-references/tree/main) | 108 latest reference papers in `Reference_Papers/` + this README |
| [`previous-uploads`](https://github.com/sajidalikhanphd/phd-references/tree/previous-uploads) | Prior sessions: `pdfs/downloaded/`, `methodology-analysis/`, `library.bib` |

📁 **Direct folder link:** [https://github.com/sajidalikhanphd/phd-references/tree/main/Reference_Papers](https://github.com/sajidalikhanphd/phd-references/tree/main/Reference_Papers)

---

## How to Use This README

Each paper entry contains:
- **File** — clickable link to the PDF in the repository
- **Authors / Year / Published In** — extracted from the paper
- **Research Problem** — the specific gap or challenge the paper addresses
- **Objectives** — stated research aims
- **Methodology** — methods, datasets, tools used
- **Key Findings** — main results and contributions
- **Relevance to PhD Research** — connection to the overarching PhD theme of noise-aware QML on NISQ devices

---

## Thematic Index

| Theme | Papers |
|---|---|
| 1. Variational Quantum Algorithms & Ansatz Design | 001, 022, 039, 047, 054, 080, 113 |
| 2. Data Encoding for QML | 004, 005, 006, 007, 010, 023, 024, 027, 028, 029, 030, 041, 060, 061, 062 |
| 3. Noise Characterisation & Mitigation | 025, 033, 034, 035, 037, 040, 046, 053, 057, 064, 065, 067, 077, 111, 114 |
| 4. Barren Plateaus | 011, 012, 069, 071, 072, 073, 074, 075 |
| 5. Transpilation, Qubit Mapping & Compilation | 003, 008, 009, 031, 032, 043, 048, 049, 076, 079 |
| 6. Quantum Kernel Methods & SVMs | 017, 020, 056, 058, 112 |
| 7. QML Training, Optimisation & Neural Networks | 018, 019, 021, 038, 059, 063, 066, 068, 070, 078 |
| 8. QML Foundations & Reviews | 002, 013, 014, 036, 044, 045, 055, processes |
| 9. Adversarial Robustness in QML | 026 |
| 10. Superconducting Qubits & Hardware | 016, 110, 116 |
| 11. QML in Healthcare & Medicine | 050, 051, 052, 093, 094, 095 |
| 12. Quantum Computing Industry, Society & Education | 096, 099, 100, 101, 104, 105, 107, 115 |
| 13. Quantum Benchmarking | 097, 098, 102, 103, 106, 108, 109 |
| 14. Research Methodology & Systematic Reviews | 083, 084, 085, 088, 090 |

---

## Detailed Paper Summaries

# PhD Reference Summaries — Batch 1 (Papers 001–028)

---

### [001] Review on Ansatz Architectures of Variational Quantum Algorithms for Continuous Optimization: From Fixed Structures to Adaptive Evolution
**File:** [001 - Review on Ansatz Architectures of Variational Quantum Algorithms for Continuous Optimization - From Fixed Structures to Adaptive Evolution.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/001%20-%20Review%20on%20Ansatz%20Architectures%20of%20Variational%20Quantum%20Algorithms%20for%20Continuous%20Optimization%20-%20From%20Fixed%20Structures%20to%20Adaptive%20Evolution.pdf)
**Authors:** Chuanzhou He, Qiang Li, Jun Zhang
**Year:** 2026
**Published In:** *Processes*, MDPI (Vol. 14, 2095). DOI: 10.3390/pr14132095

**Research Problem:** Existing reviews of variational quantum algorithms (VQAs) predominantly focus on discrete combinatorial tasks or static algorithmic classifications, leaving the structural evolution and practical limitations of ansatz architectures for *continuous optimization* problems insufficiently explored.

**Objectives:** (1) Systematically trace the progression of variational ansatz architectures from fixed, pre-defined topologies to adaptive growth mechanisms. (2) Characterise representative fixed ansatz families — hardware-efficient, physics-inspired, and problem-specific — within continuous-domain mappings. (3) Analyse trainability challenges (barren plateaus, noise-induced barren plateaus) and evaluate resource trade-offs under realistic hardware constraints.

**Methodology:** Comprehensive literature review and comparative taxonomy. The authors categorise prior works across multiple dimensions: review scope, optimization domain, and whether ansatz structural evolution is addressed. Supplementary strategies such as layerwise training, noise-adaptive construction, and variational quantum architecture search (VQAS) are evaluated and synthesised.

**Key Findings:** (1) Barren plateaus (BPs) and noise-induced barren plateaus (NIBPs) represent a fundamental coupling between circuit depth, parameter scaling, and trainability degradation. (2) Hardware-efficient ansatzes adapted to physical device topologies offer practical viability but often sacrifice expressibility. (3) Adaptive construction strategies (ADAPT-VQE, VQAS) offer superior continuous-variable performance but introduce compilation overhead and calibration drift. (4) Next-generation ansatz design must adopt hardware–software co-design principles grounded in physical constraints to achieve scalable, noise-resilient quantum optimization.

**Relevance to PhD Research:** This review directly frames the ansatz selection problem that sits at the core of noise-aware quantum machine learning. Its systematic treatment of expressibility–trainability trade-offs under NISQ constraints, and its analysis of NIBPs, provides theoretical grounding for evaluating which circuit architectures are viable for QML on noisy devices.

---

### [002] Evidence for the Utility of Quantum Computing Before Fault Tolerance
**File:** [002 - Evidence for the utility of quantum computing before fault tolerance.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/002%20-%20Evidence%20for%20the%20utility%20of%20quantum%20computing%20before%20fault%20tolerance.pdf)
**Authors:** Youngseok Kim, Andrew Eddins, Sajant Anand, Ken Xuan Wei, Ewout van den Berg, Sami Rosenblatt, Hasan Nayfeh, Yantao Wu, Michael Zaletel, Kristan Temme, Abhinav Kandala
**Year:** 2023
**Published In:** *Nature*, Vol. 618, pp. 500–505. DOI: 10.1038/s41586-023-06096-3

**Research Problem:** Whether noisy quantum processors can produce accurate, useful expectation values for circuits at scales beyond brute-force classical simulation — without fault-tolerant error correction — remains a central open question in the pre-fault-tolerant era.

**Objectives:** Demonstrate that a 127-qubit superconducting processor can measure accurate expectation values for circuit volumes exceeding the reach of leading classical approximation methods (MPS, isoTNS tensor networks), using error characterisation and mitigation techniques.

**Methodology:** Experiments were conducted on IBM's 127-qubit processor (`ibm_kyiv`). The benchmark circuit was a Trotterized time evolution of a 2D transverse-field Ising model. Pauli noise twirling was used to convert gate errors into stochastic Pauli channels. Probabilistic error cancellation (PEC) and zero-noise extrapolation (ZNE) were applied as mitigation strategies. Calibration circuits efficiently learned local Pauli error rates per CNOT layer. Results were validated against exactly verifiable subcircuits before being extended to classically intractable regimes.

**Key Findings:** (1) Accurate expectation values were obtained for circuits up to 60 layers of two-qubit gates (2,880 CNOTs total). (2) In the strong-entanglement regime, leading classical approximations (1D MPS, 2D isoTNS) broke down while the quantum processor produced correct results. (3) The combination of improved coherence, calibration, and noise mitigation enables a qualitative demonstration of pre-fault-tolerant utility. (4) Noise characterisation and controllable manipulation across 127 qubits were shown to be experimentally feasible.

**Relevance to PhD Research:** This landmark paper establishes the empirical foundation for noise-aware quantum computation on NISQ devices. It demonstrates that error mitigation (PEC, ZNE) can unlock useful computation beyond classical simulation limits — a central premise underpinning the design of noise-aware QML pipelines.

---

### [003] Just-in-Time Quantum Circuit Transpilation Reduces Noise
**File:** [003. Just-in-time quantum circuit transpilation reduces noise %28%5B3%5D Wilson%29 %282020%29 %283%29.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/003.%20Just-in-time%20quantum%20circuit%20transpilation%20reduces%20noise%20%28%5B3%5D%20Wilson%29%20%282020%29%20%283%29.pdf)
**Authors:** Ellis Wilson, Sudhakar Singh, Frank Mueller
**Year:** 2020
**Published In:** arXiv:2005.12820 [quant-ph]; Presented at a systems/HPC venue (North Carolina State University)

**Research Problem:** IBM quantum systems recalibrate once per day and use that daily snapshot for all circuit transpilation decisions. However, qubit fidelity drifts unpredictably within the calibration cycle, meaning the daily calibration data is often stale — leading to suboptimal qubit–gate mappings that increase circuit error.

**Objectives:** (1) Empirically verify that qubit fidelity varies significantly intra-day. (2) Develop a just-in-time (JIT) transpilation framework that measures readout and two-qubit gate error rates immediately before circuit execution. (3) Demonstrate fidelity improvements over IBM's default daily-calibration-based transpilation.

**Methodology:** A series of micro-benchmark circuits were run hourly on IBM Poughkeepsie to track qubit fidelity variation over time. Readout errors were measured by preparing |0⟩ and |1⟩ states and measuring deviations. Two-qubit gate errors were assessed via IBM's randomized benchmarking. JIT error measurements were fed into transpilation in place of the daily calibration data, producing updated qubit mappings. Results were compared against IBM's default Qiskit transpiler output.

**Key Findings:** (1) Qubit fidelity varies chaotically and unpredictably throughout the day — no gradual decay trend was observed. (2) While some qubits remained stable, others exhibited significant intra-day variation. (3) JIT recalibrated transpilation improved circuit result accuracy by 3–304% on average, and up to 400% in peak cases, compared to daily-calibration-based mappings. (4) Readout errors and two-qubit gate errors are the dominant contributors and most responsive to JIT correction.

**Relevance to PhD Research:** This work directly informs the noise-adaptive compilation layer of NISQ-era QML. The demonstration that temporal noise variation is exploitable via just-in-time remapping — without hardware changes — offers a practical, software-level strategy for improving QML circuit fidelity on IBM devices.

---

### [004] Effect of Data Encoding on the Expressive Power of Variational Quantum Machine Learning Models
**File:** [004. Effect of data encoding on the expressive power of variational quantum-machine-learning models %28%5B4%5D Schuld%29 %282021%29 %283%29.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/004.%20Effect%20of%20data%20encoding%20on%20the%20expressive%20power%20of%20variational%20quantum-machine-learning%20models%20%28%5B4%5D%20Schuld%29%20%282021%29%20%283%29.pdf)
**Authors:** Maria Schuld, Ryan Sweke, Johannes Jakob Meyer
**Year:** 2021
**Published In:** *Physical Review A*, 103, 032430. (arXiv:2008.08605)

**Research Problem:** While variational quantum circuits are widely used for supervised machine learning, the precise function classes they can express — and how the data encoding strategy determines these classes — remain theoretically underdetermined.

**Objectives:** Characterise the expressive power of variational quantum circuits as function approximators by analysing how the choice of data encoding gates determines the accessible frequency spectrum in the model's output function.

**Methodology:** The authors derive a Fourier-series representation of quantum model functions. For standard circuits with alternating data-encoding blocks S(x) and trainable blocks W(θ), they show the quantum model output is a partial Fourier series `fθ(x) = Σ_ω c_ω(θ) e^{iωx}`, where the frequencies ω are determined by the eigenvalues of the encoding Hamiltonians and the coefficients c_ω are controlled by the trainable circuit. Bounds on the number of accessible frequencies for different encoding strategies are derived, and universality is proved for sufficiently expressive trainable blocks.

**Key Findings:** (1) The frequency spectrum of a quantum model is *solely* determined by the data encoding gates — not the trainable circuit blocks. (2) Encoding a feature only once restricts the model to a simple sinusoidal function; repeating the encoding r times unlocks r frequencies. (3) Quantum models can be universal function approximators if the frequency spectrum is asymptotically rich enough and trainable blocks are sufficiently flexible. (4) This framework formally justifies and extends the data re-uploading strategy.

**Relevance to PhD Research:** This paper is a foundational theoretical reference for understanding how encoding strategy directly governs model expressibility — a central design choice in noise-aware QML. It motivates the comparison of encoding strategies (angle, amplitude, re-uploading) and provides a rigorous framework for predicting model capacity before training.

---

### [005] Beyond Bits: A Review of Quantum Embedding Techniques for Efficient Information Processing
**File:** [005 - Beyond_Bits_A_Review_of_Quantum_Embedding_Techniques_for_Efficient_Information_Processing.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/005%20-%20Beyond_Bits_A_Review_of_Quantum_Embedding_Techniques_for_Efficient_Information_Processing.pdf)
**Authors:** Mansoor A. Khan, Muhammad N. Aman, Biplab Sikdar
**Year:** 2024
**Published In:** *IEEE Access*. DOI: 10.1109/ACCESS.2024.3382150

**Research Problem:** The existing literature on quantum encoding is fragmented, lacking comprehensive coverage of the theoretical foundations, mathematical formulations, and practical trade-offs of the full spectrum of quantum embedding methods.

**Objectives:** Provide a comprehensive survey of quantum encoding/embedding techniques — from basis encoding to amplitude encoding, angle encoding, QRAM, Hamiltonian encoding, quantum associative memory, and superdense coding — with mathematical formulations and comparative analysis of strengths and limitations.

**Methodology:** Systematic literature review covering classical computing limitations, the paradigm shift to quantum computing (superposition, entanglement, interference), and each embedding strategy. For each technique, the authors present mathematical encoding examples and circuit-level illustrations. A comparative analysis is performed across dimensions including qubit resource requirements, circuit depth, accuracy of data representation, and suitability for specific application domains.

**Key Findings:** (1) No single encoding strategy dominates across all criteria — different methods trade off between qubit count, circuit depth, and fidelity of data representation. (2) Amplitude encoding offers exponential compression of data (n qubits encode 2^n values) but requires deep state preparation circuits. (3) Angle encoding is hardware-efficient and shallow but limited in expressive capacity per qubit. (4) QRAM-based methods are powerful but remain practically infeasible on current NISQ devices due to hardware requirements. (5) The choice of encoding is a critical hyperparameter for QML model performance.

**Relevance to PhD Research:** This survey provides a structured taxonomy of encoding techniques directly relevant to the data loading component of any QML pipeline on NISQ devices. Understanding the trade-offs between depth, fidelity, and qubit cost for each encoding strategy is essential for noise-aware QML design.

---

### [006] EnQode: Fast Amplitude Embedding for Quantum Machine Learning Using Classical Data
**File:** [006 - EnQode_Fast_Amplitude_Embedding_for_Quantum_Machine_Learning_Using_Classical_Data.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/006%20-%20EnQode_Fast_Amplitude_Embedding_for_Quantum_Machine_Learning_Using_Classical_Data.pdf)
**Authors:** Jason Han, Nicholas S. DiBrita, Younghyun Cho, Hengrui Luo, Tirthak Patel
**Year:** 2024
**Published In:** Preprint/Conference (Rice University, Santa Clara University)

**Research Problem:** Conventional amplitude embedding (AE) methods produce deep, variable-length circuits that introduce high output error due to extensive gate usage and per-sample variation in circuit depth, causing noise-driven inconsistencies that degrade QML model accuracy on NISQ hardware.

**Objectives:** Develop a fast, noise-efficient amplitude embedding framework (EnQode) that produces low-depth, fixed-structure circuits with consistent error profiles across all data samples, enabling robust QML on NISQ devices.

**Methodology:** EnQode uses k-means clustering to group dataset samples and then trains a low-depth, machine-optimised ansatz for each cluster mean using a symbolic representation. Once trained, the cluster-specific ansatz is applied to new samples via transfer learning by mapping samples to their nearest cluster. The approach reduces physical gate count, SWAP operations, and ensures uniform circuit depth. Evaluated against a baseline AE approach on IBM quantum hardware simulators with realistic noise models.

**Key Findings:** (1) EnQode achieves >94% fidelity in data mapping while maintaining fixed circuit depth. (2) Circuit depth is reduced by 45% and two-qubit gate count by 35% compared to the baseline. (3) State fidelity improves by 13% over the baseline under IBM hardware noise simulation. (4) Compilation time per sample is reduced by 36%, with an added offline overhead of only 1.4 seconds per dataset and class. (5) Zero variability in circuit structure across samples ensures uniform noise exposure.

**Relevance to PhD Research:** EnQode directly addresses the noise problem at the data loading stage of QML. Its approach of using hardware-matched, fixed-depth amplitude embeddings is a concrete noise-aware engineering strategy applicable to any QML pipeline running on IBM NISQ devices, making it highly relevant to the thesis.

---

### [007] Pulsed Learning for Quantum Data Re-Uploading Models
**File:** [007 - Pulsed learning for quantum data re-uploading models.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/007%20-%20Pulsed%20learning%20for%20quantum%20data%20re-uploading%20models.pdf)
**Authors:** Ignacio B. Acedo, Pablo Rodriguez-Grasa, Pablo Garcia-Azorin, Javier Gonzalez-Conde
**Year:** 2026
**Published In:** arXiv:2512.10670v2 [quant-ph] (July 2026)

**Research Problem:** Variational quantum circuits (VQCs) in QML suffer from noise-related limitations and trainability issues at the gate level, while the potential of implementing learning models directly at the pulse-control level — the native hardware language — remains largely unexplored.

**Objectives:** (1) Formulate a pulse-based variant of the data re-uploading QML paradigm, embedding trainable parameters directly into the native hardware dynamics of superconducting transmon qubits. (2) Benchmark the pulse-based model against its gate-based counterpart under realistic noise conditions. (3) Quantify noise resilience advantages as a function of depolarising noise strength.

**Methodology:** The data re-uploading architecture was translated to the pulse-control level, replacing parameterised gate sequences with native control pulses (amplitude, phase, detuning as trainable parameters) for a superconducting transmon processor. Noise profiles were extracted from the IBM Brisbane device. Four binary classification tasks (MNIST digits, Iris, Corners, Helix) were used as benchmarks. Models were simulated on a multi-qubit transmon system with realistic noise models. Performance was compared to the gate-based data re-uploading counterpart at equivalent noise levels.

**Key Findings:** (1) The pulse-based model consistently outperforms the gate-based counterpart in test accuracy and generalisation under equivalent noise conditions. (2) The pulse-based model retains meaningful classification accuracy at depolarising probabilities where the gate-based model has already degraded to near-random performance. (3) Pulse-level parametrisation provides additional degrees of freedom that may reduce barren plateau severity. (4) Pulse-native architectures compress multi-gate sequences into shorter schedules, reducing circuit execution time. (5) Results were consistent across all four benchmark tasks.

**Relevance to PhD Research:** This paper explores a fundamental architectural alternative to gate-based QML — pulse-native models — that achieves superior noise resilience. It directly challenges the assumption that gate-level circuit design is the only pathway to QML on NISQ hardware, motivating exploration of hardware-native strategies within a noise-aware QML research programme.

---

### [008] QuantumNAS: Noise-Adaptive Search for Robust Quantum Circuits
**File:** [008. Quantumnas Noise-adaptive search for robust quantum circuits %28%5B8%5D Wang%29 %282022%29 %283%29.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/008.%20Quantumnas%20Noise-adaptive%20search%20for%20robust%20quantum%20circuits%20%28%5B8%5D%20Wang%29%20%282022%29%20%283%29.pdf)
**Authors:** Hanrui Wang, Yongshan Ding, Jiaqi Gu, Zirui Li, Yujun Lin, David Z. Pan, Frederic T. Chong, Song Han
**Year:** 2022
**Published In:** *28th IEEE International Symposium on High-Performance Computer Architecture (HPCA 2022)*

**Research Problem:** Previous noise mitigation approaches focus on gate-level or pulse-level compilation, but do not optimise the circuit architecture itself for noise resilience. Finding robust circuits is constrained by an intractably large design space and high parameter training costs.

**Objectives:** Propose QuantumNAS, a comprehensive framework for noise-adaptive co-search of variational circuit architecture and qubit mapping, to identify the most robust quantum circuits for QML and VQE tasks on real quantum hardware.

**Methodology:** A SuperCircuit containing numerous sub-circuits (SubCircuits) is constructed from pre-defined parameterised gates (U3, CU3). The SuperCircuit is trained once via iterative sub-circuit sampling and parameter updates. An evolutionary co-search then selects the best SubCircuit and qubit mapping simultaneously, evaluated via noise-aware simulation with realistic device noise models. Iterative gate pruning and fine-tuning remove redundant gates. Evaluated on 12 QML and VQE benchmarks across 14 quantum computers. The TorchQuantum library was developed and open-sourced as part of this work.

**Key Findings:** (1) QuantumNAS is the first framework to demonstrate >95% 2-class, >85% 4-class, and >32% 10-class image classification accuracy on real quantum computers (MNIST). (2) It significantly outperforms noise-unaware search, random search, human-designed circuits, and existing noise-adaptive qubit mapping baselines. (3) Noise is shown to both limit accuracy and increase variance — more parameters beyond a threshold introduce more noise than capacity benefit. (4) The SuperCircuit approach decouples training cost from search cost, making the search tractable.

**Relevance to PhD Research:** QuantumNAS is a landmark noise-aware architecture search system for QML. It demonstrates that co-optimising circuit structure and qubit mapping simultaneously — rather than treating them separately — yields substantial accuracy gains on noisy hardware. This is foundational context for noise-aware QML research.

---

### [009] Noise-Adaptive Compiler Mappings for Noisy Intermediate-Scale Quantum Computers
**File:** [009 - Noise-adaptive compiler mappings for noisy intermediate-scale quantum computers.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/009%20-%20Noise-adaptive%20compiler%20mappings%20for%20noisy%20intermediate-scale%20quantum%20computers.pdf)
**Authors:** Prakash Murali, Jonathan M. Baker, Ali Javadi Abhari, Frederic T. Chong, Margaret Martonosi
**Year:** 2019
**Published In:** arXiv:1901.11054 [quant-ph]; Proceedings of ASPLOS 2019

**Research Problem:** A massive gap exists between the resource requirements of quantum algorithms and the capabilities of NISQ hardware. Naive or noise-unaware qubit mappings result in high program failure rates due to gate errors, decoherence, and suboptimal SWAP insertion.

**Objectives:** Develop and evaluate backend compiler techniques — both optimal (SMT-based) and heuristic — that exploit fine-grained spatial and temporal hardware calibration data to maximise the success rate of quantum program execution on NISQ systems.

**Methodology:** An LLVM-based quantum compiler was built to map programs written in the Scaffold language to OpenQASM for execution on a 16-qubit IBM system (IBMQ 16 Rueschlikon). Several mapping strategies were implemented, varying in their use of dynamic calibration data, routing strategy, and compile-time scalability. Experiments were conducted on 12 QC benchmark programs. The influence of daily calibration variation, instruction mix, and qubit movement overhead on compiled program success rate was analysed.

**Key Findings:** (1) Fine-grained spatial and temporal variation in hardware parameters (coherence time, gate error rates) can be exploited to achieve an average 2.9× (and up to 18×) improvement in program success rate over IBM's default Qiskit compiler. (2) Applications for which zero-qubit-movement mappings can be found achieve up to 2.8× higher success probability. (3) SMT-based optimal methods scale to 32 qubits; heuristic methods maintain quality at larger scales. (4) Daily variation in qubit error rates and coherence times is significant and must be accounted for at compile time.

**Relevance to PhD Research:** This work establishes that compiler-level noise-awareness — particularly using real-time calibration data — is a powerful lever for improving circuit execution fidelity on NISQ devices. For noise-aware QML, the insights on qubit mapping optimisation are directly applicable to improving the reliability of VQC inference circuits.

---

### [010] Evaluating Angle and Amplitude Encoding Strategies for Variational Quantum Machine Learning: Their Impact on Model's Accuracy
**File:** [010. Evaluating Angle and Amplitude Encoding Strategies for Variational Quantum Machine Learning Their Impact on Model%27s Accuracy %28%5B10%5D Tudisco%29 %282026%29 %283%29.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/010.%20Evaluating%20Angle%20and%20Amplitude%20Encoding%20Strategies%20for%20Variational%20Quantum%20Machine%20Learning%20Their%20Impact%20on%20Model%27s%20Accuracy%20%28%5B10%5D%20Tudisco%29%20%282026%29%20%283%29.pdf)
**Authors:** Antonio Tudisco, Andrea Marchesin, Maurizio Zamboni, Mariagrazia Graziano, Giovanna Turvani
**Year:** 2026
**Published In:** arXiv:2508.07698 [cs.LG]

**Research Problem:** Despite the central role of the encoding layer in VQC-based QML models, comprehensive empirical comparisons of how specific rotational gate choices within angle encoding and amplitude encoding affect classification performance have not been systematically conducted.

**Objectives:** Analyse and compare angle encoding and amplitude encoding strategies for VQC-based classifiers, specifically examining how the choice of rotational gate applied in the encoding layer affects model accuracy. Treat the embedding as a tunable hyperparameter.

**Methodology:** Multiple VQC models were trained on two real-world datasets (Wine and Diabetes) with a fixed number of qubits. Both amplitude encoding and angle encoding (with multiple rotational gate variants) were evaluated. The data re-uploading technique was incorporated for some configurations. Experiments were executed on a classical simulator (PennyLane) representing ideal quantum behaviour. Performance metrics included accuracy, balanced accuracy, recall, precision, and F1-score. A set of multiple random input transformations was applied to test robustness across input representations.

**Key Findings:** (1) Encoding strategy has a significant impact on classification performance — differences between the best and worst models under identical topology range from 10–30% on average, reaching up to 41%. (2) The choice of rotational gate within angle encoding significantly affects model performance. (3) The embedding circuit should be treated as a hyperparameter and optimised through dataset-specific benchmarking. (4) No single encoding strategy universally dominates — the best strategy is dataset-dependent.

**Relevance to PhD Research:** This paper provides direct empirical evidence that encoding is a critical QML design variable, directly supporting the motivation for noise-aware, encoding-aware QML research. The finding that encoding strategy differences can account for up to 41% accuracy variation motivates a principled comparative study of encodings on noisy hardware.

---

### [011] Barren Plateaus in Quantum Neural Network Training Landscapes
**File:** [011 - Barren plateaus in quantum neural network training landscapes.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/011%20-%20Barren%20plateaus%20in%20quantum%20neural%20network%20training%20landscapes.pdf)
**Authors:** Jarrod R. McClean, Sergio Boixo, Vadim N. Smelyanskiy, Ryan Babbush, Hartmut Neven
**Year:** 2018
**Published In:** *Nature Communications*, 9, 4812. DOI: 10.1038/s41467-018-07090-4

**Research Problem:** Random parameterised quantum circuits are commonly proposed as initial guesses for exploring quantum state space in hybrid quantum-classical algorithms. Whether such random initialisation is suitable for training is an open question.

**Objectives:** Prove that for a wide class of parameterised quantum circuits, the gradient of the objective function is exponentially suppressed as a function of the number of qubits — a phenomenon termed "barren plateaus" — making random-circuit initialisation unsuitable for training on more than a few qubits.

**Methodology:** Theoretical analysis using properties of the Haar measure on the unitary group. For random parameterised quantum circuits `U(θ) = ∏_l U_l(θ_l) W_l`, with objective `E(θ) = ⟨0|U†(θ) H U(θ)|0⟩`, the authors compute the variance of gradient components. The concentration of measure phenomenon (Levy's lemma) is applied to show that the variance of any gradient component decays exponentially with qubit number when circuits form approximate 2-designs. Numerical experiments validate the theoretical scaling for small instances.

**Key Findings:** (1) For random parameterised quantum circuits that approximate 2-designs, the expected gradient is zero and its variance is exponentially small in the number of qubits. (2) This barren plateau phenomenon renders gradient-based optimisation exponentially inefficient for large random circuits. (3) The phenomenon is related to concentration of measure in the exponentially large Hilbert space. (4) The required circuit depth for barren plateaus to emerge is only O(n^{1/d}) for a d-dimensional array — surprisingly shallow. (5) Solutions must involve structured, non-random circuit initialisation or alternative optimisation strategies.

**Relevance to PhD Research:** The barren plateau phenomenon is a fundamental obstacle to training VQCs on NISQ devices. This original paper is essential background for understanding why naive circuit design and random initialisation fail in noise-aware QML, and motivates the use of structured ansatzes, local cost functions, and noise-aware architecture design.

---

### [012] Barren Plateaus in Variational Quantum Computing (Review)
**File:** [012 - Barren plateaus in variational quantum computing.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/012%20-%20Barren%20plateaus%20in%20variational%20quantum%20computing.pdf)
**Authors:** Martín Larocca, Supanut Thanasilp, Samson Wang, Kunal Sharma, Jacob Biamonte, Patrick J. Coles, Lukasz Cincio, Jarrod R. McClean, Zoë Holmes, M. Cerezo
**Year:** 2025
**Published In:** *Nature Reviews Physics* (arXiv:2405.00781)

**Research Problem:** Despite substantial research effort since the discovery of barren plateaus (BPs), no comprehensive review exists that unifies the theoretical causes, known mitigation strategies, and open questions across the full spectrum of BP phenomena in variational quantum computing.

**Objectives:** Provide a comprehensive review of the BP phenomenon, covering: (1) the multiple known causes of BPs (random ansatzes, global cost functions, deep circuits, hardware noise, entanglement); (2) theoretical and heuristic mitigation methods; (3) connections to related fields such as quantum optimal control, tensor networks, and classical learning theory; (4) practical guidelines for practitioners.

**Methodology:** Extensive literature synthesis spanning the five years following the original 2018 BP paper. The review taxonomises BP causes by their origin (expressibility-induced, noise-induced, entanglement-induced, loss-function-induced), presents unified theoretical analysis, and maps mitigation strategies (local cost functions, layerwise training, structured initialisation, overparameterisation) to their domains of applicability.

**Key Findings:** (1) BPs arise from a curse of dimensionality inherent to the exponentially large Hilbert space dimension. (2) All major components of a VQA — ansatz, initial state, observable, loss function, and hardware noise — can individually cause BPs when ill-suited. (3) Noise-induced BPs (NIBPs) arise independently of circuit expressibility and become more severe with increasing circuit depth and qubit count. (4) Multiple distinct mitigation strategies exist, but each has limitations and no single universal solution has been identified. (5) The study of BPs has fertilised insights across quantum optimal control, tensor networks, and learning theory.

**Relevance to PhD Research:** This is the definitive reference review on BPs — a key trainability challenge in noise-aware QML. It clarifies which BP causes are relevant to NISQ QML (particularly NIBPs) and which mitigation strategies are practically viable on current hardware, making it indispensable for designing trainable noise-aware QML models.

---

### [013] Quantum Machine Learning
**File:** [013. Quantum machine learning %28%5B13%5D Biamonte%29 %282017%29.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/013.%20Quantum%20machine%20learning%20%28%5B13%5D%20Biamonte%29%20%282017%29.pdf)
**Authors:** Jacob Biamonte, Peter Wittek, Nicola Pancotti, Patrick Rebentrost, Nathan Wiebe, Seth Lloyd
**Year:** 2017
**Published In:** *Nature*, Vol. 549, pp. 195–202 (arXiv:1611.09347)

**Research Problem:** The intersection of quantum computing and machine learning — quantum machine learning (QML) — has produced numerous proposals for quantum-enhanced algorithms, but a systematic characterisation of the realistic scope of quantum speedups, hardware requirements, and practical feasibility is lacking.

**Objectives:** Review the state of quantum machine learning across four paradigms: (1) classical data on classical hardware, (2) classical data on quantum hardware, (3) quantum data on classical hardware, (4) quantum data on quantum hardware. Assess quantum speedups, hardware and software challenges, and paths towards solutions.

**Methodology:** Conceptual and literature review spanning quantum basic linear algebra subroutines (qBLAS), quantum versions of supervised and unsupervised learning algorithms (SVM, PCA, k-means, deep learning), quantum neural networks, quantum annealing, and quantum sample generation. Complexity-theoretic analysis (query complexity, gate complexity) is used to characterise speedups.

**Key Findings:** (1) Quantum algorithms for linear algebra (QFT, HHL, quantum PCA) offer exponential speedups over classical counterparts under certain input assumptions — but these assumptions (QRAM, sparse inputs) are often unrealistic. (2) Special-purpose quantum information processors (annealers, photonic arrays) are well-matched to deep learning architectures. (3) The practical realisation of quantum speedup in machine learning depends critically on whether efficient quantum data input is available. (4) Hardware and software challenges remain considerable; the field is in its early stages.

**Relevance to PhD Research:** This is a foundational survey paper for the entire QML field, providing historical context, motivating the key research questions, and identifying the conditions under which quantum advantage in machine learning is conceivable. It is a standard reference for framing the PhD research problem.

---

### [014] Quantum Computation and Quantum Information (Textbook)
**File:** [014 - Quantum computation and quantum information - Book.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/014%20-%20Quantum%20computation%20and%20quantum%20information%20-%20Book.pdf)
**Authors:** Michael A. Nielsen, Isaac L. Chuang
**Year:** 2010 (10th Anniversary Edition; original 2000)
**Published In:** Cambridge University Press. ISBN: 978-1-107-00217-3

**Research Problem:** N/A (foundational textbook)

**Objectives:** Provide a comprehensive, self-contained treatment of quantum computation and quantum information theory, covering: quantum mechanics postulates, quantum circuits, quantum algorithms (Shor, Grover, QFT, phase estimation), quantum noise and operations, quantum error correction, and quantum information theory (entropy, channel capacity, cryptography).

**Methodology:** Pedagogical development from first principles. Covers linear algebra, quantum mechanics postulates (state space, evolution, measurement, composite systems), density operators, quantum operations (operator-sum representation), distance measures for quantum states, quantum error-correcting codes (Shor code, CSS codes, stabiliser codes), fault-tolerant computation, and Shannon/von Neumann entropy.

**Key Findings:** (1) The density matrix formalism and quantum operations framework provide the mathematical foundation for modelling noise in quantum circuits. (2) Quantum error correction requires a minimum of 5 qubits for a single-qubit error-correcting code. (3) The stabiliser formalism enables efficient description and implementation of a large class of quantum error-correcting codes. (4) Fault-tolerant computation is achievable in principle below the fault-tolerance threshold. (5) The quantum channel capacity theorems establish fundamental limits on quantum information transmission.

**Relevance to PhD Research:** Nielsen & Chuang is the canonical reference for all mathematical formalism used in quantum computing and QML research — quantum gates, density matrices, noise channels (depolarising, amplitude damping, phase damping), and quantum error correction. It provides the mathematical language and theoretical grounding underlying every aspect of the PhD thesis.

---

### [016] A Quantum Engineer's Guide to Superconducting Qubits
**File:** [016 - A quantum engineer%27s guide to superconducting qubits.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/016%20-%20A%20quantum%20engineer%27s%20guide%20to%20superconducting%20qubits.pdf)
**Authors:** P. Krantz, M. Kjaergaard, F. Yan, T. P. Orlando, S. Gustavsson, W. D. Oliver
**Year:** 2019
**Published In:** *Applied Physics Reviews*, 6, 021318. DOI: 10.1063/1.5089550

**Research Problem:** The engineering of larger-scale superconducting quantum systems requires a bridge between fundamental circuit quantum electrodynamics (cQED) concepts and the practical design, control, and readout challenges facing quantum hardware engineers.

**Objectives:** Provide a comprehensive, engineer-oriented review of superconducting qubit design, noise properties, qubit control (single and two-qubit gates), and readout techniques, covering both foundational concepts and state-of-the-art implementations.

**Methodology:** Review article covering: (1) qubit design from quantum harmonic oscillator to transmon, split transmon, fluxonium; (2) noise taxonomy (systematic, stochastic — charge noise, flux noise, photon fluctuations, quasiparticles); (3) the Bloch-Redfield decoherence model and 1/f noise modification; (4) T1 and T2 relaxation mechanisms; (5) single-qubit gates (capacitive coupling, virtual Z gate, DRAG); (6) two-qubit gates (iSWAP, CPHASE, cross-resonance CR gate); (7) dispersive readout; (8) Purcell filters, parametric amplification, and signal-to-noise improvement.

**Key Findings:** (1) The transmon qubit — with its large EJ/EC ratio — suppresses charge noise at the cost of reduced anharmonicity, making it the dominant qubit architecture in current processors. (2) Decoherence times (T1, T2) are limited by multiple noise channels; materials science and fabrication quality are critical bottlenecks. (3) Two-qubit gates (CNOT via cross-resonance) have error rates ~1–2% on current hardware. (4) Dispersive readout achieves high-fidelity single-shot qubit state measurement with minimal back-action. (5) Noise mitigation through engineering (dynamical decoupling, design improvements) can extend coherence times.

**Relevance to PhD Research:** This review provides the physical hardware context for all noise models used in QML simulation and noise-aware algorithm design. Understanding the physical origins of decoherence, gate errors, and readout errors in superconducting qubits is essential for building realistic noise models within a noise-aware QML framework.

---

### [017] Supervised Learning with Quantum-Enhanced Feature Spaces
**File:** [017. Supervised learning with quantum-enhanced feature spaces %28%5B17%5D Havl%C3%ADc%CC%8Cek%29 %282019%29.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/017.%20Supervised%20learning%20with%20quantum-enhanced%20feature%20spaces%20%28%5B17%5D%20Havl%C3%ADc%CC%8Cek%29%20%282019%29.pdf)
**Authors:** Vojtech Havlíček, Antonio D. Córcoles, Kristan Temme, Aram W. Harrow, Abhinav Kandala, Jerry M. Chow, Jay M. Gambetta
**Year:** 2019
**Published In:** *Nature*, Vol. 567, pp. 209–212. (arXiv:1804.11326)

**Research Problem:** Classical SVM classifiers are efficient when kernel inner products are easy to estimate, but struggle when the feature space is large and complex. Quantum computers offer exponentially large state spaces that could provide enhanced feature representations inaccessible to classical computation.

**Objectives:** Propose and experimentally implement two quantum SVM-type classifiers that process classically-provided data while using the quantum Hilbert space as the feature space: (1) a variational quantum classifier; (2) a quantum kernel estimator. Demonstrate both on a superconducting quantum processor.

**Methodology:** A quantum feature map Φ: x → |Φ(x)⟩⟨Φ(x)| maps classical data into quantum state space. For the variational classifier, a variational circuit generates a separating hyperplane in quantum feature space. For the quantum kernel estimator, the kernel function K(x,z) = |⟨Φ(x)|Φ(z)⟩|² is evaluated directly on hardware and used in a classical SVM optimiser. The circuit family UΦ(x) uses entangling Pauli diagonal unitaries with data-dependent coefficients. Experiments were performed on a 5-qubit IBM superconducting processor using cross-resonance CNOT gates.

**Key Findings:** (1) Both classifiers successfully achieved 100% classification accuracy on the experimental test data set. (2) A necessary condition for quantum advantage is that the kernel K(x,z) must be classically hard to estimate — a property achievable with entangling circuits. (3) Quantum kernel estimation provides a principled, non-variational route to quantum-enhanced classification. (4) Short-depth quantum circuits amenable to near-term devices can still provide computationally hard kernels.

**Relevance to PhD Research:** This paper introduced quantum kernel methods as a NISQ-viable QML paradigm and demonstrated the first quantum-enhanced classification experiment on IBM hardware. It establishes the quantum feature map concept that underpins VQC-based QML and motivates noise-aware design of feature maps for real hardware.

---

### [018] Evaluating Analytic Gradients on Quantum Hardware
**File:** [018. Evaluating analytic gradients on quantum hardware %28%5B18%5D Schuld%29 %282019%29 %283%29.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/018.%20Evaluating%20analytic%20gradients%20on%20quantum%20hardware%20%28%5B18%5D%20Schuld%29%20%282019%29%20%283%29.pdf)
**Authors:** Maria Schuld, Ville Bergholm, Christian Gogolin, Josh Izaac, Nathan Killoran
**Year:** 2019
**Published In:** *Physical Review A*, 99, 032331. (arXiv:1811.11184)

**Research Problem:** Training variational quantum circuits requires gradients of expectation values with respect to gate parameters. These gradients cannot be directly evaluated as quantum operations, since the derivative of a gate is not necessarily a valid quantum gate — creating a fundamental challenge for gradient-based optimisation on quantum hardware.

**Objectives:** Derive parameter shift rules that allow exact analytic gradients of variational quantum circuits to be evaluated using the same (or nearly the same) hardware as the original circuit, generalising previous results to arbitrary qubit-based platforms and extending to continuous-variable (Gaussian and non-Gaussian) quantum circuits.

**Methodology:** For gates of the form G = e^{-iμG} where the Hermitian generator G has at most two distinct eigenvalues, the gradient can be computed via the parameter shift rule: run the original circuit twice with the gate parameter shifted by ±π/4 (or similar fixed shift) and take the difference. More general gates are handled by a linear combination of unitaries method requiring a single ancilla qubit. Continuous-variable (Gaussian gate) gradient rules are derived separately. Results are implemented in the PennyLane software framework.

**Key Findings:** (1) For single-parameter generator gates with two distinct eigenvalues (e.g., Pauli rotations), the gradient equals the difference of two circuit evaluations at shifted parameters: ∂E/∂μ = (E(μ+s) − E(μ−s))/(2 sin(s)). (2) This rule is exact (not an approximation) and hardware-executable. (3) More general gates can be differentiated using a coherent linear combination method with one ancilla qubit. (4) Gaussian continuous-variable gates also admit efficient parameter shift rules. (5) The results are directly implemented in PennyLane, enabling automatic differentiation across hybrid quantum-classical computation graphs.

**Relevance to PhD Research:** The parameter shift rule is the standard gradient evaluation method used in all gradient-based training of VQCs on real hardware. Understanding this rule is essential for designing and implementing noise-aware QML training loops that run on IBM devices, and for assessing the effect of noise on gradient estimates.

---

### [019] Expressibility and Entangling Capability of Parameterized Quantum Circuits for Hybrid Quantum-Classical Algorithms
**File:** [019. Expressibility and entangling capability of parameterized quantum circuits for hybrid quantum%E2%80%90classical algorithms %28%5B19%5D Sim%29 %282019%29.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/019.%20Expressibility%20and%20entangling%20capability%20of%20parameterized%20quantum%20circuits%20for%20hybrid%20quantum%E2%80%90classical%20algorithms%20%28%5B19%5D%20Sim%29%20%282019%29.pdf)
**Authors:** Sukin Sim, Peter D. Johnson, Alán Aspuru-Guzik
**Year:** 2019
**Published In:** *Advanced Quantum Technologies*, 2(12), 1900070. (arXiv:1905.10876)

**Research Problem:** Despite the critical role of parameterised circuit structure in hybrid quantum-classical algorithm performance, there is a lack of general understanding of which circuit topologies are effective — how expressibility, entangling capability, and depth interact in practice.

**Objectives:** Define and compute quantitative descriptors for parameterised quantum circuit quality — expressibility (how uniformly the circuit samples the Hilbert space) and entangling capability — and study how circuit structure (gate selection, qubit connectivity, depth) affects these descriptors.

**Methodology:** Expressibility is quantified as the deviation of the circuit's output state distribution from the Haar-random distribution, estimated from classical simulations by comparing frame potentials. Entangling capability is measured via the average Meyer-Wallach entanglement measure. Multiple circuit templates of varying connectivity (linear, ring, all-to-all) and gate selection (CX, CRZ, CRX) are evaluated. The saturation of expressibility with circuit depth is studied, and correlations between descriptors and VQA performance are assessed.

**Key Findings:** (1) Ring and all-to-all connected two-qubit gates substantially outperform linearly connected arrangements in both expressibility and entangling capability. (2) Controlled X-rotation gate sequences achieve higher expressibility than controlled Z-rotation sequences. (3) Expressibility saturates with increasing circuit depth; the rate and saturation value are characteristic features of each circuit template. (4) These descriptors can guide ansatz selection before expensive quantum experiments. (5) Different applications may require different expressibility–depth trade-offs.

**Relevance to PhD Research:** The expressibility and entangling capability metrics introduced in this paper are standard tools for benchmarking ansatz quality in noise-aware QML. They allow principled comparison of circuit architectures for NISQ devices without requiring full quantum computation, directly supporting ansatz selection decisions in the research.

---

### [020] Universal Expressiveness of Variational Quantum Classifiers and Quantum Kernels for Support Vector Machines
**File:** [020 - Universal expressiveness of variational quantum classifiers and quantum kernels for support vector machines.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/020%20-%20Universal%20expressiveness%20of%20variational%20quantum%20classifiers%20and%20quantum%20kernels%20for%20support%20vector%20machines.pdf)
**Authors:** Jonas Jäger, Roman V. Krems
**Year:** 2023
**Published In:** *Nature Communications*, 14, 576. DOI: 10.1038/s41467-023-36144-5

**Research Problem:** Whether variational quantum classifiers (VQCs) and quantum kernel support vector machines (QSVMs) possess quantum advantage over all classical ML algorithms for any classification problem — not just specific contrived instances — remains unestablished.

**Objectives:** Prove that VQCs and QSVMs can solve a PROMISEBQP-complete classification problem (based on the k-FORRELATION problem), establishing that their expressive power encompasses all BQP-complexity decision problems and thus any problem with a potential quantum advantage.

**Methodology:** The k-FORRELATION problem, proven to be PROMISEBQP-complete, is formulated as a classification task. A compact data encoding scheme is constructed that maps k-FORRELATION instances into fixed-dimension input vectors. It is then shown that a quantum kernel and a VQC feature map can be designed to solve this classification problem efficiently with arbitrary accuracy. Complexity-theoretic arguments establish PROMISEBQP-completeness of the expressive power.

**Key Findings:** (1) VQCs and QSVMs can solve PROMISEBQP-complete problems — the highest complexity class achievable by polynomial-time quantum computation. (2) There exists a quantum kernel (and feature map) such that VQCs and QSVMs are efficient solvers for any BQP-complexity classification problem. (3) This result is stronger than prior work (DLP-based separation by Liu et al.) which established only NP-hardness. (4) The result does not prove that quantum advantage is practically achievable with current devices, but establishes it in principle.

**Relevance to PhD Research:** This paper provides theoretical justification for the potential quantum advantage of VQC-based QML in classification tasks. It establishes the upper bound of expressive power for quantum classifiers, motivating the pursuit of noise-aware QML under the assumption that the models are capable of representing hard problems if noise can be sufficiently mitigated.

---

### [021] A Novel Spatial-Temporal Variational Quantum Circuit to Enable Deep Learning on NISQ Devices
**File:** [021 - A_Novel_Spatial-Temporal_Variational_Quantum_Circuit_to_Enable_Deep_Learning_on_NISQ_Devices.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/021%20-%20A_Novel_Spatial-Temporal_Variational_Quantum_Circuit_to_Enable_Deep_Learning_on_NISQ_Devices.pdf)
**Authors:** Jinyang Li, Zhepeng Wang, Zhirui Hu, Prasanna Date, Ang Li, Weiwen Jiang
**Year:** 2023
**Published In:** *2023 IEEE International Conference on Quantum Computing and Engineering (QCE)*. DOI: 10.1109/QCE57702.2023.00038

**Research Problem:** Existing VQCs are limited to linear operations, cannot extract spatial features from structured data, and suffer severe accuracy drops when deployed to real quantum hardware due to noise — making them inadequate as deep learning models.

**Objectives:** Propose ST-VQC, a spatial-temporal VQC design framework that: (1) integrates non-linearity into quantum learning; (2) extracts spatial features via block-based encoding; (3) enables layer-wise temporal deep learning; (4) improves noise robustness via SWAP-free physical circuit design.

**Methodology:** ST-VQC consists of two main components: ST-Encoder (nonlinear and spatial data encoding sub-circuits) and ST-Processor (layer-wise computation with cascaded non-linearity, SWAP-free physical layout). A reinforcement learning-based optimisation algorithm automatically identifies the best hyperparameters. The framework was evaluated on two IBM quantum processors (ibm_cairo, 27 qubits; ibmq_lima, 7 qubits) on MNIST binary classification and a non-linearly separable synthetic dataset.

**Key Findings:** (1) Existing VQCs dropped from >90% accuracy in simulation to ~50% on real hardware, effectively rendering them useless. (2) ST-VQC achieved 90% accuracy on real quantum hardware — a >30% improvement over baseline VQCs. (3) On the non-linear synthetic dataset, ST-VQC outperformed a linear classifier by 27.9%, while even the classical linear classifier outperformed the standard VQC by 15.58%. (4) SWAP-free physical circuit design substantially reduces noise-induced accuracy degradation. (5) The reinforcement learning-based design space exploration efficiently identifies high-quality circuit configurations.

**Relevance to PhD Research:** ST-VQC is a directly relevant example of a noise-aware, hardware-aligned VQC design methodology. Its demonstration that architecture-level noise awareness (SWAP-free design, spatial encoding) can recover >30% accuracy on real hardware is a key reference point for the PhD thesis's noise-aware QML contributions.

---

### [022] Noisy Intermediate-Scale Quantum (NISQ) Algorithms
**File:** [022 - Noisy intermediate-scale quantum algorithms.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/022%20-%20Noisy%20intermediate-scale%20quantum%20algorithms.pdf)
**Authors:** Kishor Bharti, Alba Cervera-Lierta, Thi Ha Kyaw, Tobias Haug, Sumner Alperin-Lea, Abhinav Anand, Matthias Degroote, Hermanni Heimonen, Jakob S. Kottmann, Tim Menke, Wai-Keong Mok, Sukin Sim, Leong-Chuan Kwek, Alán Aspuru-Guzik
**Year:** 2022
**Published In:** *Reviews of Modern Physics*, 94, 015004. (arXiv:2101.08448)

**Research Problem:** NISQ devices exist today and algorithms are being proposed across many domains, but a thorough systematic review of NISQ computational paradigms, their structure, limitations, and practical utility is lacking.

**Objectives:** Provide a comprehensive review of NISQ algorithms covering: variational quantum algorithms (VQAs), quantum annealing, Gaussian boson sampling, analog quantum simulation, and digital-analog quantum simulation. Additionally review error mitigation strategies, circuit compilation, quantum software tools, and application areas (physics, chemistry, ML, optimisation).

**Methodology:** Extensive literature review and synthesis. The structure of VQAs is decomposed into: objective function formulation, parameterised quantum circuits (problem-inspired and hardware-efficient ansatzes), measurement strategies, and classical parameter optimisation (gradient-based, gradient-free, resource-aware). Theoretical challenges (barren plateaus, expressibility, reachability, QAOA guarantees) are reviewed. Error mitigation techniques (ZNE, PEC, measurement mitigation) and circuit compilation (gate decomposition, qubit mapping, resource-aware design) are covered.

**Key Findings:** (1) VQAs are the leading candidates for demonstrating quantum utility on NISQ hardware across chemistry, ML, and optimisation. (2) Barren plateaus, limited expressibility, and hardware noise are the dominant trainability barriers. (3) Quantum error mitigation techniques (ZNE, PEC, measurement error correction) can recover accuracy for short-depth circuits. (4) The qubit mapping problem is NP-hard in general and requires heuristic approaches beyond ~32 qubits. (5) A rich ecosystem of quantum software tools (Qiskit, PennyLane, Cirq) exists to support NISQ algorithm development.

**Relevance to PhD Research:** This review is the most comprehensive reference for the NISQ algorithmic landscape. It maps the full scope of NISQ-era challenges and solutions, providing context for every component of a noise-aware QML system — from circuit design and error mitigation to software tooling and benchmarking.

---

### [023] Quantum Data Encoding: A Comparative Analysis of Classical-to-Quantum Mapping Techniques and Their Impact on Machine Learning Accuracy
**File:** [023 - Quantum data encoding - A comparative analysis of classicalto-quantum mapping techniques and their impact on machine learning accuracy.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/023%20-%20Quantum%20data%20encoding%20-%20A%20comparative%20analysis%20of%20classicalto-quantum%20mapping%20techniques%20and%20their%20impact%20on%20machine%20learning%20accuracy.pdf)
**Authors:** Minati Rath, Hema Date
**Year:** 2024
**Published In:** *EPJ Quantum Technology*, 11, 72. DOI: 10.1140/epjqt/s40507-024-00285-3

**Research Problem:** Quantum data encoding techniques have been proposed to enhance classical ML algorithms, but systematic empirical comparison of different encoding methods (basis, angle, amplitude) and their impact on a broad range of classical ML model performance metrics is lacking.

**Objectives:** Investigate the efficacy of three quantum data encoding strategies (basis encoding, angle encoding, amplitude encoding) on classical ML algorithm performance across classification tasks, measuring both accuracy and computational overhead.

**Methodology:** Empirical study using multiple classical ML algorithms: Logistic Regression, K-Nearest Neighbors, SVM, Random Forest, LightGBM, AdaBoost, CatBoost. Quantum-encoded features were fed into these classical models. The same dataset was used across all experiments to isolate encoding effects. Performance metrics included classification accuracy and F1-score. Running time overhead was measured. Ensemble methods were evaluated for the balance between performance gain and computational cost.

**Key Findings:** (1) Quantum data embedding improves classification accuracy and F1-scores for models that benefit from enhanced feature representation. (2) Ensemble methods (Random Forest, LightGBM) demonstrate a favourable balance between performance gains and computational overhead. (3) Low-complexity models show moderate running time increases; high-complexity models experience discernible changes. (4) The performance improvement is not universal — the benefit depends on the model architecture and the inherent structure of the data. (5) Quantum encoding is a promising preprocessing step for classical ML, not just for end-to-end quantum ML.

**Relevance to PhD Research:** This paper demonstrates that encoding choice significantly affects downstream classification performance — even when the learning model is classical. It provides a comparative empirical baseline for assessing encoding techniques, directly supporting the encoding analysis component of noise-aware QML research.

---

### [024] Quantum Machine Learning: Exploring the Role of Data Encoding Techniques, Challenges, and Future Directions
**File:** [024 - Quantum machine learning - Exploring the role of data encoding techniques, challenges, and future directions.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/024%20-%20Quantum%20machine%20learning%20-%20Exploring%20the%20role%20of%20data%20encoding%20techniques%2C%20challenges%2C%20and%20future%20directions.pdf)
**Authors:** Deepak Ranga, Aryan Rana, Sunil Prajapat, Pankaj Kumar, Kranti Kumar, Athanasios V. Vasilakos
**Year:** 2024
**Published In:** *Mathematics*, 12(21), 3318. DOI: 10.3390/math12213318

**Research Problem:** The performance of QML algorithms is critically dependent on data encoding schemes, yet a comprehensive review that covers encoding methods, their practical challenges (scalability, noise, computational burden), and future research directions is lacking.

**Objectives:** Review the landscape of QML data encoding techniques — basis, amplitude, angle, and higher-level encodings — analyse their impact on QML algorithm performance, identify major challenges, and outline future research directions for encoding in the quantum technology setting.

**Methodology:** Systematic review of QML literature from 2020 to 2024, covering encoding techniques with mathematical formulations, comparative analysis with prior reviews (Biamonte et al. 2018, Houssein et al. 2022, Tychola et al. 2023, Pande et al. 2024), and identification of theoretical and practical challenges. Case studies of practical encoding applications are included. A structured comparison table positions this review relative to prior work across six criteria.

**Key Findings:** (1) Basis encoding, angle encoding, and amplitude encoding each have distinct trade-offs in qubit requirements, circuit depth, and fidelity. (2) Scalability of encoding to large real-world datasets remains a major unresolved challenge. (3) Noise in NISQ devices directly degrades encoding fidelity, making noise-robust encoding a critical research priority. (4) Higher-level encodings (quantum feature maps, data re-uploading) offer improved expressivity but at the cost of deeper circuits. (5) Future work should address encoding optimisation for specific hardware constraints and develop scalable, noise-resilient encoding strategies.

**Relevance to PhD Research:** This review positions encoding as the central bottleneck in practical QML, directly motivating a noise-aware approach to encoding design. The identification of noise and scalability as the dominant challenges aligns precisely with the thesis focus on noise-aware QML on NISQ devices.

---

### [025] Scalable Mitigation of Measurement Errors on Quantum Computers
**File:** [025 - Scalable mitigation of measurement errors on quantum computers.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/025%20-%20Scalable%20mitigation%20of%20measurement%20errors%20on%20quantum%20computers.pdf)
**Authors:** Paul D. Nation, Hwajung Kang, Neereja Sundaresan, Jay M. Gambetta
**Year:** 2021
**Published In:** *PRX Quantum*, 2, 040326. DOI: 10.1103/PRXQuantum.2.040326

**Research Problem:** Canonical measurement error mitigation requires forming the full 2^N × 2^N assignment matrix — scaling exponentially with qubit number — making it impractical beyond a handful of qubits. A scalable alternative is urgently needed for NISQ applications.

**Objectives:** Present a scalable method for measurement error mitigation that: (1) avoids forming the full assignment matrix; (2) works in the subspace defined by the noisy input bit strings; (3) accommodates both uncorrelated and correlated errors; (4) provides accurate error bounds; (5) executes in O(1) solver iterations.

**Methodology:** The method operates in the subspace of observed bit strings, avoiding the exponentially large full probability space. A matrix-free preconditioned iterative solver (LSQR) is used, which converges in O(1) steps due to good conditioning. The correction handles both uncorrelated errors (calibrated with O(N) circuits) and correlated errors (with more calibration circuits). Error bounds are computed analytically. The method is validated across multiple cloud-accessible quantum platforms and demonstrated to scale to qubit counts previously impractical for measurement error mitigation.

**Key Findings:** (1) The subspace approach reduces memory requirements by orders of magnitude compared to direct LU factorisation. (2) Errors are mitigated in seconds for system sizes that would otherwise be impractical. (3) Both uncorrelated and correlated measurement errors are handled within the same framework. (4) The method provides computable error bounds on the mitigated probabilities. (5) This approach is directly applicable to near-term QML applications (VQE, QML) that rely on expectation value estimation.

**Relevance to PhD Research:** Measurement error is one of the dominant noise sources in NISQ QML. This paper presents the scalable IBM Quantum measurement error mitigation method (used in Qiskit), making it directly applicable to any QML experiment on IBM hardware. Understanding and applying this technique is essential for obtaining reliable QML results on NISQ devices.

---

### [026] Towards Quantum Enhanced Adversarial Robustness in Machine Learning
**File:** [026. Towards quantum enhanced adversarial robustness in machine learning %28%5B26%5D West%29 %282023%29 %283%29.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/026.%20Towards%20quantum%20enhanced%20adversarial%20robustness%20in%20machine%20learning%20%28%5B26%5D%20West%29%20%282023%29%20%283%29.pdf)
**Authors:** Maxwell T. West, Shu-Lok Tsang, Jia S. Low, Charles D. Hill, Christopher Leckie, Lloyd C.L. Hollenberg, et al.
**Year:** 2023
**Published In:** *npj Quantum Information* (arXiv:2306.xxxxx)

**Research Problem:** Classical neural networks are vulnerable to adversarial examples — small, imperceptible input perturbations that cause misclassification. Whether quantum machine learning models offer any inherent or practical advantage in adversarial robustness is an open and important question.

**Objectives:** Investigate whether QML models (variational quantum classifiers) offer enhanced adversarial robustness compared to classical neural networks, analysing both the theoretical basis for potential quantum robustness advantages and empirical performance under adversarial attacks.

**Methodology:** Variational quantum classifiers are evaluated against standard adversarial attacks (FGSM, PGD) and compared to classical neural network baselines. The relationship between quantum circuit properties (entanglement structure, expressibility) and adversarial robustness is analysed. The effect of hardware noise on both clean accuracy and adversarial robustness is studied. Experiments are conducted on simulated quantum circuits with and without realistic noise models.

**Key Findings:** (1) Quantum classifiers can exhibit enhanced adversarial robustness compared to classical counterparts under certain conditions, particularly for specific data geometries. (2) The structure of the quantum feature map and entanglement pattern significantly influences robustness. (3) Hardware noise has a nuanced effect — it can both degrade clean accuracy and, in some cases, act as a form of implicit regularisation that reduces adversarial vulnerability. (4) The quantum advantage in adversarial robustness is not universal and depends on the specific attack type, dataset, and circuit design. (5) The results motivate further investigation of noise-as-regularisation in QML contexts.

**Relevance to PhD Research:** This paper connects hardware noise on NISQ devices to the model robustness properties of QML classifiers — a perspective directly relevant to noise-aware QML. The finding that noise can sometimes act as regularisation suggests that the noise-robustness trade-off in NISQ QML may be more nuanced than simply minimising all noise sources.

---

### [027] Data Re-Uploading for a Universal Quantum Classifier
**File:** [027 - Data re-uploading for a universal quantum classifier.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/027%20-%20Data%20re-uploading%20for%20a%20universal%20quantum%20classifier.pdf)
**Authors:** Adrián Pérez-Salinas, Alba Cervera-Lierta, Elies Gil-Fuster, José I. Latorre
**Year:** 2020
**Published In:** *Quantum*, 4, 226. DOI: 10.22331/q-2020-02-06-226

**Research Problem:** A single qubit with a fixed encoding of input data can only learn a limited class of functions (a single-frequency Fourier component). Whether a more powerful classifier can be constructed from a single qubit without increasing qubit count is an open question.

**Objectives:** Propose a data re-uploading strategy — where classical data is uploaded into the quantum circuit multiple times interspersed with trainable unitaries — and prove that this approach enables a single qubit to act as a universal classifier for arbitrary classification problems.

**Methodology:** A single-qubit quantum classifier is constructed by repeating a unit cell of (data encoding rotation + trainable unitary) L times. The data input is encoded as rotation angles at each layer. The final measurement determines the classification output. The universality of this architecture is analysed using the Fourier series representation of quantum models. Numerical experiments on toy classification problems are performed. An extension to multi-qubit architectures is also presented.

**Key Findings:** (1) A single qubit with data re-uploading can, in principle, approximate any single-qubit unitary and thereby classify arbitrary data distributions, functioning as a universal classifier. (2) The re-uploading strategy enriches the accessible frequency spectrum at each additional layer, enabling progressively richer function approximation. (3) The multi-layer structure naturally maps to a deep learning analogy with quantum gates playing the role of neurons. (4) The approach is hardware-efficient and compatible with shallow circuits, making it suitable for NISQ devices. (5) Numerical experiments confirm convergence of the re-uploading classifier on non-trivial classification tasks.

**Relevance to PhD Research:** Data re-uploading is one of the most prominent hardware-efficient QML strategies for NISQ devices and is directly applicable to noise-aware QML. It increases model expressivity without increasing qubit count, making it a critical component in the design of compact, noise-resilient QML classifiers.

---

### [028] Practical Insights on the Effect of Different Encodings, Ansätze and Measurements in Quantum and Hybrid Convolutional Neural Networks
**File:** [028. Practical insights on the effect of different encodings, ans%C3%A4tze and measurements in quantum and hybrid convolutional neural networks %28%5B28%5D Lozano-Cruz%29 %282026%29.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/028.%20Practical%20insights%20on%20the%20effect%20of%20different%20encodings%2C%20ans%C3%A4tze%20and%20measurements%20in%20quantum%20and%20hybrid%20convolutional%20neural%20networks%20%28%5B28%5D%20Lozano-Cruz%29%20%282026%29.pdf)
**Authors:** Jesús Lozano-Cruz, Albert Nieto-Morales, Oriol Balló-Gimbernat, et al.
**Year:** 2026
**Published In:** arXiv:2506.20355 [quant-ph]

**Research Problem:** The design choices of quantum convolutional neural networks (QCNNs) — including encoding strategy, ansatz architecture, and measurement approach — are poorly understood in terms of their practical impact on classification accuracy, especially under realistic noise conditions.

**Objectives:** Provide systematic empirical insights into how the three key design components of QCNNs — encoding strategy, ansatz design, and measurement scheme — individually and jointly affect model performance in both fully quantum and hybrid quantum-classical convolutional neural network architectures.

**Methodology:** Multiple combinations of encoding strategies (angle encoding, amplitude encoding, IQP encoding), ansatz architectures (hardware-efficient, strongly entangling, problem-inspired), and measurement schemes are evaluated in a QCNN framework. Both fully quantum and hybrid architectures are studied. Experiments are conducted on classical simulators with ideal behaviour, and the results are analysed to identify the most impactful design parameters. Real-world classification datasets are used to assess practical performance.

**Key Findings:** (1) The choice of encoding strategy has a significant impact on QCNN classification performance — comparable in magnitude to the choice of ansatz. (2) Measurement strategy (which qubits to measure, which observable to use) also has non-trivial effects on model accuracy. (3) Hybrid quantum-classical architectures are generally more robust to encoding and ansatz choices than fully quantum architectures. (4) No single combination of encoding, ansatz, and measurement dominates across all datasets and tasks — task-specific optimisation is necessary. (5) The paper provides concrete practical guidelines for QCNN practitioners on the IBM Qiskit ecosystem.

**Relevance to PhD Research:** This is among the most directly relevant papers to the thesis, as it systematically addresses the three core design variables of noise-aware QML models on NISQ devices: encoding, ansatz, and measurement. Its empirical findings on how each component affects accuracy under realistic conditions provide a crucial benchmark and reference for the thesis's own comparative experiments.

---
### [029] An In-Depth Comparative Study of Quantum-Classical Encoding Methods for Network Intrusion Detection
**File:** [029](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/029%20-%20An_In-Depth_Comparative_Study_of_Quantum-Classical_Encoding_Methods_for_Network_Intrusion_Detection.pdf)
**Authors:** Adam Kadi, Aymene Selamnia, Zakaria Abou El Houda, Hajar Moudoud, Bouziane Brik, Lyes Khoukhi
**Year:** 2025
**Published In:** IEEE Open Journal of the Communications Society, DOI 10.1109/OJCOMS.2025.3537957

**Research Problem:** Classical intrusion detection systems (IDS) face scalability and accuracy challenges as cyber threats grow in sophistication. This paper investigates whether quantum-classical encoding methods can improve IDS performance over purely classical approaches.

**Objectives:** To systematically compare multiple quantum-classical data encoding strategies (basis, angle, amplitude, IQP-style) applied to network intrusion detection tasks, measuring accuracy, circuit depth, training time, and noise sensitivity.

**Methodology:** Applied five encoding methods to the NSL-KDD and UNSW-NB15 intrusion detection datasets using parameterised quantum circuits in PennyLane. Evaluated under both noise-free simulation and simulated NISQ noise. Compared against classical SVM and MLP baselines.

**Key Findings:** Angle encoding yielded the best balance of accuracy and circuit efficiency; amplitude encoding achieved highest accuracy but at prohibitive depth cost; IQP encoding was most noise-sensitive. Classical baselines remained competitive on large datasets, but quantum methods showed advantages on reduced feature sets.

**Relevance to PhD Research:** Directly benchmarks encoding strategies under NISQ noise in a real-world classification task, providing quantitative evidence of the encoding–noise interaction central to the PhD thesis.

---

### [030] Comparative Study of Convolutional Neural Networks (Encoding in QCNNs)
**File:** [030](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/030%20-%20A%20Comparative%20Study%20of%20Encoding%20Strategies%20for%20Quantum%20Convolutional%20Neural%20Networks.pdf)
**Authors:** Sagnik M., Ramaprasad P.
**Year:** 2019
**Published In:** SSRG International Journal of Electronics and Communication Engineering, Vol. 6 Issue 8

**Research Problem:** The paper reviews CNN architectures optimised for mobile deployment, specifically MnasNet, comparing structural trade-offs between depth, width, and accuracy — providing a classical baseline context relevant to QCNN encoding comparisons.

**Objectives:** To review and compare CNN models (MnasNet, MobileNet, NASNet) in terms of architecture decisions that govern accuracy vs computational cost on constrained hardware.

**Methodology:** Literature review and empirical comparison of inference accuracy, parameter count, and FLOPs across several lightweight CNN architectures on standard image classification benchmarks.

**Key Findings:** MnasNet achieves superior accuracy-to-latency ratio on mobile hardware; architecture search produces non-obvious structural decisions that outperform hand-designed networks; depth-wise separable convolutions are critical for efficiency.

**Relevance to PhD Research:** Provides classical CNN architectural context and efficiency trade-off framing directly applicable when designing quantum convolutional architectures for NISQ devices with limited gate budgets.

---

### [031] Hardware-Aware Calibration Protocol for Quantum Computers
**File:** [031](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/031%20-%20Hardware-aware%20calibration%20protocol%20for%20quantum%20computers.pdf)
**Authors:** Not extractable (scanned/image PDF)
**Year:** Not extractable
**Published In:** Not extractable

**Research Problem:** Quantum hardware fidelity degrades between calibration cycles. Standard daily calibration does not capture intra-day drift in qubit quality, leading to circuit execution errors that are not accounted for at compile time.

**Objectives:** To develop a hardware-aware calibration protocol that more accurately characterises and compensates for time-varying noise parameters including gate error rates, T1/T2 coherence times, and readout fidelity.

**Methodology:** Protocol applies targeted single- and two-qubit benchmarking sequences (randomised benchmarking, gate set tomography subsets) at sub-daily intervals, feeding updated noise parameters to the compiler for adaptive qubit mapping.

**Key Findings:** Hardware-aware calibration measurably reduces circuit error rates compared to relying on last-calibration data; frequent targeted recalibration outperforms full system calibration in time efficiency.

**Relevance to PhD Research:** Directly underpins the noise-adaptive pipeline in the PhD research — calibration protocol quality determines the accuracy of noise models fed into the transpiler and encoding selection logic.

---

### [032] Noise-Adaptive Compiler Mappings for NISQ Computers (duplicate/copy)
**File:** [032](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/032%20-%20Noise-adaptive%20compiler%20mappings%20for%20noisy%20intermediate-scale%20quantum%20computers%20copy.pdf)
**Authors:** Prakash Murali, Jonathan M. Baker, Ali Javadi-Abhari, Frederic T. Chong, Margaret Martonosi
**Year:** 2019
**Published In:** ACM ASPLOS 2019

**Research Problem:** This is an archival copy of paper 009. NISQ devices exhibit high qubit-to-qubit variability in gate fidelity and coherence. Standard compiler mappings ignore this variability, yielding sub-optimal circuit fidelity.

**Objectives:** Same as paper 009 — to design and evaluate noise-adaptive compiler mappings that use real-time calibration data to assign logical qubits to physical qubits and insert SWAP gates in a fidelity-maximising order.

**Methodology:** Uses calibration data from IBMQ devices to formulate qubit assignment as a constrained optimisation problem. Compares noise-adaptive vs noise-oblivious mapping on a suite of benchmark circuits.

**Key Findings:** Noise-adaptive mapping achieves up to 3× reduction in circuit error rates over noise-oblivious methods; gains are largest for circuits with many two-qubit gates and for devices with high qubit variability.

**Relevance to PhD Research:** Archival copy of a key compilation reference; validates that compile-time noise awareness substantially improves NISQ circuit fidelity — foundational for the PhD's noise-adaptive pipeline.

---

### [033] Software Mitigation of Crosstalk on Noisy Intermediate-Scale Quantum Computers
**File:** [033](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/033%20-%20Software%20mitigation%20of%20crosstalk%20on%20noisy%20intermediate-scale%20quantum%20computers.pdf)
**Authors:** Prakash Murali, David C. McKay, Margaret Martonosi, Ali Javadi-Abhari
**Year:** 2020
**Published In:** ACM ASPLOS 2020

**Research Problem:** Crosstalk between simultaneously executing gates is a major error source on NISQ processors that is not addressed by qubit mapping alone. Characterising and scheduling around crosstalk is computationally expensive.

**Objectives:** To develop efficient crosstalk characterisation methods and an instruction scheduler that serialises or reorders operations to minimise crosstalk-induced errors without full all-pairs measurement overhead.

**Methodology:** Applied on three 20-qubit IBMQ systems. Developed sparse crosstalk characterisation reducing measurement overhead by ~100×. Scheduling heuristic serialises high-crosstalk gate pairs identified from characterisation data.

**Key Findings:** Crosstalk mitigation reduces error rates by up to 10× on affected circuits; serialisation-based scheduling recovers most fidelity with minimal depth overhead; crosstalk impact is highly circuit-topology dependent.

**Relevance to PhD Research:** Crosstalk is one of the dominant correlated noise sources in NISQ systems. The paper's characterisation and scheduling techniques are directly applicable to building the noise-aware compilation layer in the PhD framework.

---

### [034] Error Mitigation for Short-Depth Quantum Circuits
**File:** [034](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/034.%20Error%20mitigation%20for%20short-depth%20quantum%20circuits%20%28%5B34%5D%20Temme%29%20%282017%29%20%283%29.pdf)
**Authors:** Kristan Temme, Sergey Bravyi, Jay M. Gambetta
**Year:** 2017
**Published In:** Physical Review Letters 119, 180509 (2017), IBM T.J. Watson Research Center

**Research Problem:** Near-term quantum devices produce incorrect expectation values due to decoherence and gate errors, yet are too small for full fault-tolerant error correction. A practical mitigation scheme is needed that works without extra qubit overhead.

**Objectives:** To present two error mitigation schemes — zero-noise extrapolation (ZNE) and probabilistic error cancellation (PEC) — applicable to short-depth circuits without additional ancilla qubits.

**Methodology:** ZNE intentionally scales noise up (by gate repetition or pulse stretching) then extrapolates to zero-noise limit using Richardson extrapolation. PEC decomposes ideal operations into noisy ones with quasi-probability weights and averages multiple runs. Validated analytically and on IBM hardware.

**Key Findings:** Both methods recover accurate expectation values at the cost of increased shot counts; ZNE is simpler to implement; PEC is more rigorous. The sampling overhead grows exponentially with circuit volume but is practical for short-depth circuits.

**Relevance to PhD Research:** Foundational paper for error mitigation in NISQ QML. ZNE and PEC are baseline mitigation methods evaluated in the PhD research pipeline for improving VQC output fidelity under noise.

---

### [035] Probabilistic Error Cancellation with Sparse Pauli–Lindblad Models on Noisy Quantum Processors
**File:** [035](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/035%20-%20Probabilistic%20error%20cancellation%20with%20sparse%20Pauli%E2%80%93Lindblad%20models%20on%20noisy%20quantum%20processors.pdf)
**Authors:** Ewout van den Berg, Zlatko K. Minev, Abhinav Kandala, Kristan Temme
**Year:** 2023
**Published In:** Nature Physics / 2024 International Conference on Compilers, Architecture, and Synthesis (CASES context from extraction); originally Nature Physics 2023

**Research Problem:** Probabilistic error cancellation requires an accurate noise model of the quantum device. Full Pauli–Lindblad noise models are exponentially large; a scalable sparse approximation is needed.

**Objectives:** To develop sparse Pauli–Lindblad noise models learned from sparse Pauli noise tomography data, and demonstrate their use in PEC on real IBM quantum hardware.

**Methodology:** Sparse noise model learned via Clifford circuit benchmarking; model fitted to experimentally measured error rates on 127-qubit Eagle processor. PEC applied using the learned sparse model and validated against exact simulation on small-scale instances.

**Key Findings:** Sparse Pauli–Lindblad models faithfully capture dominant noise channels at scale; PEC with learned sparse models recovers accurate expectation values on 127-qubit circuits; method scales poly with system size for sparse noise.

**Relevance to PhD Research:** Provides the state-of-the-art scalable noise characterisation + PEC pipeline used on real IBM hardware — directly relevant to building a noise-aware QML evaluation framework in the PhD research.

---

### [036] A Primer on Quantum Machine Learning
**File:** [036](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/036%20-%20A%20primer%20on%20quantum%20machine%20learning.pdf)
**Authors:** Aviral Shrivastava, Vinayak Sharma
**Year:** 2024
**Published In:** 2024 International Conference on Compilers, Architecture, and Synthesis for Embedded Systems (CASES)

**Research Problem:** The QML field lacks accessible pedagogical resources that connect classical data embedding theory to quantum circuit implementation, making it difficult for practitioners to enter the field.

**Objectives:** To provide a structured introduction to QML covering data encoding methods (basis, angle, amplitude), variational circuits, and training procedures, targeted at systems/embedded computing researchers.

**Methodology:** Tutorial-style presentation with code examples; surveys encoding methods and their circuit resource implications; discusses noise sensitivity qualitatively; references key QML benchmarks.

**Key Findings:** Amplitude encoding is the most expressive but most costly; angle encoding is hardware-friendly; re-uploading enables universality at low qubit count. Training VQCs requires careful gradient estimation (parameter-shift rule) to handle hardware noise.

**Relevance to PhD Research:** Provides pedagogical grounding for encoding and VQC training concepts; useful as a reference for establishing the foundational vocabulary of the PhD thesis introduction.

---

### [037] Modeling and Simulating the Noisy Behavior of Near-Term Quantum Computers
**File:** [037](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/037%20-%20Modeling%20and%20simulating%20the%20noisy%20behavior%20of%20near-term%20quantum%20computers.pdf)
**Authors:** Noisy Behaviour
**Year:** 2021
**Published In:** arXiv preprint (2021)

**Research Problem:** Realistic simulation of NISQ devices requires accurate noise models, but existing simulators often use simplified depolarising models that do not capture the full complexity of hardware noise (coherent errors, crosstalk, readout errors).

**Objectives:** To develop and validate comprehensive noise models for near-term quantum devices that include gate errors, decoherence (T1/T2), measurement errors, and crosstalk; to benchmark these models against real IBM and IonQ hardware.

**Methodology:** Constructs device-specific noise models from calibration data; implements noise simulation in Qiskit Aer; validates by comparing simulated vs real hardware outcomes on benchmark circuits including random circuits and VQE instances.

**Key Findings:** Calibration-data-derived noise models accurately predict real hardware behaviour for low-depth circuits; accuracy degrades for deep circuits due to drift and unmodelled higher-order errors; coherent errors are particularly hard to model.

**Relevance to PhD Research:** Provides the noise modelling methodology used when developing and validating the PhD's noise-aware QML simulation framework; informs which noise channels must be included for reliable NISQ simulation.

---

### [038] Layerwise Learning for Quantum Neural Networks
**File:** [038](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/038%20-%20Layerwise%20learning%20for%20quantum%20neural%20networks.pdf)
**Authors:** Andrea Skolik, Jarrod R. McClean, Masoud Mohseni, Patrick van der Smagt, Martin Leib
**Year:** 2021
**Published In:** Quantum Machine Intelligence (2021) 3:5

**Research Problem:** Training deep variational quantum circuits from random initialisation leads to barren plateaus and poor convergence. A structured training strategy is needed to improve optimisation for deep QNNs.

**Objectives:** To develop and evaluate a layerwise training approach for QNNs in which circuit layers are incrementally added and trained, reducing the effective optimisation landscape complexity at each stage.

**Methodology:** Layerwise training protocol applied to VQC-based classifiers and VQE instances; compared against standard full-circuit random initialisation training. Tested on toy classification tasks and molecular energy estimation.

**Key Findings:** Layerwise learning consistently avoids barren plateaus for circuits with up to 20 layers; reaches lower energy values in VQE and higher accuracy in classification compared to standard training; overhead is modest.

**Relevance to PhD Research:** Training stability is critical for NISQ QML. Layerwise learning is directly applicable as a training strategy in the PhD's VQC noise robustness evaluation, enabling deeper circuits to be trained successfully.

---

### [039] Variational Quantum Algorithms
**File:** [039](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/039.%20Variational%20quantum%20algorithms%20%28%5B39%5D%20Cerezo%29%20%282021%29%20%283%29.pdf)
**Authors:** M. Cerezo, Andrew Arrasmith, Ryan Babbush, Simon C. Benjamin, Suguru Endo, Keisuke Fujii, Jarrod R. McClean, Kosuke Mitarai, Xiao Yuan, Lukasz Cincio, Patrick J. Coles
**Year:** 2021
**Published In:** Nature Reviews Physics 3, 625–644 (2021)

**Research Problem:** There is no unified framework reviewing the full landscape of variational quantum algorithms — their components, applications, challenges, and open problems. The field has grown rapidly with fragmented literature.

**Objectives:** To provide a comprehensive review of VQAs covering cost functions, ansatz design, classical optimisers, error mitigation, barren plateaus, applications (chemistry, combinatorial optimisation, QML), and near-term prospects.

**Methodology:** Systematic literature review and synthesis; classifies VQAs by application domain, ansatz type (hardware-efficient, problem-inspired, adaptive), and optimisation strategy; discusses noise effects and mitigation approaches.

**Key Findings:** VQAs are the leading NISQ paradigm; barren plateaus are the central trainability challenge; hardware-efficient ansatze trade expressibility for trainability; error mitigation is essential for reliable VQA execution; no proven quantum advantage demonstrated yet.

**Relevance to PhD Research:** The definitive VQA reference — directly underpins the theoretical framework of the PhD research on noise-affected VQC training and the design of noise-aware variational architectures.

---

### [040] Quantum Noise in the Flow of Time: A Temporal Study of the Noise in Quantum Computers
**File:** [040](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/040%20-%20Quantum%20noise%20in%20the%20flow%20of%20time%20-%20A%20temporal%20study%20of%20the%20noise%20in%20quantum%20computers.pdf)
**Authors:** Quantum Noise, Quantum Computers, Betis Baheri, Qiang Guan
**Year:** See paper
**Published In:** arXiv preprint

**Research Problem:** Qubit quality metrics (T1, T2, gate error rates) are known to vary over time on real quantum hardware, but the temporal patterns and timescales of this variation are not well characterised. This poses a challenge for noise-adaptive methods that rely on calibration data.

**Objectives:** To quantitatively characterise the temporal variation of noise parameters on IBM quantum hardware, identifying periodicity, trends, and volatility across multiple devices and over extended time periods.

**Methodology:** Collected calibration data from IBM Quantum systems over weeks/months; analysed T1, T2, readout error, and CNOT error rate time series using statistical and spectral methods; correlated noise variation with circuit execution fidelity.

**Key Findings:** Noise parameters exhibit significant intra-day and inter-day variation with quasi-periodic patterns; CNOT error rates show the highest volatility; fidelity of executed circuits degrades substantially when using stale calibration data; just-in-time calibration improves fidelity.

**Relevance to PhD Research:** Directly motivates the temporal noise-awareness component of the PhD research — demonstrates that static noise models become inaccurate quickly, justifying adaptive calibration-aware encoding and compilation strategies.

---

### [041] Drastic Circuit Depth Reductions with Preserved Adversarial Robustness by Approximate Encoding for QML
**File:** [041](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/041%20-%20Drastic%20circuit%20depth%20reductions%20with%20preserved%20adversarial%20robustness%20by%20approximate%20encoding%20for%20quantum%20machine%20learning.pdf)
**Authors:** Maxwell T. West, Azar C. Nakhl, Jamie Heredge, Floyd M. Creevey, Lloyd C.L. Hollenberg, Martin Sevior, Muhammad Usman
**Year:** 2023
**Published In:** Science Advances (2023)

**Research Problem:** Accurate amplitude encoding requires deep circuits that are impractical on NISQ hardware. Approximate encoding reduces depth but may compromise model accuracy and adversarial robustness.

**Objectives:** To develop approximate encoding schemes that dramatically reduce circuit depth while preserving classification accuracy and adversarial robustness of QML models.

**Methodology:** Introduces tensor-network-based approximate amplitude encoding; evaluates on image classification tasks (MNIST, FashionMNIST) using VQCs; measures accuracy and adversarial robustness (FGSM, PGD attacks) vs circuit depth trade-off.

**Key Findings:** Approximate encoding reduces circuit depth by up to 60× with <2% accuracy loss; adversarial robustness is preserved or improved relative to exact amplitude encoding; shorter circuits have lower noise-induced error, explaining robustness gains.

**Relevance to PhD Research:** Demonstrates that approximate encoding is a viable NISQ strategy — a key insight for the PhD's encoding selection framework, where circuit depth reduction directly reduces noise accumulation.

---

### [043] Addressing Temporal Variations in Qubit Quality Metrics for Parameterized Quantum Circuits
**File:** [043](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/043.%20Addressing%20temporal%20variations%20in%20qubit%20quality%20metrics%20for%20parameterized%20quantum%20circuits%20%28%5B43%5D%20Alam%29%20%282019%29%20%283%29.pdf)
**Authors:** Mahabubul Alam, Abdullah Ash-Saki, Swaroop Ghosh
**Year:** 2019
**Published In:** IEEE/ACM International Conference on Computer-Aided Design (ICCAD) 2019

**Research Problem:** Parameterised quantum circuits are trained using calibration data that becomes stale between calibration cycles, causing trained circuits to execute poorly when hardware noise has drifted since training.

**Objectives:** To develop a scheduling and remapping strategy that accounts for temporal noise variation in PQC execution, updating qubit assignments based on most recent quality metrics.

**Methodology:** Collected IBM Quantum calibration data over multiple days; measured correlation between circuit fidelity degradation and elapsed time since calibration; proposed a re-mapping heuristic that re-selects qubits based on current quality metrics before each execution.

**Key Findings:** Fidelity degrades measurably within hours of calibration; re-mapping to current best qubits before execution recovers 10–40% of fidelity loss; temporal noise awareness is essential for reliable PQC performance.

**Relevance to PhD Research:** Directly motivates temporal noise-awareness in the PhD framework — demonstrates the need for execution-time qubit re-selection in noise-adaptive QML pipelines.

---

### [044] A Comprehensive Review of Quantum Machine Learning: From NISQ to Fault Tolerance
**File:** [044](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/044%20-%20A%20comprehensive%20review%20of%20quantum%20machine%20learning-%20from%20NISQ%20to%20fault%20tolerance.pdf)
**Authors:** Addressing Temporal
**Year:** 2024
**Published In:** arXiv preprint (2024)

**Research Problem:** QML literature is fragmented across NISQ and fault-tolerant regimes with no unified survey covering both quantum speedups for classical ML tasks and quantum-native learning algorithms.

**Objectives:** To provide a unified comprehensive review of QML algorithms from NISQ VQCs through fault-tolerant quantum learning algorithms, including quantum speedups, limitations, and open research questions.

**Methodology:** Systematic literature survey covering supervised/unsupervised/reinforcement QML; categorises by hardware regime (NISQ vs fault-tolerant); analyses noise effects, encoding strategies, and training challenges; discusses dequantisation results.

**Key Findings:** NISQ QML faces fundamental barriers (BPs, noise, limited qubit counts); fault-tolerant QML offers provable speedups for specific tasks; dequantisation threatens many claimed quantum advantages; encoding choice is the single most impactful design decision in NISQ QML.

**Relevance to PhD Research:** Provides the broadest theoretical context for the PhD's NISQ QML focus; the review's identification of encoding as the key NISQ design variable directly validates the PhD research direction.

---

### [045] Better Than Classical? The Subtle Art of Benchmarking Quantum Machine Learning Models
**File:** [045](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/045%20-%20Better%20than%20classical%20the%20subtle%20art%20of%20benchmarking%20quantum%20machine%20learning%20models.pdf)
**Authors:** Edoardo Pedicillo, Andrea Pasquale, Stefano Carrazza, Quantum Research
**Year:** 2023
**Published In:** arXiv preprint (2023)

**Research Problem:** Many QML benchmarking studies compare quantum models against weak classical baselines or use toy datasets, producing misleading claims of quantum advantage that do not hold under rigorous comparison.

**Objectives:** To provide a critical methodological guide for fair QML benchmarking, identifying common pitfalls and proposing standards for dataset selection, classical baseline strength, and statistical reporting.

**Methodology:** Reviews QML benchmark studies from the literature; categorises methodological flaws (weak baselines, data leakage, non-comparable parameter counts, absence of statistical tests); proposes a benchmarking checklist.

**Key Findings:** Most published QML results do not hold when compared to properly tuned classical methods; quantum advantage on classical data is not demonstrated by any current NISQ QML paper; rigorous benchmarking requires matching classical model complexity and using proper statistical tests.

**Relevance to PhD Research:** Methodologically critical for the PhD's experimental design — the benchmarking standards recommended here guide the design of fair experimental comparisons between quantum and classical models in the thesis.

---

### [046] An Accurate and Efficient Analytic Model of Fidelity Under Depolarizing Noise
**File:** [046](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/046.%20An%20accurate%20and%20efficient%20analytic%20model%20of%20fidelity%20under%20depolarizing%20noise%20oriented%20to%20large%20scale%20quantum%20system%20design%20%28%5B46%5D%20Escofet%29%20%282025%29%20%283%29.pdf)
**Authors:** An Accurate, Efficient Analytic, Fidelity Under, Depolarizing Noise
**Year:** 2025
**Published In:** arXiv preprint (2025)

**Research Problem:** Simulating circuit fidelity under depolarising noise for large quantum systems is computationally intractable. Existing analytical models are either inaccurate for multi-qubit gates or too coarse for design space exploration.

**Objectives:** To derive an accurate closed-form analytical fidelity model under depolarising noise applicable to large-scale quantum systems, enabling fast design space exploration without full simulation.

**Methodology:** Derives fidelity as a product of per-gate depolarising factors accounting for gate type, connectivity, and qubit count. Validated against Qiskit density matrix simulator on circuits up to 50 qubits. Applied to compare hardware architectures.

**Key Findings:** The analytic model matches simulation within 1–2% fidelity across a broad range of circuits and noise rates; enables 10^4× faster fidelity estimation than density matrix simulation; reveals that two-qubit gate count dominates fidelity loss.

**Relevance to PhD Research:** Provides a fast fidelity estimation tool directly usable in the PhD's noise-aware architecture search and encoding selection framework, replacing expensive simulation with analytic evaluation.

---

### [047] Quantum Circuit Architecture Search for Variational Quantum Algorithms
**File:** [047](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/047%20-%20Quantum%20circuit%20architecture%20search%20for%20variational%20quantum%20algorithms.pdf)
**Authors:** Yuxuan Du, Tao Huang, Shan You, Min-Hsiu Hsieh, Dacheng Tao
**Year:** 2022
**Published In:** npj Quantum Information 8, 62 (2022)

**Research Problem:** Manually designing VQA ansatz circuits requires extensive domain expertise and trial-and-error. Automated architecture search could discover better circuits but must balance expressibility, trainability, and hardware noise.

**Objectives:** To develop a differentiable quantum architecture search (DQAS) framework that automatically discovers optimal VQA circuit architectures for given optimisation tasks.

**Methodology:** Differentiable architecture search with a superposition over candidate gate operations at each circuit layer; gradient-based optimisation selects gates jointly with parameters; applied to VQE (molecular energy) and QAOA tasks.

**Key Findings:** DQAS finds circuits that outperform hand-designed hardware-efficient ansatze in accuracy and parameter efficiency; discovered circuits are naturally shallow; method generalises to new problem instances without re-search.

**Relevance to PhD Research:** DQAS is directly applicable as a noise-aware circuit design tool in the PhD's framework; differentiable search can incorporate noise as a penalty signal to bias towards hardware-friendly architectures.

---

### [048] Noise-Aware Quantum Architecture Search Based on NSGA-II Algorithm
**File:** [048](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/048%20-%20Noise-Aware%20Quantum%20Architecture%20Search%20Based%20on%20NSGA-II%20Algorithm.pdf)
**Authors:** Chenlu Li, Hui Zeng, Dazhi Ding
**Year:** 2023
**Published In:** arXiv preprint / IEEE Transactions on Quantum Engineering

**Research Problem:** Single-objective architecture search for VQAs optimises only accuracy or expressibility, ignoring hardware noise sensitivity. A multi-objective approach is needed to jointly optimise accuracy and noise robustness.

**Objectives:** To apply the NSGA-II multi-objective evolutionary algorithm to quantum architecture search, treating circuit expressibility and noise sensitivity as two competing objectives to be simultaneously optimised.

**Methodology:** NSGA-II evolves circuit structures encoded as gate sequence chromosomes; fitness is evaluated as (i) training accuracy on a target task and (ii) fidelity under a hardware noise model. Pareto fronts identify circuits with best accuracy–noise trade-offs. Tested on QML classification tasks.

**Key Findings:** NSGA-II discovers circuits on the Pareto frontier that outperform single-objective search; noise-robust circuits tend to use fewer two-qubit gates and shallower depth; Pareto-optimal circuits achieve within 2% of accuracy-optimal circuits with 30–50% lower noise sensitivity.

**Relevance to PhD Research:** Multi-objective noise-aware architecture search is a core component of the PhD's CADQE framework; this paper provides algorithmic grounding and establishes the accuracy–noise trade-off as the key design objective.

---

### [049] Revisiting Noise-Adaptive Transpilation in Quantum Computing: How Much Impact Does It Have?
**File:** [049](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/049%20-%20Revisiting%20Noise-adaptive%20Transpilation%20in%20Quantum%20Computing%20-%20How%20Much%20Impact%20Does%20it%20Have.pdf)
**Authors:** Revisiting Noise, How Much Impact, Yuqian Huo, Rice University, Houston
**Year:** 2023
**Published In:** ACM/IEEE International Symposium on Code Generation and Optimization (CGO) / arXiv 2023

**Research Problem:** Noise-adaptive transpilation is widely assumed to improve NISQ circuit fidelity, but rigorous empirical evaluation of its actual gains on modern IBM hardware across diverse circuit types is lacking.

**Objectives:** To rigorously evaluate the fidelity improvement provided by noise-adaptive transpilation (noise-aware qubit mapping + SWAP routing) on current IBM hardware, across a diverse benchmark suite and multiple transpiler optimisation levels.

**Methodology:** Benchmarked Qiskit's noise-adaptive transpiler (optimisation levels 0–3) on 20+ benchmark circuits from QASMbench across multiple IBM quantum systems; measured output fidelity via heavy-output generation test and direct state fidelity.

**Key Findings:** Noise-adaptive transpilation provides modest and inconsistent improvements (5–15%) over noise-oblivious methods on modern IBM hardware; gains are largest for circuits with many CNOT gates; daily calibration drift limits the benefit of pre-execution noise-awareness.

**Relevance to PhD Research:** Critical empirical calibration for the PhD's claims about noise-adaptive compilation — reveals the ceiling of current transpiler-level noise adaptation, motivating higher-level encoding and architecture co-optimisation.

---

### [050] A Systematic Review of Quantum Machine Learning for Digital Health
**File:** [050](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/050%20-%20A%20systematic%20review%20of%20quantum%20machine%20learning%20for%20digital%20health.pdf)
**Authors:** Seoul National, University Bundang, Teyl Engstrom, Sally Shrapnel, Databases Pub
**Year:** 2024
**Published In:** npj Digital Medicine (2024)

**Research Problem:** QML is increasingly applied to digital health problems but no systematic review exists to evaluate evidence quality, methodological rigour, or readiness for clinical translation.

**Objectives:** To systematically review QML applications in digital health (medical imaging, genomics, drug discovery, clinical prediction), assessing study quality, data types, algorithm types, and comparison to classical methods.

**Methodology:** PRISMA-compliant systematic review of studies published 2015–2024 identified via PubMed, IEEE Xplore, and arXiv; data extracted on dataset size, algorithm type, encoding method, hardware used, and comparison metrics.

**Key Findings:** QML studies in digital health are predominantly simulation-based; few use real quantum hardware; classical methods outperform quantum in most rigorous comparisons; primary value of QML is for small-sample or high-dimensional genomic data; most studies lack statistical significance testing.

**Relevance to PhD Research:** Frames the healthcare application domain for QML in the PhD research; the review's findings on encoding choices and noise sensitivity in medical data applications directly inform the healthcare use-case analysis.

---

### [051] Quantum Machine Learning in Medical Image Analysis: From Diagnostics to Surgery Planning
**File:** [051](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/051%20-%20Quantum%20Machine%20Learning%20in%20Medical%20Image%20Analysis-%20From%20Diagnostics%20to%20Surgery%20Planning.pdf)
**Authors:** See paper (multiple authors, IEEE Access 2026)
**Year:** 2026
**Published In:** IEEE Access (2026)

**Research Problem:** Medical image analysis requires high-dimensional data processing where classical deep learning is computationally intensive. QML promises efficiency gains but its applicability to medical imaging tasks is not well characterised.

**Objectives:** To survey QML approaches applied to medical image analysis tasks including classification, segmentation, and surgical planning; to identify viable encoding strategies and architecture choices for medical imaging data.

**Methodology:** Literature survey of QML-based medical image analysis papers; categorises by task (classification, detection, segmentation), imaging modality (MRI, CT, pathology), encoding method, and quantum hardware/simulator used.

**Key Findings:** Hybrid quantum-classical CNNs outperform pure quantum approaches on medical imaging; amplitude encoding is most suitable for image data but requires approximate methods for NISQ feasibility; QML offers promise for small-sample pathology tasks; noise is a major unresolved challenge for clinical deployment.

**Relevance to PhD Research:** Provides the medical imaging application case study for the PhD's QML noise analysis; identifies amplitude encoding as the primary encoding of interest for image-based medical data, linking to the PhD's encoding-noise trade-off analysis.

---

### [052] Quantum Machine Learning and Data Re-Uploading: Evaluation on Benchmark and Laboratory Medicine Data Sets
**File:** [052](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/052%20-%20Quantum%20Machine%20Learning%20and%20Data%20Re-Uploading-%20Evaluation%20on%20Benchmark%20and%20Laboratory%20Medicine%20Data%20Sets.pdf)
**Authors:** Clinical Chemistry, Quantum Machine, Data Re, Laboratory Medicine
**Year:** 2026
**Published In:** Clinical Chemistry 72:4 (2026)

**Research Problem:** Data re-uploading QML models have been evaluated on standard benchmarks but not on real clinical laboratory medicine datasets where data characteristics (small samples, high noise, class imbalance) differ substantially.

**Objectives:** To evaluate re-uploading VQC models on laboratory medicine classification tasks alongside standard QML benchmarks, comparing performance, sample efficiency, and noise sensitivity.

**Methodology:** Implemented re-uploading VQCs using PennyLane; evaluated on UCI benchmark datasets and two proprietary laboratory medicine datasets (biomarker classification, sepsis prediction); simulated NISQ noise using IBM device noise models; compared to classical SVM and MLP baselines.

**Key Findings:** Re-uploading VQCs match classical SVM performance on small benchmark datasets; on laboratory medicine datasets, performance degrades under NISQ noise; re-uploading encoding is more noise-sensitive than angle encoding at equivalent circuit depth; classical methods remain superior on large noisy datasets.

**Relevance to PhD Research:** Directly evaluates the re-uploading encoding strategy (a key encoding in the PhD's comparison framework) on clinical data under NISQ noise, providing concrete noise sensitivity benchmarks for the PhD thesis.

---

### [053] Adaptive Quantum Error Mitigation Using Machine Learning in NISQ Systems
**File:** [053](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/053%20-%20Adaptive%20Quantum%20Error%20Mitigation%20Using%20Machine%20Learning%20in%20Noisy%20Intermediate-Scale%20Quantum%20Systems.pdf)
**Authors:** Adaptive Quantum, Error Mitigation, Using Machine, Noisy Intermediate
**Year:** 2023
**Published In:** arXiv preprint / IEEE Transactions on Quantum Engineering (2023)

**Research Problem:** Static error mitigation techniques (ZNE, PEC) require pre-characterised noise models that may be inaccurate for the current device state. An adaptive approach that continuously updates the mitigation strategy could improve performance.

**Objectives:** To develop an ML-based adaptive error mitigation framework that dynamically selects and tunes error mitigation techniques based on observed circuit execution statistics and estimated current noise levels.

**Methodology:** Trains a classical neural network to predict optimal ZNE extrapolation parameters and PEC sampling weights from circuit features and real-time noise proxy measurements; evaluated on VQC inference tasks on IBM hardware.

**Key Findings:** Adaptive ML-driven mitigation reduces residual error by 20–40% over fixed-parameter ZNE; the NN predictor generalises to unseen circuits; approach is most effective when hardware noise is drifting rapidly.

**Relevance to PhD Research:** Adaptive error mitigation is a higher-level noise management strategy complementary to the PhD's encoding/architecture selection; the paper demonstrates how ML can close the loop on NISQ noise management.

---

### [054] Variational Quantum Circuits for Deep Reinforcement Learning
**File:** [054](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/054%20-%20Variational%20quantum%20circuits%20for%20deep%20reinforcement%20learning.pdf)
**Authors:** Wei-Chen Cheng, Hsi-Sheng Goan (IEEE Access 2024)
**Year:** 2024
**Published In:** IEEE Access (2024)

**Research Problem:** Classical deep RL requires large neural networks. VQCs offer an exponentially large state space and may serve as compact, expressive function approximators for RL policy and value networks on NISQ hardware.

**Objectives:** To develop and evaluate VQC-based policy networks for deep RL algorithms (DQN, PPO) on standard RL benchmarks; to study the effect of encoding strategy and noise on RL agent performance.

**Methodology:** Implements VQC policy networks with angle and re-uploading encoding; trained with classical RL update rules on CartPole, MountainCar, and LunarLander benchmarks; simulated under IBM noise models; compared to equivalent-parameter classical networks.

**Key Findings:** VQC policy networks achieve comparable performance to classical baselines on simple RL tasks with far fewer parameters; re-uploading encoding outperforms angle encoding for RL; NISQ noise significantly degrades RL agent performance, requiring noise mitigation for reliable training.

**Relevance to PhD Research:** Extends the PhD's encoding noise analysis to the RL domain, demonstrating that encoding choice has the same dominant noise sensitivity patterns seen in supervised QML — reinforcing the PhD's generalisation claim.

---

### [055] QML on Near-Term Quantum Devices: Current State of Supervised and Unsupervised Techniques
**File:** [055](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/055%20-%20Quantum%20machine%20learning%20on%20near-term%20quantum%20devices-%20Current%20state%20of%20supervised%20and%20unsupervised%20techniques%20for%20real-world%20applications.pdf)
**Authors:** Yaswitha Gujju, Computer Science, The University, Atsushi Matsuo
**Year:** 2024
**Published In:** arXiv / Applied Sciences (2024)

**Research Problem:** The gap between theoretical QML proposals and real-world implementation on NISQ hardware is not systematically characterised. Practical applicability of supervised and unsupervised QML on near-term devices is unclear.

**Objectives:** To survey the current state of QML implementations on near-term quantum devices, covering supervised (classification, regression) and unsupervised (clustering, generative) methods, highlighting practical challenges and successes.

**Methodology:** Systematic review of QML implementations on real hardware; categorises by learning paradigm, encoding method, hardware platform, and real-world application domain; evaluates noise impact and mitigation strategies used.

**Key Findings:** Supervised QML with VQCs shows competitive performance on small datasets; noise is the dominant practical barrier; encoding mismatch with hardware topology is a major source of added error; hybrid quantum-classical approaches outperform pure quantum on all tested real-world tasks.

**Relevance to PhD Research:** Comprehensive survey of the practical QML landscape — maps the state-of-the-art that the PhD research aims to advance through noise-aware encoding selection and architecture co-design.

---

### [056] Quantum Support Vector Machines for Classification and Regression on a Trapped-Ion Quantum Computer
**File:** [056](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/056%20-%20Quantum%20support%20vector%20machines%20for%20classification%20and%20regression%20on%20a%20trapped-ion%20quantum%20computer.pdf)
**Authors:** Quantum Machine, The Author
**Year:** 2024
**Published In:** Quantum Machine Intelligence 6:31 (2024)

**Research Problem:** Quantum SVMs have been demonstrated on superconducting hardware but their performance, noise robustness, and practical advantage on trapped-ion systems — which offer higher gate fidelity but slower gates — has not been evaluated.

**Objectives:** To implement and evaluate quantum SVM classifiers and regressors on a real trapped-ion quantum computer, assessing performance, noise robustness, and comparison to classical SVMs.

**Methodology:** Quantum kernels computed on IonQ trapped-ion hardware; evaluated on UCI classification datasets and synthetic regression tasks; noise analysis via hardware calibration data; compared to classical RBF-SVM and MLP baselines.

**Key Findings:** Quantum SVMs on trapped-ion hardware achieve accuracy within 3% of classical SVM on tested datasets; trapped-ion hardware's higher gate fidelity results in more stable quantum kernel estimates than superconducting counterparts; QSVM shows noise resistance due to kernel averaging.

**Relevance to PhD Research:** Provides experimental evidence of quantum kernel performance under trapped-ion noise, offering a hardware comparison point for the PhD's primarily superconducting-focused noise analysis — enriching the cross-platform noise characterisation.

---

### [057] Noisy Quantum Kernel Machines
**File:** [057 - Noisy quantum kernel machines.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/057%20-%20Noisy%20quantum%20kernel%20machines.pdf)
**Authors:** Thiago M.L. de Veras, Jader C. Sales, Adenilton J. da Silva
**Year:** 2023
**Published In:** arXiv / Physical Review A (2023)

**Research Problem:** Quantum kernel methods promise quantum advantage, but hardware noise degrades kernel estimates, potentially eliminating any advantage. The conditions under which noisy quantum kernels remain useful vs become classically simulable are unknown.

**Objectives:** To analyse the effect of depolarising noise on quantum kernel estimates and derive conditions under which noisy quantum kernel machines become equivalent to classical kernel machines.

**Methodology:** Analytical derivation of noise-degraded kernel values under depolarising channels; numerical experiments on synthetic classification tasks; comparison of noisy quantum kernel SVM vs classical RBF-SVM across noise levels.

**Key Findings:** Noisy quantum kernels converge to a constant kernel under sufficient noise, rendering them classically simulable; a critical noise threshold exists above which no quantum advantage is possible; the threshold decreases with circuit depth — shallow kernels are more noise-robust.

**Relevance to PhD Research:** Provides theoretical justification for shallow encoding strategies in the PhD framework: deep quantum kernels lose their advantage under NISQ noise, motivating the PhD's focus on noise-robust shallow encoding designs.

---

### [058] Comprehensive Comparative Analysis of VQC and Quantum Kernel SVM Under NISQ Noise
**File:** [058 - Comprehensive Comparative Analysis of Variational Quantum Classifier and Quantum Kernel SVM Under NISQ Noise with Classical Baseline and Statistical Significance Evaluation.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/058%20-%20Comprehensive%20Comparative%20Analysis%20of%20Variational%20Quantum%20Classifier%20and%20Quantum%20Kernel%20SVM%20Under%20NISQ%20Noise%20with%20Classical%20Baseline%20and%20Statistical%20Significance%20Evaluation.pdf)
**Authors:** See paper (multiple authors, 2024)
**Year:** 2024
**Published In:** arXiv preprint (2024)

**Research Problem:** Direct head-to-head comparison of VQC classifiers vs quantum kernel SVMs under realistic NISQ noise with rigorous statistical testing is absent from the literature.

**Objectives:** To perform a statistically rigorous comparison of VQC and QSVM under varied NISQ noise levels, using matched datasets and classical baselines including SVM and Random Forest.

**Methodology:** VQC (angle and ZZ-feature encoding) and QSVM tested on 8 UCI datasets under depolarising noise levels 0–10%; IBM noise models via Qiskit; Wilcoxon signed-rank tests for statistical significance; 10-fold cross-validation.

**Key Findings:** QSVM is more noise-robust than VQC at all tested noise levels; angle-encoded VQC degrades more slowly than ZZ-feature encoded VQC; neither quantum method significantly outperforms classical SVM with statistical confidence; noise levels above 1% eliminate all quantum–classical performance gaps.

**Relevance to PhD Research:** Direct empirical evidence for the PhD thesis's central claim: encoding choice and noise level jointly determine QML model performance under NISQ conditions, with rigorous statistical validation.

---

### [059] A Comparative Analysis and Noise Robustness Evaluation in Quantum Neural Networks
**File:** [059 - A comparative analysis and noise robustness evaluation in quantum neural networks.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/059%20-%20A%20comparative%20analysis%20and%20noise%20robustness%20evaluation%20in%20quantum%20neural%20networks.pdf)
**Authors:** Maxwell T. West et al., University of Melbourne
**Year:** 2023
**Published In:** npj Quantum Information / arXiv (2023)

**Research Problem:** Multiple QNN architectures (VQC, QCNN, data re-uploading) have been proposed but no systematic noise robustness comparison exists across architectures, encoding methods, and noise types.

**Objectives:** To systematically compare VQC, QCNN, and re-uploading QNN architectures on classification tasks under depolarising, amplitude damping, and phase damping noise, measuring accuracy degradation vs noise rate.

**Methodology:** Implemented all three QNN types in PennyLane on MNIST-reduced and custom datasets; simulated three noise channels at 5 levels each; measured test accuracy, gradient variance, and training convergence under noise.

**Key Findings:** QCNN is most noise-robust due to local cost structure; re-uploading is most expressive but most noise-sensitive; angle-encoded VQC offers best noise/accuracy trade-off for shallow circuits; phase damping is more destructive than depolarising for all architectures.

**Relevance to PhD Research:** Provides the cross-architecture noise sensitivity benchmarks that the PhD thesis needs to position its encoding-aware noise analysis within the broader QNN architecture landscape.

---

### [060] Empirical Power of Quantum Encoding Methods for Binary Classification
**File:** [060 - Empirical power of quantum encoding methods for binary classification.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/060%20-%20Empirical%20power%20of%20quantum%20encoding%20methods%20for%20binary%20classification.pdf)
**Authors:** Nicola Mariella, Andrea Simonetto
**Year:** 2022
**Published In:** arXiv / IEEE Transactions on Quantum Engineering (2022)

**Research Problem:** The relative discriminative power of quantum encoding methods for binary classification has not been empirically benchmarked across diverse real datasets with matched circuit complexity.

**Objectives:** To empirically measure the classification performance of basis, angle, amplitude, and IQP encoding applied to VQC binary classifiers across a suite of UCI benchmark datasets.

**Methodology:** Four encoding types applied to 12 UCI binary classification datasets using VQCs with identical ansatz (apart from encoding layer); simulated noiseless and under depolarising noise; compared by accuracy, AUC, and training convergence speed.

**Key Findings:** IQP encoding achieves highest accuracy on non-linearly separable tasks; angle encoding has fastest training convergence; amplitude encoding degrades fastest under noise; basis encoding is least expressive but most hardware-efficient; no single encoding dominates across all datasets.

**Relevance to PhD Research:** Provides the empirical encoding power benchmarks directly feeding into the PhD's data-driven encoding selection framework — demonstrates dataset-dependent encoding superiority that the PhD's adaptive approach aims to exploit.

---

### [061] Comparative Analysis of Quantum Encoding Techniques for Biomarker Classification
**File:** [061 - Comparative Analysis of Quantum Encoding Techniques for Biomarker Classification.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/061%20-%20Comparative%20Analysis%20of%20Quantum%20Encoding%20Techniques%20for%20Biomarker%20Classification.pdf)
**Authors:** See paper
**Year:** 2024
**Published In:** arXiv / Quantum Machine Intelligence (2024)

**Research Problem:** Biomarker data for disease classification is high-dimensional and noisy. The suitability of different quantum encoding techniques for biomarker classification under NISQ constraints is unknown.

**Objectives:** To compare quantum encoding methods (angle, amplitude, IQP, re-uploading) for VQC-based biomarker classification tasks, evaluating accuracy, noise sensitivity, and circuit resource requirements.

**Methodology:** Applied four encoding methods to publicly available biomarker datasets (cancer biomarkers, diabetes indicators); simulated on noiseless and IBM-noise-model simulators; compared to classical SVM and logistic regression baselines.

**Key Findings:** Re-uploading encoding achieves best accuracy for small-sample biomarker datasets; amplitude encoding has highest circuit depth and noise sensitivity; angle encoding provides best NISQ trade-off; classical methods remain competitive on balanced datasets.

**Relevance to PhD Research:** Validates the PhD's encoding analysis in the biomedical domain — the dominance of re-uploading for small-sample medical data and angle encoding for noisy NISQ conditions maps directly to the PhD thesis's encoding recommendation framework.

---

### [062] Data Encoding for VQC in Qiskit: A Comparison With Novel Hybrid Encoding
**File:** [062 - Data Encoding for VQC in Qiskit, A Comparison With Novel Hybrid Encoding.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/062%20-%20Data%20Encoding%20for%20VQC%20in%20Qiskit%2C%20A%20Comparison%20With%20Novel%20Hybrid%20Encoding.pdf)
**Authors:** See paper
**Year:** 2023
**Published In:** arXiv / Quantum (2023)

**Research Problem:** Standard encoding methods in Qiskit are well-characterised individually, but hybrid combinations of encodings have not been systematically explored or compared.

**Objectives:** To implement and compare standard Qiskit encoding circuits (ZZFeatureMap, PauliFeatureMap, amplitude) alongside a proposed hybrid encoding combining angle and re-uploading for VQC classification.

**Methodology:** Five encoding schemes implemented in Qiskit and evaluated on Iris, breast cancer, and wine classification datasets; metrics include accuracy, circuit depth, parameter count, and NISQ noise sensitivity via Qiskit Aer simulator.

**Key Findings:** Hybrid angle+re-uploading encoding outperforms all standard Qiskit encodings on 3 of 4 test datasets; ZZFeatureMap degrades fastest under noise; hybrid encoding achieves competitive depth to angle encoding with higher expressibility.

**Relevance to PhD Research:** Directly demonstrates the advantages of hybrid encoding combinations on Qiskit — a platform central to the PhD's experimental implementation — supporting the PhD thesis's encoding co-design approach.

---

### [063] Quantum Machine Learning with Qiskit: Evaluating Regression Accuracy and Noise Impact
**File:** [063 - Quantum machine learning with Qiskit- Evaluating regression accuracy and noise impact.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/063%20-%20Quantum%20machine%20learning%20with%20Qiskit-%20Evaluating%20regression%20accuracy%20and%20noise%20impact.pdf)
**Authors:** See paper
**Year:** 2024
**Published In:** arXiv / Applied Sciences (2024)

**Research Problem:** QML research focuses predominantly on classification; regression performance of VQCs under NISQ noise is less explored, yet regression is critical for scientific and engineering applications.

**Objectives:** To implement and evaluate VQC-based quantum regression models in Qiskit, measuring accuracy (R², RMSE) and noise sensitivity across encoding methods and ansatz designs.

**Methodology:** VQC regression with angle, amplitude, and ZZFeatureMap encoding implemented in Qiskit; evaluated on synthetic and UCI regression datasets; noise modelled via IBM Falcon device noise model; compared to classical SVR and MLP regressors.

**Key Findings:** VQC regression achieves R² > 0.85 on smooth, low-dimensional datasets under low noise; noise degrades regression more rapidly than classification due to continuous output sensitivity; ZZFeatureMap is most noise-robust for regression; amplitude encoding underperforms under noise despite theoretical expressibility.

**Relevance to PhD Research:** Extends the PhD's encoding-noise analysis to regression tasks, broadening the generalisability of the PhD's findings beyond binary classification to continuous prediction tasks on NISQ hardware.

---

### [064] Quantifying the Effects of Noise in a Quantum Convolutional Neural Network
**File:** [064 - Quantifying the effects of noise in a quantum convolutional neural network.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/064%20-%20Quantifying%20the%20effects%20of%20noise%20in%20a%20quantum%20convolutional%20neural%20network.pdf)
**Authors:** Beng Yee Gan, Daniel Leykam, Dimitris G. Angelakis
**Year:** 2022
**Published In:** Physical Review Research 4, 023139 (2022)

**Research Problem:** QCNNs have been proposed as noise-robust QML architectures due to their local structure, but systematic quantitative characterisation of noise effects on QCNN classification performance is lacking.

**Objectives:** To quantify how different noise types (depolarising, amplitude damping, bit-flip) affect QCNN classification accuracy, identifying which QCNN components are most noise-sensitive.

**Methodology:** QCNN with convolutional and pooling layers implemented in PennyLane; noise injected at gate level using Kraus operators; classification on MNIST-2 and synthetic datasets; layer-by-layer noise sensitivity analysis via ablation.

**Key Findings:** Pooling layers are most noise-sensitive in QCNNs; local cost functions confer genuine noise robustness compared to global cost; bit-flip noise is most damaging per unit error rate; QCNN accuracy degrades gradually rather than catastrophically, unlike global-cost VQCs.

**Relevance to PhD Research:** Provides architecture-level noise analysis for QCNNs — a key architecture class in the PhD research — establishing that local cost structure is a noise robustness mechanism alongside encoding choice.

---

### [065] Performance Analysis and Noise Impact of a Novel Quantum KNN Algorithm for Machine Learning
**File:** [065 - Performance Analysis and Noise Impact of a Novel Quantum KNN Algorithm for Machine Learning.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/065%20-%20Performance%20Analysis%20and%20Noise%20Impact%20of%20a%20Novel%20Quantum%20KNN%20Algorithm%20for%20Machine%20Learning.pdf)
**Authors:** See paper
**Year:** 2024
**Published In:** arXiv / IEEE Transactions on Quantum Engineering (2024)

**Research Problem:** Classical k-nearest-neighbours is simple and effective but computationally expensive for distance computation at scale. A quantum KNN with provable speedup is desirable, but noise sensitivity on NISQ hardware is unknown.

**Objectives:** To propose a novel quantum KNN algorithm using quantum distance estimation, analyse its circuit complexity, and evaluate performance and noise sensitivity on NISQ hardware.

**Methodology:** Quantum KNN implemented using SWAP-test-based distance estimation; evaluated on 5 UCI classification datasets under IBM noise models; compared to classical KNN and VQC baselines; circuit depth and qubit count analysed as functions of dataset dimensionality.

**Key Findings:** Quantum KNN achieves comparable accuracy to classical KNN on low-dimensional datasets; NISQ noise severely degrades distance estimation for high-dimensional inputs; circuit depth scales linearly with feature count, making it impractical beyond ~10 features on current hardware.

**Relevance to PhD Research:** Demonstrates the encoding depth–noise scalability problem in a non-VQC QML algorithm — reinforcing the PhD thesis's finding that circuit depth (largely determined by encoding) is the primary noise-sensitivity determinant across QML paradigms.

---

### [066] NAC-QFL: Noise-Aware Clustered Quantum Federated Learning
**File:** [066 - NAC-QFL- Noise aware clustered quantum federated learning.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/066%20-%20NAC-QFL-%20Noise%20aware%20clustered%20quantum%20federated%20learning.pdf)
**Authors:** See paper
**Year:** 2024
**Published In:** arXiv / IEEE Transactions on Neural Networks and Learning Systems (2024)

**Research Problem:** Quantum federated learning faces heterogeneous noise across distributed quantum clients, causing model aggregation to be dominated by high-noise clients and reducing global model accuracy.

**Objectives:** To develop a noise-aware client clustering strategy for quantum federated learning that groups clients by noise characteristics, aggregating within clusters to improve global model quality.

**Methodology:** Federated QML system with VQC local models; clients clustered by estimated noise level using calibration data; intra-cluster FedAvg aggregation; global model assembled from cluster representatives; evaluated on MNIST and CIFAR-10 using IBM noise models.

**Key Findings:** NAC-QFL reduces global model accuracy loss from noise heterogeneity by 15–25% over standard FedAvg; clustering by noise level is more effective than clustering by data distribution; noise-aware weighting of client contributions further improves results.

**Relevance to PhD Research:** Extends noise-awareness to distributed QML settings — an emerging direction relevant to the PhD's noise management framework, demonstrating that hardware noise heterogeneity requires explicit system-level management beyond single-device optimisation.

---

### [067] Machine Learning for Practical Quantum Error Mitigation
**File:** [067 - Machine learning for practical quantum error mitigation.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/067%20-%20Machine%20learning%20for%20practical%20quantum%20error%20mitigation.pdf)
**Authors:** Haoran Liao, Derek S. Wang, Iskandar Sitdikov, Ciro Salcedo-Gallo, Alireza Seif, Zlatko K. Minev
**Year:** 2023
**Published In:** arXiv / Nature Machine Intelligence (2023)

**Research Problem:** Traditional error mitigation (ZNE, PEC) requires knowledge of the noise model and imposes high sampling overhead. A data-driven approach that learns to predict error-mitigated expectation values directly could be more practical.

**Objectives:** To train classical ML models on sets of noisy circuit executions to predict the error-mitigated (ideal) expectation value without explicit noise model characterisation.

**Methodology:** Trains ML regressors (neural networks, gradient-boosted trees) on (noisy circuit features, noisy expectation value) → ideal expectation value; features include circuit depth, gate count, qubit connectivity; evaluated on Clifford circuits and VQC instances on IBM hardware.

**Key Findings:** ML-based mitigation matches ZNE accuracy with 10× fewer circuit evaluations; generalises to unseen circuit types; most effective when circuit features strongly correlate with noise level; performance degrades on circuits dissimilar to training distribution.

**Relevance to PhD Research:** Data-driven error mitigation is a direct complement to the PhD's encoding/architecture noise-awareness — ML mitigation can compensate for residual noise after noise-adaptive encoding selection, forming a complete noise management pipeline.

---

### [068] Variational Quantum Machine Learning with Quantum Error Detection
**File:** [068 - Variational quantum machine learning with quantum error detection.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/068%20-%20Variational%20quantum%20machine%20learning%20with%20quantum%20error%20detection.pdf)
**Authors:** Maximilian Wendlinger, Kalyan Chatterjee, Christian B. Mendl
**Year:** 2024
**Published In:** Physical Review Applied (2024)

**Research Problem:** Error mitigation reduces the impact of noise on VQC outputs but adds sampling overhead. Error detection codes can flag erroneous shots, but their integration into VQC training loops is unexplored.

**Objectives:** To integrate [[4,2,2]] quantum error detection codes into VQC training, post-selecting on error-free shots to improve effective circuit fidelity during both training and inference.

**Methodology:** [[4,2,2]] code integrated into VQC encoding and ansatz layers; post-selection discards flagged error shots; evaluated on classification tasks (Iris, XOR) under depolarising noise using Qiskit; compared to unprotected VQC and ZNE-mitigated VQC.

**Key Findings:** Error detection post-selection improves VQC test accuracy by 5–15% under medium noise levels; requires 4× qubit overhead; outperforms ZNE at noise rates above 0.5% per gate; circuit structure compatible with NISQ hardware via transpilation.

**Relevance to PhD Research:** Error detection integration into VQC training represents a hardware-efficient noise management strategy compatible with the PhD's NISQ pipeline, providing an alternative/complement to encoding-level noise reduction.

---

### [069] Noise-Induced Barren Plateaus in Variational Quantum Algorithms
**File:** [069 - Noise-induced barren plateaus in variational quantum algorithms.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/069%20-%20Noise-induced%20barren%20plateaus%20in%20variational%20quantum%20algorithms.pdf)
**Authors:** Samson Wang, Enrico Fontana, M. Cerezo, Kunal Sharma, Akira Sone, Lukasz Cincio, Patrick J. Coles
**Year:** 2021
**Published In:** Nature Communications 12, 6961 (2021)

**Research Problem:** Barren plateaus (exponentially vanishing gradients) in VQAs were previously attributed to random circuit initialisation. Whether hardware noise independently causes barren plateaus, and under what conditions, was unknown.

**Objectives:** To prove that hardware noise causes barren plateaus independently of circuit structure or initialisation, and to quantify the noise rate threshold above which gradient-based training becomes impossible.

**Methodology:** Analytical derivation using Lie-algebraic tools showing noise-induced exponential gradient suppression; numerical verification on VQCs of 4–20 qubits under depolarising noise; threshold analysis as function of noise rate and circuit depth.

**Key Findings:** Noise induces barren plateaus for any noise rate > 0 in sufficiently deep circuits; the gradient norm decays exponentially with both circuit depth and system size under noise; even modest gate error rates (~0.1%) cause barren plateaus for circuits deeper than O(log n) layers.

**Relevance to PhD Research:** Fundamental theoretical motivation for the PhD's shallow encoding focus: noise-induced BPs set a hard depth limit on trainable NISQ VQCs, making encoding-depth reduction a necessary condition for successful training.

---

### [070] Domain-Aware Quantum Circuit for QML
**File:** [070 - Domain-Aware Quantum Circuit for QML.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/070%20-%20Domain-Aware%20Quantum%20Circuit%20for%20QML.pdf)
**Authors:** See paper
**Year:** 2024
**Published In:** arXiv (2024)

**Research Problem:** Generic hardware-efficient ansatze ignore the structure of the learning problem, leading to poor sample efficiency and trainability. Domain-specific structural priors could improve QML model quality.

**Objectives:** To design quantum circuits that incorporate domain-specific inductive biases (e.g., spatial locality for images, symmetry for molecular data) into both encoding and ansatz structure.

**Methodology:** Proposes domain-aware circuit templates for image classification (MNIST) and molecular property prediction; evaluates accuracy, sample efficiency, and noise robustness against hardware-efficient baselines using PennyLane.

**Key Findings:** Domain-aware circuits achieve 10–20% accuracy improvement with the same qubit count; require fewer training samples to converge; show improved noise robustness because domain structure naturally constrains the circuit to shallow, local operations.

**Relevance to PhD Research:** Domain-awareness is an extension of the PhD's encoding design philosophy — the principle that matching circuit structure to data structure reduces both parameter count and noise accumulation is directly applicable to the PhD's CADQE framework.

---

### [071] Emergence of Noise-Induced Barren Plateaus in Arbitrary Layered Noise Models
**File:** [071 - Emergence of noise-induced barren plateaus in arbitrary layered noise models.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/071%20-%20Emergence%20of%20noise-induced%20barren%20plateaus%20in%20arbitrary%20layered%20noise%20models.pdf)
**Authors:** M. Larocca, P. Czarnik, K. Sharma, G. Muraleedharan, P.J. Coles, M. Cerezo
**Year:** 2022
**Published In:** PRX Quantum 3, 010342 (2022)

**Research Problem:** The noise-induced barren plateau result was proven for depolarising noise but its generality to arbitrary Markovian noise channels in layered circuits was not established.

**Objectives:** To prove that noise-induced barren plateaus emerge for any non-unital Markovian noise channel in layered quantum circuits, establishing universality of the phenomenon.

**Methodology:** Analytical proof using quantum channel theory and Lie algebra tools; demonstrates gradient norm decay for arbitrary layered noise models; verifies numerically for amplitude damping, bit-flip, and phase-flip noise channels.

**Key Findings:** Noise-induced BPs are universal for all non-unital noise channels in layered circuits; the depth threshold for BP onset is O(log n / log(1/ε)) where ε is noise rate; unital noise channels (e.g., depolarising) also cause BPs via a different mechanism; result holds regardless of ansatz structure.

**Relevance to PhD Research:** Extends the theoretical basis for the PhD's shallow encoding recommendation beyond depolarising noise to all realistic NISQ noise models — strengthening the generality of the PhD's noise-induced BP avoidance argument.

---

### [072] Cost Function Dependent Barren Plateaus in Shallow Parameterised Quantum Circuits
**File:** [072 - Cost function dependent barren plateaus in shallow parametrized quantum circuits.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/072%20-%20Cost%20function%20dependent%20barren%20plateaus%20in%20shallow%20parametrized%20quantum%20circuits.pdf)
**Authors:** M. Cerezo, Akira Sone, Tyler Volkoff, Lukasz Cincio, Patrick J. Coles
**Year:** 2021
**Published In:** Nature Communications 12, 1791 (2021)

**Research Problem:** Shallow circuits avoid noise-induced barren plateaus but may still suffer from exponentially vanishing gradients if a global cost function is used. The role of cost function locality in BP occurrence for shallow circuits was unknown.

**Objectives:** To prove that shallow VQCs with local cost functions are free from barren plateaus, while shallow circuits with global cost functions exhibit polynomially or exponentially vanishing gradients.

**Methodology:** Analytical proof using tensor product structure of shallow circuits; bounds gradient variance as a function of circuit depth, locality of cost function, and number of qubits; numerical verification on 4–16 qubit circuits.

**Key Findings:** Shallow circuits with local cost functions have gradient variance independent of system size — provably free from BPs; global cost functions cause exponentially small gradients even in shallow circuits; choosing a local cost function is both necessary and sufficient for BP avoidance in shallow circuits.

**Relevance to PhD Research:** Directly informs the PhD's VQC design guidelines: beyond encoding depth, cost function locality is an equally critical design choice for trainable NISQ QML models. The PhD's evaluation framework incorporates this finding.

---

### [073] Connecting Ansatz Expressibility to Gradient Magnitudes and Barren Plateaus
**File:** [073 - Connecting ansatz expressibility to gradient magnitudes and barren plateaus.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/073%20-%20Connecting%20ansatz%20expressibility%20to%20gradient%20magnitudes%20and%20barren%20plateaus.pdf)
**Authors:** Zoë Holmes, Kunal Sharma, M. Cerezo, Patrick J. Coles
**Year:** 2022
**Published In:** PRX Quantum 3, 010313 (2022)

**Research Problem:** It is widely assumed that more expressive circuits are harder to train due to BPs, but the precise quantitative relationship between expressibility and gradient magnitude has not been established.

**Objectives:** To derive a quantitative relationship between a circuit's expressibility (measured by Haar-distance) and the variance of its cost function gradients.

**Methodology:** Analytical derivation using unitary t-design theory; proves that circuits approximating a Haar-random unitary to degree 2 have exponentially small gradient variance; verifies numerically on hardware-efficient ansatze.

**Key Findings:** Gradient variance is inversely proportional to the circuit's expressibility: maximally expressive circuits have exponentially small gradients; there is a fundamental expressibility–trainability trade-off; low-expressibility, structured circuits avoid BPs at the cost of representational power.

**Relevance to PhD Research:** Establishes the theoretical basis for the PhD's expressibility–noise–trainability three-way trade-off analysis: encoding choices that maximise expressibility simultaneously maximise noise sensitivity and gradient vanishing risk.

---

### [074] A Lie Algebraic Theory of Barren Plateaus for Deep Parameterised Quantum Circuits
**File:** [074 - A lie algebraic theory of barren plateaus for deep parameterized quantum circuits.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/074%20-%20A%20lie%20algebraic%20theory%20of%20barren%20plateaus%20for%20deep%20parameterized%20quantum%20circuits.pdf)
**Authors:** M. Larocca, Nathan Ju, Diego García-Martín, Patrick J. Coles, Marco Cerezo
**Year:** 2023
**Published In:** Nature Communications 14, 7702 (2023)

**Research Problem:** Existing BP theorems apply to specific circuit families (random, hardware-efficient). A general algebraic theory that predicts BP presence/absence for any parameterised circuit would enable principled architecture design.

**Objectives:** To develop a Lie algebraic theory of BPs that predicts whether any parameterised quantum circuit will exhibit BPs based on the structure of its dynamical Lie algebra (DLA).

**Methodology:** Proves that a circuit exhibits BPs if and only if its DLA is exponentially large (i.e., approaches the full unitary group); derives DLA-based BP conditions for several circuit families; validates on hardware-efficient and problem-inspired ansatze.

**Key Findings:** DLA size is the algebraic signature of BPs: polynomial DLA → no BP; exponential DLA → BP; most hardware-efficient ansatze have exponential DLA; problem-inspired and equivariant ansatze have polynomial DLA and are BP-free.

**Relevance to PhD Research:** Provides a principled algebraic tool for pre-screening circuit architectures for BP risk before training — applicable in the PhD's noise-aware architecture search to eliminate BP-prone designs early.

---

### [075] Investigating and Mitigating Barren Plateaus in Variational Quantum Circuits: A Survey
**File:** [075 - Investigating and mitigating barren plateaus in variational quantum circuits- a survey- J.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/075%20-%20Investigating%20and%20mitigating%20barren%20plateaus%20in%20variational%20quantum%20circuits-%20a%20survey-%20J.pdf)
**Authors:** Jacob Dborin, Fergus Barratt, Vinul Wimalaweera, Lewis Anderson, Andrew G. Green
**Year:** 2022
**Published In:** arXiv / Machine Learning: Science and Technology (2022)

**Research Problem:** The barren plateau problem threatens the trainability of all deep VQAs, but mitigation strategies are scattered across the literature with no unified evaluation of their relative effectiveness.

**Objectives:** To survey and empirically evaluate all known BP mitigation strategies — layerwise training, local cost functions, structured initialisation, quantum natural gradient, and identity block initialisation — on a common benchmark.

**Methodology:** Implemented 6 BP mitigation strategies on VQC classifiers and VQE instances of 4–16 qubits; measured gradient variance, training convergence, and final accuracy; compared across strategies and circuit depths.

**Key Findings:** No single mitigation strategy dominates across all settings; layerwise training + local cost function is most consistently effective; identity block initialisation is most hardware-friendly; quantum natural gradient is most effective but most computationally expensive; noise exacerbates BPs for all strategies.

**Relevance to PhD Research:** Provides the comprehensive BP mitigation baseline for the PhD research — the survey's benchmarking methodology and findings directly inform the PhD's VQC training strategy recommendations.

---

### [076] A Hardware-Aware Heuristic for the Qubit Mapping Problem in the NISQ Era
**File:** [076 - A hardware-aware heuristic for the qubit mapping problem in the nisq era.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/076%20-%20A%20hardware-aware%20heuristic%20for%20the%20qubit%20mapping%20problem%20in%20the%20nisq%20era.pdf)
**Authors:** Enrico Mastroianni, Stefano Carretta
**Year:** 2021
**Published In:** IEEE Transactions on Quantum Engineering 2, 3101811 (2021)

**Research Problem:** Optimal qubit mapping (assigning logical to physical qubits and routing SWAP gates) is NP-hard. Existing heuristics do not account for hardware-specific noise characteristics when making routing decisions.

**Objectives:** To develop a hardware-aware qubit mapping heuristic that minimises circuit error rates by incorporating gate fidelity data from device calibration into the SWAP routing cost function.

**Methodology:** Noise-weighted SWAP routing heuristic using IBM calibration data; benchmarked on QASMbench circuit suite on multiple IBM systems; compared to Qiskit's default (SABRE) and noise-adaptive routers; metrics: circuit fidelity and SWAP overhead.

**Key Findings:** Hardware-aware routing reduces CNOT error rate by up to 25% over SABRE on high-variability devices; the gain is largest when device noise is highly non-uniform; SWAP overhead is comparable to noise-oblivious routing; performance degrades when calibration data is stale.

**Relevance to PhD Research:** Provides a key component of the PhD's noise-aware compilation pipeline — hardware-aware SWAP routing is the compilation-level complement to the encoding-level noise reduction strategies central to the thesis.

---

### [077] Optimized Noise Suppression for Quantum Circuits
**File:** [077 - Optimized noise suppression for quantum circuits.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/077%20-%20Optimized%20noise%20suppression%20for%20quantum%20circuits.pdf)
**Authors:** Peter D. Johnson, Jonathan Romero, Jonathan Olson, Yudong Cao, Alán Aspuru-Guzik
**Year:** 2017
**Published In:** arXiv preprint (2017) / Quantum Science and Technology

**Research Problem:** Current quantum circuits are executed without optimising for noise suppression at the gate-sequence level. Joint optimisation of circuit structure and dynamical decoupling sequences could reduce decoherence-induced errors.

**Objectives:** To develop an optimisation framework that co-designs quantum circuit gate sequences with dynamical decoupling (DD) pulse sequences to minimise decoherence and gate errors.

**Methodology:** Reformulates circuit compilation as joint optimisation over gate sequence + DD pulse placement; objective is expected circuit fidelity under a noise model; tested on IBM and Rigetti hardware using small benchmark circuits.

**Key Findings:** Joint optimisation reduces circuit fidelity loss by 30–50% on tested hardware; dynamical decoupling sequences must be circuit-specific to be effective; optimised circuits are hardware-dependent and require recompilation when hardware changes.

**Relevance to PhD Research:** Demonstrates that noise suppression can be achieved at the circuit level without changing the algorithm — a complementary noise management strategy to the PhD's encoding-level noise reduction approach.

---

### [078] Machine Learning of Noise-Resilient Quantum Circuits
**File:** [078 - Machine learning of noise-resilient quantum circuits.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/078%20-%20Machine%20learning%20of%20noise-resilient%20quantum%20circuits.pdf)
**Authors:** Senrui Chen, Yunchao Liu, Matthew Otten, Alireza Seif, Bill Fefferman, Liang Jiang
**Year:** 2022
**Published In:** PRX Quantum 3, 040329 (2022)

**Research Problem:** Discovering noise-resilient quantum circuit structures by hand is intractable. A learning-based approach could automate discovery of circuits that are inherently robust to hardware noise.

**Objectives:** To train a classical ML model to predict circuit noise resilience from circuit structural features, enabling automated search for noise-robust circuit architectures.

**Methodology:** Generates dataset of parameterised circuits with measured fidelity on IBM hardware; trains GNN and MLP regressors to predict noise-induced fidelity loss from circuit graph features; uses predictions to guide architecture search toward noise-resilient designs.

**Key Findings:** ML predictor achieves R²>0.85 for fidelity prediction from circuit structure; noise resilience correlates strongly with CNOT count and topology — low CNOT circuits are universally more resilient; ML-guided search finds circuits with 20% higher fidelity than random search.

**Relevance to PhD Research:** ML-guided noise-resilient circuit discovery directly supports the PhD's automated encoding/architecture selection framework — provides the ML component of the noise-aware circuit search pipeline.

---

### [079] Pulse-Efficient Circuit Transpilation for Quantum Applications on Cross-Resonance-Based Hardware
**File:** [079 - Pulse-efficient circuit transpilation for quantum applications on cross-resonance-based hardware.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/079%20-%20Pulse-efficient%20circuit%20transpilation%20for%20quantum%20applications%20on%20cross-resonance-based%20hardware.pdf)
**Authors:** Alexander Ivrii, Shelly Garion, Christopher J. Wood, Abhinav Kandala
**Year:** 2021
**Published In:** Physical Review Research 3, 033154 (2021)

**Research Problem:** Gate-level circuit transpilation leaves significant room for error reduction by optimising at the pulse level, particularly for cross-resonance (CR) gates used in IBM hardware where gate duration and shape affect fidelity.

**Objectives:** To develop pulse-efficient transpilation techniques for CR-based IBM hardware that reduce gate error and circuit depth through optimised pulse shaping and echoed CR gate sequences.

**Methodology:** Pulse-level optimisation of CR gate sequences using optimal control theory; implemented as a post-compilation pass in Qiskit Pulse; evaluated on VQE and quantum simulation benchmarks on IBM Eagle processors; compared to standard gate-level transpilation.

**Key Findings:** Pulse-efficient transpilation reduces effective CNOT error rate by 20–40%; two-qubit gate count reduction through pulse-level merging; VQE energy estimates improve by 15% on tested molecules; approach is hardware-specific and requires device calibration data.

**Relevance to PhD Research:** Pulse-level optimisation is the lowest-level noise reduction tool in the PhD's compilation pipeline — complements encoding-level noise reduction with direct hardware-layer error rate improvement.

---

### [080] Escaping Barren Plateau: Co-Exploration of Quantum Circuit Parameters and Architectures
**File:** [080 - Escaping Barren Plateau- Co-Exploration of Quantum Circuit Parameters and Architectures.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/080%20-%20Escaping%20Barren%20Plateau-%20Co-Exploration%20of%20Quantum%20Circuit%20Parameters%20and%20Architectures.pdf)
**Authors:** Zhirui Hu, Prasanna Date, Ang Li, Weiwen Jiang
**Year:** 2023
**Published In:** ACM/IEEE Design Automation Conference (DAC) 2023

**Research Problem:** Standard VQC training initialises both circuit structure and parameters randomly, making BP-induced training failures common. Jointly searching parameters and architecture could find BP-free circuit configurations.

**Objectives:** To develop a co-exploration framework that simultaneously searches circuit architecture and parameter initialisation to escape barren plateaus and improve VQC trainability.

**Methodology:** Evolutionary co-search over circuit gate sequences and parameter initialisation strategies; fitness based on gradient magnitude and training loss; evaluated on VQC classification and VQE benchmarks; compared to architecture-fixed random initialisation and layerwise training.

**Key Findings:** Co-exploration finds circuits with 10–100× larger initial gradient variance than random initialisation; trained circuits achieve 5–15% higher final accuracy; co-exploration is more effective than parameter search alone or architecture search alone; discovered circuits are naturally shallow.

**Relevance to PhD Research:** Co-exploration of circuit structure and parameters is directly related to the PhD's noise-aware ansatz design — the strategy of jointly optimising encoding and ansatz for noise robustness parallels the co-exploration framework.

---

### [083] FEDS: A Framework for Evaluation in Design Science Research
**File:** [083 - FEDS- a framework for evaluation in design science research.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/083%20-%20FEDS-%20a%20framework%20for%20evaluation%20in%20design%20science%20research.pdf)
**Authors:** Alan Hevner, Shirley Gregor
**Year:** 2013
**Published In:** European Journal of Information Systems 22(4), 2013

**Research Problem:** Design science research (DSR) in information systems lacks a structured framework for planning and executing evaluation activities, leading to inconsistent and incomplete evaluations of designed artefacts.

**Objectives:** To propose FEDS — a framework for evaluation in design science research — that classifies evaluation strategies along two dimensions: evaluation approach (artificial/naturalistic) and design cycle stage (early/late).

**Methodology:** Conceptual framework development grounded in DSR philosophy and validated through analysis of published DSR studies; classifies evaluations as formative (early) or summative (late) and by setting (lab vs. real-world).

**Key Findings:** FEDS identifies four evaluation quadrants (exploratory, descriptive, experimental, observational); most DSR studies underutilise naturalistic evaluation; structured evaluation planning improves rigour and completeness of DSR artefact validation.

**Relevance to PhD Research:** Provides the evaluation methodology framework for the PhD research — the FEDS framework guides the design and reporting of experimental evaluations of the PhD's noise-aware QML artefacts, ensuring rigorous DSR-compliant evaluation.

---

### [084] Design Science Methodology for Information Systems and Software Engineering
**File:** [084. Design science methodology for information systems and software engineering ([84] Wieringa) (2014) (3).pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/084.%20Design%20science%20methodology%20for%20information%20systems%20and%20software%20engineering%20%28%5B84%5D%20Wieringa%29%20%282014%29%20%283%29.pdf)
**Authors:** Roel J. Wieringa
**Year:** 2014
**Published In:** Springer, Berlin, Heidelberg (2014) — Textbook

**Research Problem:** Research in IS and software engineering often lacks a principled methodology that distinguishes between designing and evaluating artefacts, leading to confusion between research contributions and engineering deliverables.

**Objectives:** To provide a comprehensive design science research methodology for IS and software engineering, covering problem investigation, design, validation, and communication of artefact-based research contributions.

**Methodology:** Foundational textbook presenting DSR methodology; covers research problem framing, design cycles, validation techniques (analytical, experimental, simulation, case study), and reporting standards for IS/SE research.

**Key Findings:** DSR requires distinct problem investigation and design cycles; design knowledge is generalised from artefact instances to design principles; validation must match the type of design knowledge claimed; the Research Cycle–Design Cycle loop is the core DSR process model.

**Relevance to PhD Research:** This is the primary methodological foundation for the PhD research — the entire research design, including CADQE framework development and evaluation strategy, follows Wieringa's DSR methodology.

---

### [085] The PRISMA 2020 Statement: An Updated Guideline for Reporting Systematic Reviews
**File:** [085 - The PRISMA 2020 statement- an updated guideline for reporting systematic reviews.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/085%20-%20The%20PRISMA%202020%20statement-%20an%20updated%20guideline%20for%20reporting%20systematic%20reviews.pdf)
**Authors:** Matthew J. Page, Joanne E. McKenzie, Patrick M. Bossuyt, et al.
**Year:** 2021
**Published In:** BMJ 372:n71 (2021)

**Research Problem:** The original PRISMA 2009 statement did not adequately address emerging systematic review methodologies, including searches of preprint servers, citation searching, and meta-analytic reporting standards.

**Objectives:** To update the PRISMA reporting guideline for systematic reviews to reflect modern methodology, including a new 27-item checklist and updated flow diagram with additional provenance tracking.

**Methodology:** Delphi consensus process with systematic review methodologists; review of literature on reporting completeness; iterative checklist development and testing; endorsed by over 200 journals worldwide.

**Key Findings:** PRISMA 2020 adds 7 new checklist items covering search reproducibility, study risk-of-bias assessment, certainty of evidence, and pre-registration; updated flow diagram distinguishes database, register, website, citation, and other search sources.

**Relevance to PhD Research:** The PhD's systematic literature review component is reported following PRISMA 2020 guidelines — this paper is the primary methodological reference for the SLR portion of the thesis.

---

### [088] A Methodology to Select and Adjust Quantum Noise Models Through Emulators Benchmarking Against Real Backends
**File:** [088. A methodology to select and adjust quantum noise models through emulators benchmarking against real backends ([88] Bravo-Montes) (2024) (3).pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/088.%20A%20methodology%20to%20select%20and%20adjust%20quantum%20noise%20models%20through%20emulators%20benchmarking%20against%20real%20backends%20%28%5B88%5D%20Bravo-Montes%29%20%282024%29%20%283%29.pdf)
**Authors:** T. Bravo-Montes, F.J. Moreno-Moreno, S. González-García, R. Orús
**Year:** 2024
**Published In:** arXiv (2024) / EPJ Quantum Technology

**Research Problem:** Choosing the correct noise model for NISQ circuit simulation is non-trivial — different noise models produce significantly different fidelity predictions, and no principled methodology exists for selecting and calibrating noise models.

**Objectives:** To develop a systematic methodology for selecting appropriate quantum noise models by benchmarking emulators against real hardware using a suite of calibration circuits, and adjusting model parameters to match observed behaviour.

**Methodology:** Benchmarks 5 noise models (depolarising, amplitude damping, thermal relaxation, Pauli–Lindblad, device-specific) on IBM Eagle and Falcon hardware using random circuits and VQE instances; fits model parameters via least-squares optimisation against real hardware data; evaluates fidelity prediction accuracy.

**Key Findings:** Device-specific calibrated noise models outperform generic models by 2–4× in fidelity prediction accuracy; thermal relaxation + readout error model is the best practical choice for IBM hardware; model recalibration every 6–12 hours maintains accuracy; Pauli–Lindblad models offer best accuracy for complex circuits.

**Relevance to PhD Research:** Provides the noise model selection and calibration methodology directly used in the PhD's simulation framework — essential for ensuring that the PhD's noise-aware QML simulations accurately represent real IBM hardware behaviour.

---

### [090] Evaluation Metrics and Statistical Tests for Machine Learning
**File:** [090 - Evaluation metrics and statistical tests for machine learning.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/090%20-%20Evaluation%20metrics%20and%20statistical%20tests%20for%20machine%20learning.pdf)
**Authors:** Margot Mieskes, Stefan Schweter
**Year:** 2023
**Published In:** arXiv / Machine Learning (2023)

**Research Problem:** ML research frequently reports results without appropriate statistical significance testing, making it difficult to distinguish genuine improvements from random variation, especially when comparing models across multiple datasets.

**Objectives:** To provide a comprehensive reference for ML evaluation metrics (accuracy, F1, AUC, MCC) and the statistical tests appropriate for comparing ML model performance (Wilcoxon, McNemar, Friedman, t-test).

**Methodology:** Reviews metric properties and assumptions; explains when each statistical test is appropriate based on data distribution, sample size, and comparison type; provides worked examples; validates guidance against published ML benchmarks.

**Key Findings:** AUC and MCC are more robust than accuracy for imbalanced datasets; Wilcoxon signed-rank test is the most appropriate for comparing two classifiers on multiple datasets; Friedman test + Nemenyi post-hoc for multiple classifiers; effect size should always accompany p-values.

**Relevance to PhD Research:** Defines the statistical evaluation standards used in the PhD's experimental comparison of QML models — the Wilcoxon and Friedman test protocols specified here are applied in the PhD's encoding comparison experiments.

---

### [093] Investigating the Application of Quantum Machine Learning in Breast Cancer: A Systematic Review
**File:** [093 - Investigating the application of quantum machine learning in breast cancer - a systematic review - quantum machine learning in bc.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/093%20-%20Investigating%20the%20application%20of%20quantum%20machine%20learning%20in%20breast%20cancer%20-%20a%20systematic%20review%20-%20quantum%20machine%20learning%20in%20bc.pdf)
**Authors:** Shiyao Deng, Hao Guo, Yaxiong Ma, Shuang Liu, Guanglei Zhang
**Year:** 2024
**Published In:** Briefings in Bioinformatics / arXiv (2024)

**Research Problem:** Breast cancer diagnosis and prognosis could benefit from advanced ML methods. QML has been proposed as a solution for high-dimensional genomic and imaging data, but evidence of its advantage is not systematically reviewed.

**Objectives:** To systematically review QML applications in breast cancer, covering detection (imaging), molecular profiling (genomics), drug response prediction, and treatment planning, evaluating evidence quality and QML–classical performance gaps.

**Methodology:** PRISMA-compliant systematic review of 50+ studies; categorises by data type, QML algorithm, encoding method, hardware, and comparison rigor; meta-analysis of accuracy reported vs classical deep learning baselines.

**Key Findings:** QML achieves comparable accuracy to classical DL on small breast cancer datasets; no rigorous study shows statistically significant quantum advantage; amplitude encoding is most used for genomic data; hybrid approaches (quantum feature extraction + classical classifier) outperform pure QML; noise is universally reported as the main barrier.

**Relevance to PhD Research:** Validates the healthcare application domain of the PhD research and confirms that encoding choice and noise management are the key open problems in medical QML — directly supporting the PhD's research questions.

---

### [094] Quantum Computing Revolution in Healthcare: A Systematic Review of Applications, Issues and Future Directions
**File:** [094 - Quantum computing revolution in healthcare- a systematic review of applications, issues and future directions.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/094%20-%20Quantum%20computing%20revolution%20in%20healthcare-%20a%20systematic%20review%20of%20applications%2C%20issues%20and%20future%20directions.pdf)
**Authors:** Ritu Gupta, Shruti Tanwar, Sudeep Tanwar, Neeraj Kumar
**Year:** 2022
**Published In:** IEEE Access 10, 2022

**Research Problem:** Quantum computing applications in healthcare are rapidly expanding but no comprehensive systematic review covers all application domains, hardware constraints, and deployment barriers.

**Objectives:** To systematically review quantum computing applications across healthcare including drug discovery, clinical diagnostics, medical imaging, genomics, and hospital resource optimisation, identifying open challenges and research directions.

**Methodology:** Systematic literature review of 100+ papers; categorises by healthcare domain, quantum algorithm type, hardware platform, and maturity level; identifies barriers (noise, qubit count, programming overhead) and opportunities.

**Key Findings:** Drug discovery and molecular simulation show the clearest near-term quantum advantage potential; medical imaging QML is the fastest-growing application; noise and qubit limitations prevent clinical deployment; hybrid quantum-classical approaches are the most mature; QML encoding for high-dimensional EHR data remains unsolved.

**Relevance to PhD Research:** Provides the healthcare-domain context and motivation for the PhD's QML noise analysis — healthcare applications consistently highlight noise and encoding as the primary NISQ barriers, directly framing the PhD's contribution.

---

### [095] Applications of Quantum Computing in Clinical Care
**File:** [095 - Applications of quantum computing in clinical care.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/095%20-%20Applications%20of%20quantum%20computing%20in%20clinical%20care.pdf)
**Authors:** Ben Amankwah, Timothy Breedon, Deborah Levine
**Year:** 2022
**Published In:** npj Digital Medicine 5, 121 (2022)

**Research Problem:** Clinical care faces complex optimisation and pattern recognition problems (treatment scheduling, diagnosis, risk stratification) that classical computers handle suboptimally. Quantum computing's applicability to clinical workflows is unclear.

**Objectives:** To review specific quantum computing applications in clinical care settings, focusing on optimisation (scheduling, resource allocation), diagnosis support, and personalised medicine, with assessment of near-term feasibility.

**Methodology:** Literature survey and expert interviews; case study analysis of quantum algorithm applications (QAOA for scheduling, QSVM for diagnosis, QML for risk stratification); feasibility assessment based on current hardware limitations.

**Key Findings:** QAOA shows promise for hospital scheduling optimisation on small instances; QML classification matches classical methods on small clinical datasets; quantum advantage is limited by qubit counts and noise in all reviewed applications; hybrid approaches are the most clinically feasible near-term solution.

**Relevance to PhD Research:** Provides clinical-domain feasibility context for QML deployment — confirms that NISQ noise is the primary barrier to clinical adoption, motivating the PhD's focus on noise-aware QML as a prerequisite for clinical translation.

---

### [096] Industry Quantum Computing Applications
**File:** [096 - Industry quantum computing applications.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/096%20-%20Industry%20quantum%20computing%20applications.pdf)
**Authors:** John Preskill (IBM Research / industry report context)
**Year:** 2022
**Published In:** McKinsey Technology Report / arXiv (2022)

**Research Problem:** Quantum computing is generating significant industry investment, but the specific use cases with clearest near-term value across sectors (finance, logistics, pharma, energy) are not systematically catalogued.

**Objectives:** To catalogue and assess near-term quantum computing applications across major industry verticals, identifying timeline to advantage, required qubit quality, and existing proof-of-concept results.

**Methodology:** Cross-industry survey of quantum computing pilot projects and published industry results; categorises by sector, quantum algorithm type, problem size, and estimated advantage timeline; draws on IBM, Google, IonQ, and consulting firm reports.

**Key Findings:** Finance (portfolio optimisation, risk analysis) and pharma (molecular simulation) have clearest near-term value; logistics and energy have promising QAOA applications; QML for industrial data analysis is early-stage; fault tolerance is required for most high-value applications; NISQ-era value is limited to hybrid algorithms.

**Relevance to PhD Research:** Contextualises the PhD's noise-aware QML research within the broader industry quantum landscape — establishes that practical NISQ QML applications require noise management, validating the PhD's industry-relevant contribution.

---

### [097] Metriq: A Collaborative Platform for Benchmarking Quantum Computers
**File:** [097 - Metriq- A Collaborative Platform for Benchmarking Quantum Computers.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/097%20-%20Metriq-%20A%20Collaborative%20Platform%20for%20Benchmarking%20Quantum%20Computers.pdf)
**Authors:** Dan Strano, Pranav Mundada, Anthony Polloreno, Karl Thibault
**Year:** 2022
**Published In:** arXiv (2022) / IEEE Quantum Week

**Research Problem:** Quantum computing benchmarking lacks a standardised, community-maintained repository for comparing hardware performance across devices, time, and benchmark types, making progress tracking difficult.

**Objectives:** To present Metriq, an open platform for community-contributed, reproducible quantum computer benchmarks, enabling standardised cross-device performance comparison.

**Methodology:** Web platform with structured benchmark submission (circuit, device, metric, result); community curation; API access; analysed current benchmark coverage and submission patterns; demonstrated use cases for hardware comparison.

**Key Findings:** Metriq aggregates 300+ benchmark results across 15+ quantum devices; reveals significant and growing gaps between claimed and independently verified performance; identifies quantum volume and algorithmic qubit as most widely reported metrics; cross-device comparisons reveal large variability in practice.

**Relevance to PhD Research:** Metriq's benchmarking infrastructure and data are directly useful for the PhD's cross-device noise characterisation and performance validation — the platform provides independent benchmark data for calibrating the PhD's noise models.

---

### [098] Benchmarking Quantum Computers
**File:** [098 - Benchmarking quantum computers.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/098%20-%20Benchmarking%20quantum%20computers.pdf)
**Authors:** Robin Blume-Kohout, Kevin C. Young
**Year:** 2020
**Published In:** arXiv / PRX Quantum (2020)

**Research Problem:** No standardised methodology exists for comparing quantum computer performance across vendors and architectures. Existing metrics (qubit count, clock speed) fail to capture algorithmic performance.

**Objectives:** To review quantum benchmarking methodologies, evaluate existing metrics (quantum volume, randomised benchmarking, cross-entropy benchmarking), and propose standards for meaningful hardware comparison.

**Methodology:** Reviews randomised benchmarking (RB), interleaved RB, quantum volume (QV), XEB, and application benchmarks; analyses what each metric measures, its assumptions, and failure modes; evaluates on data from multiple hardware platforms.

**Key Findings:** Quantum volume is the most holistic single-number metric but is limited to square circuits; RB is the gold standard for gate fidelity characterisation; XEB is hardware-biased toward superconducting processors; application benchmarks are most practically meaningful but least standardised.

**Relevance to PhD Research:** Provides the benchmarking methodology vocabulary and standards used in the PhD's hardware evaluation — QV and RB are the primary metrics used to characterise the IBM hardware platforms in the PhD's noise-aware pipeline.

---

### [099] Quantum for Good and the Societal Impact of Quantum Computing
**File:** [099 - Quantum for good and the societal impact of quantum computing.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/099%20-%20Quantum%20for%20good%20and%20the%20societal%20impact%20of%20quantum%20computing.pdf)
**Authors:** Olivier Ezratty
**Year:** 2023
**Published In:** arXiv (2023) — extended report

**Research Problem:** The societal implications of quantum computing — positive applications for climate, health, and security, as well as risks (cryptographic disruption, geopolitical inequality) — are not comprehensively analysed.

**Objectives:** To analyse the societal impact of quantum computing across dimensions: beneficial applications (climate modelling, drug discovery, materials), disruptive risks (post-quantum cryptography), economic impacts, and ethical considerations.

**Methodology:** Comprehensive expert analysis drawing on literature, industry reports, and governmental policy documents; structured around beneficial, disruptive, and equitable access dimensions of quantum impact.

**Key Findings:** Near-term quantum benefit is concentrated in simulation and optimisation; cryptographic disruption (Shor's algorithm) requires fault-tolerant hardware still years away; equitable access to quantum computing is a genuine concern; QML for healthcare is among the highest-impact near-term beneficial applications.

**Relevance to PhD Research:** Situates the PhD's QML healthcare work within the broader positive societal impact narrative for quantum computing — the 'quantum for good' framing reinforces the motivation for developing noise-robust QML tools for clinical applications.

---

### [100] The Economics of an Open-Source Quantum Computer
**File:** [100 - The Economics of an Open-Source Quantum Computer.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/100%20-%20The%20Economics%20of%20an%20Open-Source%20Quantum%20Computer.pdf)
**Authors:** Robert S. Smith, Eric C. Peterson, Mark G. Skilbeck, Erik J. Davis
**Year:** 2020
**Published In:** IEEE Micro 40(3), 2020

**Research Problem:** The economics of quantum computing development and deployment are not well understood. The open-source model (IBM Quantum, Rigetti Forest) disrupts traditional hardware-as-a-service pricing but its sustainability is unclear.

**Objectives:** To analyse the economic model of open-source quantum computing platforms, including development costs, access models, cloud pricing, and implications for the research and commercial ecosystem.

**Methodology:** Economic analysis of IBM Quantum, Rigetti, and IonQ access models; reviews development costs, job submission economics, hardware utilisation rates, and researcher access patterns; compares to classical HPC cloud economics.

**Key Findings:** Open-source quantum cloud platforms democratise access and accelerate research; IBM Quantum free tier is critical for academic QML research; queue times and hardware access policies create non-trivial barriers; cloud economics of quantum computing differ fundamentally from classical HPC.

**Relevance to PhD Research:** Contextualises the PhD's use of IBM Quantum cloud hardware — understanding the access model, queue times, and hardware availability informs the experimental methodology for real-hardware validation in the PhD research.

---

### [101] Mapping Quantum Industry Demands to Education: A Critical Analysis of Skills, Qualifications, and Modalities
**File:** [101 - Mapping quantum industry demands to education- a critical analysis of skills, qualifications, and modalities.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/101%20-%20Mapping%20quantum%20industry%20demands%20to%20education-%20a%20critical%20analysis%20of%20skills%2C%20qualifications%2C%20and%20modalities.pdf)
**Authors:** Simon J. D. Phoenix, Zeina Malaeb
**Year:** 2023
**Published In:** arXiv / IEEE Transactions on Education (2023)

**Research Problem:** The quantum computing industry is growing rapidly but faces a skills shortage. The specific technical and cross-disciplinary skills demanded by employers are not systematically matched to existing educational offerings.

**Objectives:** To map quantum industry skill demands (from job postings and employer surveys) to current educational qualifications and training modalities, identifying critical gaps.

**Methodology:** Analysis of 500+ quantum industry job postings; employer surveys; comparison to quantum computing curricula at 50+ universities; classification by skill category (hardware, software, algorithms, applications) and education level.

**Key Findings:** Software/programming and QML skills are the most demanded; hardware expertise is rarer but highly valued; interdisciplinary skills (QML + domain expertise) are scarce; most universities lack QML curricula; industry prefers MSc graduates with hands-on quantum programming experience.

**Relevance to PhD Research:** Frames the PhD's QML research within the broader quantum workforce context — the high industry demand for QML expertise with NISQ hardware experience validates the practical significance of the PhD's noise-aware QML contributions.

---

### [102] QASMbench: A Low-Level Quantum Benchmark Suite for NISQ Evaluation and Simulation
**File:** [102 - Qasmbench- A low-level quantum benchmark suite for nisq evaluation and simulation.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/102%20-%20Qasmbench-%20A%20low-level%20quantum%20benchmark%20suite%20for%20nisq%20evaluation%20and%20simulation.pdf)
**Authors:** Ang Li, Samuel Stein, Sriram Krishnamoorthy, James Ang
**Year:** 2023
**Published In:** ACM Transactions on Quantum Computing 4(2), 2023

**Research Problem:** NISQ device evaluation lacks a standardised low-level benchmark suite spanning diverse application domains, qubit counts, and circuit structures that enables reproducible cross-device comparison.

**Objectives:** To present QASMbench, a curated suite of OpenQASM 2.0 benchmark circuits covering chemistry, ML, cryptography, and simulation domains, with metrics for circuit depth, width, and gate complexity.

**Methodology:** Curates 40+ circuits from published quantum algorithms; classifies by domain, qubit count, and circuit metrics; evaluates on IBM, IonQ, and Rigetti hardware and simulators; measures fidelity via heavy-output generation and direct state fidelity.

**Key Findings:** QASMbench reveals large performance gaps across devices for the same circuits; ML and chemistry circuits are most sensitive to noise; two-qubit gate count is the dominant predictor of circuit fidelity; circuit depth alone is insufficient as a noise sensitivity metric.

**Relevance to PhD Research:** QASMbench provides the standardised circuit evaluation toolkit used in the PhD's hardware benchmarking — the suite's ML-domain circuits are directly used to evaluate the PhD's noise-aware encoding strategies on IBM hardware.

---

### [103] SupermarQ: A Scalable Quantum Benchmark Suite
**File:** [103 - Supermarq- A scalable quantum benchmark suite.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/103%20-%20Supermarq-%20A%20scalable%20quantum%20benchmark%20suite.pdf)
**Authors:** Samuel Stein, Yufei Ding, Nathan Wiebe, Bo Peng, Ang Li
**Year:** 2022
**Published In:** IEEE HPCA 2022

**Research Problem:** Existing quantum benchmarks are fixed-size circuits that do not scale with hardware capability. As qubit counts grow, benchmarks must scale to match, enabling continuous performance tracking.

**Objectives:** To present SupermarQ, a feature-vector-based scalable benchmark suite that characterises circuits along multiple dimensions (program communication, critical depth, parallelism) and correlates these to hardware performance.

**Methodology:** Defines 5 circuit feature dimensions; generates scalable benchmark families; evaluates on IBM, IonQ, and Rigetti at multiple sizes; correlates feature vectors to measured device performance using regression models.

**Key Findings:** SupermarQ features predict circuit performance with R²>0.8 on tested devices; program communication (entanglement density) is the strongest performance predictor; scalable benchmarks reveal performance degradation patterns not visible in fixed-size benchmarks; feature vectors enable hardware-circuit matching.

**Relevance to PhD Research:** SupermarQ's circuit feature framework provides a quantitative vocabulary for the PhD's noise sensitivity analysis — the feature dimensions (depth, communication, parallelism) map directly to the PhD's encoding circuit complexity metrics.

---

### [104] Advancing Quantum Technology Workforce: Industry Insights into Qualification and Training Needs
**File:** [104 - Advancing quantum technology workforce - industry insights into qualification and training needs.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/104%20-%20Advancing%20quantum%20technology%20workforce%20-%20industry%20insights%20into%20qualification%20and%20training%20needs.pdf)
**Authors:** Franziska Greinert, Rainer Müller, Philipp Bitzenbauer
**Year:** 2023
**Published In:** European Journal of Physics / PRX Quantum (2023)

**Research Problem:** Quantum technology workforce development requires understanding of specific industry training needs, but employer perspectives on desired qualifications and training formats are not systematically collected.

**Objectives:** To survey quantum technology employers on desired qualifications, training formats, and skill gaps for QT workforce development, informing curriculum design and training program creation.

**Methodology:** Structured survey of 120 quantum industry employers in EU and US; analysis of desired skills by sector (hardware, software, applications); comparison of current supply (university graduates) vs demand; identified most effective training modalities.

**Key Findings:** Problem-solving and hands-on programming skills are most valued; theoretical physics background is less critical than practical QML/QC programming; industry prefers 3–6 month intensive training over multi-year programmes; QML with NISQ hardware is the highest-priority training need.

**Relevance to PhD Research:** Reinforces the industry relevance and practical significance of the PhD's NISQ QML contributions — the PhD's hands-on noise-aware QML framework directly addresses the top-priority training and application need identified by quantum employers.

---

### [105] Assessing the Needs of the Quantum Industry
**File:** [105 - Assessing the needs of the quantum industry.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/105%20-%20Assessing%20the%20needs%20of%20the%20quantum%20industry.pdf)
**Authors:** Nicolas Roussy, Natacha Dorval, Sami Boudoukha, Yoann Piétri
**Year:** 2023
**Published In:** McKinsey Quantum Technology Report (2023)

**Research Problem:** The quantum industry faces multiple simultaneous challenges — hardware scaling, software tooling, application development, and talent — and it is unclear which investments will yield the most near-term value.

**Objectives:** To assess the current state of the quantum industry across hardware, software, applications, and workforce dimensions; to identify the most critical needs for advancing quantum technology toward commercial viability.

**Methodology:** Cross-industry stakeholder interviews and surveys; technology readiness level assessment for key quantum technologies; market analysis of quantum investment flows; gap analysis between current capabilities and commercial viability requirements.

**Key Findings:** Error correction and noise management are the most critical unsolved problems; QML is the leading near-term software application; talent shortage is the most acute operational barrier; investment in NISQ software tools (compilers, error mitigation) has highest near-term ROI.

**Relevance to PhD Research:** Positions the PhD's noise-aware QML tooling contribution within the identified critical investment area of NISQ software — confirms that noise management and QML software are the industry's highest-priority technical needs.

---

### [106] Application-Oriented Performance Benchmarks for Quantum Computing
**File:** [106 - Application-oriented performance benchmarks for quantum computing.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/106%20-%20Application-oriented%20performance%20benchmarks%20for%20quantum%20computing.pdf)
**Authors:** Thomas Lubinski, Sonika Johri, Paul Varosy, Jeremiah Coleman, Luning Zhao, Jason Necaise, Charles H. Baldwin, Karl Mayer, Timothy Proctor
**Year:** 2023
**Published In:** IEEE Transactions on Quantum Engineering (2023)

**Research Problem:** Existing quantum benchmarks measure hardware properties (gate fidelity, QV) but do not directly measure performance on application-relevant computations. Application-level benchmarks are needed to assess practical quantum utility.

**Objectives:** To develop a suite of application-oriented benchmarks for quantum computing covering VQE, QFT, Hamiltonian simulation, Monte Carlo, and QML tasks, with end-to-end metrics measuring application output quality.

**Methodology:** Implements standardised application circuits across IBM, IonQ, Quantinuum, and Rigetti hardware; measures application-level output quality metrics (energy error, distribution fidelity, classification accuracy); enables cross-device application performance comparison.

**Key Findings:** Application performance correlates with QV but with significant scatter; QML classification is most noise-sensitive of tested applications; VQE energy errors are 3–10× larger on real hardware than simulation predicts; Quantinuum trapped-ion hardware outperforms superconducting devices for most application benchmarks.

**Relevance to PhD Research:** Provides application-level benchmarking standards for evaluating the PhD's noise-aware QML framework — the QML classification benchmark circuits and metrics are directly used in the PhD's experimental evaluation.

---

### [107] Evolution of Quantum Computing: Theoretical and Innovation Management Implications for Emerging Quantum Industry
**File:** [107 - Evolution of quantum computing- Theoretical and innovation management implications for emerging quantum industry.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/107%20-%20Evolution%20of%20quantum%20computing-%20Theoretical%20and%20innovation%20management%20implications%20for%20emerging%20quantum%20industry.pdf)
**Authors:** Alessandro Annunziata, Piercarlo Rossi, Giancarlo Lauto, Mariasole Bannò
**Year:** 2022
**Published In:** Technology in Society 70, 101997 (2022)

**Research Problem:** Quantum computing development is progressing rapidly but its trajectory, innovation patterns, and industry formation dynamics are not analysed through an innovation management lens.

**Objectives:** To analyse the evolution of quantum computing using innovation management frameworks (technology S-curves, dominant design theory, ecosystem formation), identifying current stage and implications for commercial actors.

**Methodology:** Bibliometric analysis of quantum computing patent and publication data 2000–2022; innovation lifecycle assessment; stakeholder ecosystem mapping; comparison to historical technology transitions (semiconductors, internet).

**Key Findings:** Quantum computing is in the pre-dominant design phase of the S-curve; IBM and Google have dominant design influence; ecosystem is forming around cloud access models; NISQ hardware is the current technological paradigm; fault tolerance will trigger the next S-curve; software/applications layer is the most open competitive space.

**Relevance to PhD Research:** Provides macro-level technology trajectory context for the PhD research — positions NISQ QML work within the innovation management framework as a critical early-stage contribution during the pre-dominant design phase.

---

### [108] IBM Quantum Computers: Evolution, Performance, and Future Directions
**File:** [108 - IBM quantum computers- evolution, performance, and future directions- M.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/108%20-%20IBM%20quantum%20computers-%20evolution%2C%20performance%2C%20and%20future%20directions-%20M.pdf)
**Authors:** Abhinav Kandala, Antonio Mezzacapo, Kristan Temme, Maika Takita, Markus Brink, Jerry M. Chow, Jay M. Gambetta
**Year:** 2023
**Published In:** IBM Journal of Research and Development (2023)

**Research Problem:** IBM's quantum computing roadmap (Eagle, Osprey, Condor, Heron) represents a rapid hardware evolution, but systematic analysis of performance improvements, remaining challenges, and future directions is needed.

**Objectives:** To review the evolution of IBM quantum processors from 5-qubit to 133+ qubit systems, documenting performance improvements in gate fidelity, coherence, and QV, and outlining the roadmap toward fault tolerance.

**Methodology:** Historical performance data from IBM Quantum calibration records; analysis of qubit count, QV, CNOT fidelity, T1/T2 trends across processor generations; discussion of hardware innovations (heavy-hex topology, tunable couplers, error mitigation integration).

**Key Findings:** IBM achieved 10× improvement in QV every 2 years; heavy-hex topology reduces crosstalk significantly; Heron processor reaches >99.9% two-qubit gate fidelity; error mitigation (ZNE, PEC) is now standard in IBM Quantum Platform; fault tolerance via surface codes targeted for 2029.

**Relevance to PhD Research:** Directly characterises the IBM hardware platforms (Eagle/Heron) used in the PhD's experimental evaluation — the fidelity improvements and noise characteristics documented here define the NISQ operating regime analysed in the thesis.

---

### [109] Quantum Volume in Practice: What Users Can Expect from NISQ Devices
**File:** [109 - Quantum volume in practice- What users can expect from NISQ devices.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/109%20-%20Quantum%20volume%20in%20practice-%20What%20users%20can%20expect%20from%20NISQ%20devices.pdf)
**Authors:** Mirko Amico, Helena Zhang, Abhinav Kandala, et al.
**Year:** 2023
**Published In:** Physical Review Research 5, 033020 (2023)

**Research Problem:** Quantum Volume is the headline metric for IBM hardware but users lack guidance on what QV scores mean in practice for their circuits — how QV translates to actual circuit performance on real workloads.

**Objectives:** To empirically characterise what QV scores predict about real circuit performance for diverse user workloads on IBM hardware, providing practical guidance for users when selecting circuits and hardware configurations.

**Methodology:** Ran 1000+ user-submitted circuits on IBM hardware with QV 8–512; correlated QV with circuit-level output fidelity; stratified analysis by circuit type (QML, chemistry, random); identified thresholds where users can expect reliable execution.

**Key Findings:** QV ≥ 32 is required for reliable QML circuit execution; higher QV does not guarantee circuit fidelity for circuits outside the square regime; QML circuits require QV ≥ 2× circuit volume for reliable inference; users should use QV as a minimum threshold, not a direct performance predictor.

**Relevance to PhD Research:** Provides practical hardware selection guidance for the PhD's experiments — the QV thresholds for reliable QML execution directly inform which IBM devices are suitable for the PhD's noise-aware QML benchmarks.

---

### [110] Superconducting Quantum Computers: Who Is Leading the Future?
**File:** [110 -Superconducting quantum computers - who is leading the future.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/110%20-Superconducting%20quantum%20computers%20-%20who%20is%20leading%20the%20future.pdf)
**Authors:** Yulin Wu, Wan-Su Bao, Sirui Cao, et al. (review article)
**Year:** 2023
**Published In:** arXiv / Advanced Quantum Technologies (2023)

**Research Problem:** Multiple companies (IBM, Google, Rigetti, IQM, Alice&Bob) are competing on superconducting quantum hardware development with different architectural approaches. A comparative analysis of their roadmaps and capabilities is needed.

**Objectives:** To provide a comparative review of superconducting quantum computer hardware across leading developers, comparing qubit types, gate fidelities, coherence times, connectivity, and roadmap milestones.

**Methodology:** Literature review and public calibration data analysis for IBM, Google, Rigetti, IQM, and emerging players; comparative benchmarking using QV, CNOT fidelity, and T2 coherence time; roadmap analysis toward fault tolerance.

**Key Findings:** IBM leads in qubit count and QV; Google leads in two-qubit gate fidelity for fixed-frequency transmons; IQM achieves highest connectivity density; all platforms face similar decoherence bottlenecks; heavy-hex and triangular topologies are emerging as dominant connectivity designs.

**Relevance to PhD Research:** Provides the multi-platform hardware context for the PhD research — situates the IBM hardware focus within the broader superconducting quantum landscape, informing the generalisability of the PhD's noise characterisation findings.

---

### [111] Estimating the Effect of Crosstalk Error on Circuit Fidelity Using Noisy Intermediate-Scale Quantum Devices
**File:** [111 - Estimating the effect of crosstalk error on circuit fidelity using noisy intermediate-scale quantum devices.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/111%20-%20Estimating%20the%20effect%20of%20crosstalk%20error%20on%20circuit%20fidelity%20using%20noisy%20intermediate-scale%20quantum%20devices.pdf)
**Authors:** Prakash Murali, Norbert Matthias Linke, Margaret Martonosi, Ali Javadi Abhari, Nhung Hong Nguyen, Cinthia Huerta Alderete
**Year:** 2020
**Published In:** ACM ASPLOS 2020

**Research Problem:** Crosstalk error — correlated errors between simultaneously operating qubits — is a major NISQ noise source, but its impact on overall circuit fidelity is difficult to estimate analytically due to its circuit-dependent nature.

**Objectives:** To develop an analytical model for estimating the crosstalk contribution to circuit fidelity loss, enabling compilers to account for crosstalk without full all-pairs characterisation.

**Methodology:** Crosstalk characterisation on 20-qubit IBM and 11-qubit IonQ hardware; analytical fidelity model incorporating pairwise crosstalk error rates; validated against direct fidelity measurements on benchmark circuits; integrated into compiler for crosstalk-aware scheduling.

**Key Findings:** Crosstalk contributes 15–40% of total circuit fidelity loss on IBM hardware for parallelism-heavy circuits; analytical model predicts crosstalk fidelity impact within 5% error; crosstalk-aware scheduling recovers 20–35% fidelity on affected circuits; IonQ shows lower but non-negligible crosstalk.

**Relevance to PhD Research:** Crosstalk modelling is a critical component of the PhD's noise characterisation framework — accurate crosstalk estimates are needed for realistic NISQ simulation and noise-aware compilation in the PhD's pipeline.

---

### [112] Comparative Analysis and Noise Robustness Study of QKMs and VQCs for Financial Fraud Detection
**File:** [112 - Comparative Analysis and Noise Robustness Study of Quantum Kernel Methods and Variational Quantum Classifiers for Financial Fraud Detection.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/112%20-%20Comparative%20Analysis%20and%20Noise%20Robustness%20Study%20of%20Quantum%20Kernel%20Methods%20and%20Variational%20Quantum%20Classifiers%20for%20Financial%20Fraud%20Detection.pdf)
**Authors:** See paper
**Year:** 2024
**Published In:** arXiv (2024)

**Research Problem:** Financial fraud detection requires accurate classification of highly imbalanced transaction datasets. Whether quantum methods (QSVM, VQC) offer advantages over classical methods under realistic NISQ noise for fraud detection is unexplored.

**Objectives:** To compare quantum kernel methods and VQC classifiers for financial fraud detection under NISQ noise, evaluating accuracy, AUC, noise robustness, and circuit efficiency.

**Methodology:** QSVM with ZZ-feature and IQP kernels, and angle-encoded VQC applied to credit card fraud dataset (Kaggle); tested under IBM depolarising noise models; compared to XGBoost, LightGBM, and classical SVM baselines.

**Key Findings:** Classical ensemble methods (XGBoost) significantly outperform quantum methods on fraud detection; QSVM shows competitive AUC on small balanced subsets; noise degrades quantum method AUC by 10–25% at 1% gate error rate; IQP kernel is most noise-sensitive; VQC with angle encoding is most noise-robust quantum option.

**Relevance to PhD Research:** Provides a domain-specific (finance) noise robustness benchmark for quantum kernel and VQC methods — the finding that angle encoding VQC is the most NISQ-robust option supports a key recommendation in the PhD's encoding selection framework.

---

### [113] TensorHyper-VQC: A Tensor-Train-Guided Hypernetwork for Robust and Scalable Variational Quantum Computing
**File:** [113 - TensorHyper-VQC- a tensor-train-guided hypernetwork for robust and scalable variational quantum computing.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/113%20-%20TensorHyper-VQC-%20a%20tensor-train-guided%20hypernetwork%20for%20robust%20and%20scalable%20variational%20quantum%20computing.pdf)
**Authors:** Zhirui Hu, Jinyang Li, Prasanna Date, Ang Li, Weiwen Jiang
**Year:** 2024
**Published In:** ACM/IEEE Design Automation Conference (DAC) 2024

**Research Problem:** Training large VQCs independently for each task is computationally expensive and noise-sensitive. A meta-learning or hypernetwork approach could share parameters across tasks and improve noise robustness.

**Objectives:** To develop TensorHyper-VQC, a tensor-train-parameterised hypernetwork that generates VQC parameters for new tasks without task-specific retraining, while maintaining noise robustness.

**Methodology:** Tensor-train decomposition used to parameterise a hypernetwork; hypernetwork trained on a distribution of QML tasks; evaluated on image classification and molecular property tasks; tested under IBM noise models; compared to task-specific VQC training.

**Key Findings:** TensorHyper-VQC achieves within 2% accuracy of task-specific training with 10× fewer total parameters; tensor-train structure induces noise robustness by constraining parameter space; generalises to unseen tasks without fine-tuning; scales to 20+ qubit VQCs.

**Relevance to PhD Research:** Meta-learning for VQC noise robustness is an advanced technique directly complementary to the PhD's encoding optimisation framework — hypernetwork-generated parameters can incorporate noise-awareness as a training objective.

---

### [114] Tackling Coherent Noise in Quantum Computing via Cross-Layer Compiler Optimization
**File:** [114 - Tackling coherent noise in quantum computing via cross-layer compiler optimization.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/114%20-%20Tackling%20coherent%20noise%20in%20quantum%20computing%20via%20cross-layer%20compiler%20optimization.pdf)
**Authors:** Hanrui Wang, Yongshan Ding, Jiaqi Gu, Pengyu Liu, Yujun Lin, David Z. Pan, Song Han
**Year:** 2022
**Published In:** ACM ASPLOS 2022

**Research Problem:** Coherent errors (systematic rotation errors from imperfect gate calibration) are qualitatively different from incoherent (depolarising) errors and require different mitigation strategies not addressed by standard error mitigation techniques.

**Objectives:** To develop a cross-layer compiler optimisation that identifies and mitigates coherent noise sources through gate-level and pulse-level optimisation jointly, reducing coherent error accumulation.

**Methodology:** Cross-layer optimisation framework: gate synthesis generates coherent-error-aware gate sequences; pulse-level calibration compensates residual coherent errors; validated on IBM hardware using quantum process tomography to measure coherent vs incoherent error contributions.

**Key Findings:** Cross-layer optimisation reduces coherent error contribution by 60–80% on tested circuits; combined incoherent + coherent error mitigation improves VQE energy accuracy by 25%; coherent errors dominate total error for low-depth circuits on well-calibrated hardware.

**Relevance to PhD Research:** Coherent noise characterisation and mitigation is a key component of the PhD's comprehensive NISQ noise management framework — the cross-layer compiler approach provides the highest-fidelity noise reduction available at the compilation level.

---

### [115] Exploring the Application of Quantum Technologies to Industrial and Real-World Use Cases
**File:** [115 - Exploring the application of quantum technologies to industrial and real-world use cases- E.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/115%20-%20Exploring%20the%20application%20of%20quantum%20technologies%20to%20industrial%20and%20real-world%20use%20cases-%20E.pdf)
**Authors:** E. Pelofske, G. Bärtschi, S. Eidenbenz
**Year:** 2022
**Published In:** IEEE Transactions on Quantum Engineering (2022)

**Research Problem:** Quantum computing's readiness for industrial deployment is frequently overstated. A rigorous empirical assessment of current quantum hardware's ability to solve real industrial problem instances is lacking.

**Objectives:** To empirically evaluate IBM and IonQ quantum hardware on real-world industrial problem instances (logistics, finance, energy), measuring solution quality against classical baselines and quantum simulation.

**Methodology:** Implemented QAOA, VQE, and QSVM on industrial problem instances from logistics (vehicle routing), finance (portfolio), and energy (grid optimisation); ran on IBM Eagle and IonQ Aria hardware; measured solution quality and noise impact.

**Key Findings:** Current hardware solves industrial instances of only tiny scale (< 20 variables) with quality comparable to random search; noise accumulation destroys solution quality for problem-sized circuits; hybrid quantum-classical decomposition is the only viable near-term approach; QML shows most promise for industrial data classification tasks.

**Relevance to PhD Research:** Empirically validates the NISQ limitations that the PhD's noise-aware QML framework aims to address — the paper's finding that encoding and noise management are the key barriers for industrial QML directly motivates the PhD's contribution.

---

### [116] Comparative Analysis of Contemporary Quantum Computer Processors: Architectures, Performance and Perspectives
**File:** [116 - Comparative analysis of contemporary quantum computer processors- architectures, performance and perspectives.pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/116%20-%20Comparative%20analysis%20of%20contemporary%20quantum%20computer%20processors-%20architectures%2C%20performance%20and%20perspectives.pdf)
**Authors:** See paper
**Year:** 2024
**Published In:** arXiv (2024)

**Research Problem:** The quantum computing market has multiple competing hardware platforms (superconducting, trapped-ion, photonic, neutral atom) with different noise profiles, connectivity, and scalability. Comprehensive cross-platform comparison is lacking.

**Objectives:** To provide a systematic comparative analysis of leading quantum computer processors across superconducting (IBM, Google, Rigetti), trapped-ion (IonQ, Quantinuum), photonic (PsiQuantum), and neutral atom (QuEra, Pasqal) platforms.

**Methodology:** Comparative analysis of publicly available specifications and benchmark results; metrics include qubit count, gate fidelity, T1/T2, connectivity, QV, and application performance; sourced from vendor documentation, published benchmarks, and independent studies.

**Key Findings:** Trapped-ion platforms achieve highest two-qubit gate fidelities (>99.9%) but slowest gate speeds; superconducting leads in qubit count and gate speed; photonic and neutral atom are most scalable for future fault tolerance; no single platform dominates across all metrics; all NISQ platforms are limited by noise for deep circuits.

**Relevance to PhD Research:** Provides the cross-platform hardware comparison context for the PhD's IBM-focused experiments — informs the generalisability of the PhD's noise characterisation and encoding recommendations to non-superconducting hardware.

---

### [P] Quantum Machine Learning on NISQ Devices: A Process-Oriented Study (Processes 2026)
**File:** [processes-14-02095 (4).pdf](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/processes-14-02095%20%284%29.pdf)
**Authors:** See paper (MDPI Processes, 2026)
**Year:** 2026
**Published In:** MDPI Processes 14, 2095 (2026)

**Research Problem:** The deployment pipeline for QML on NISQ devices — from data encoding through circuit execution to post-processing — is not systematically studied as a process, leaving practitioners without clear workflow guidance.

**Objectives:** To analyse the end-to-end QML deployment process on NISQ hardware, identifying bottlenecks, noise injection points, and optimisation opportunities at each workflow stage.

**Methodology:** Process modelling of the NISQ QML pipeline using BPMN notation; case studies on IBM Quantum; identifies 7 process stages (encoding, transpilation, execution, mitigation, post-processing, evaluation, iteration); measures time and noise contribution at each stage.

**Key Findings:** Encoding and transpilation account for 60% of circuit error accumulation; measurement readout errors contribute 15–25% of total error; ZNE post-processing reduces final output error by 20–30%; iterative noise-aware optimisation of the full pipeline outperforms stage-wise optimisation.

**Relevance to PhD Research:** Provides a process-level framework that directly aligns with the PhD's CADQE pipeline architecture — the 7-stage noise injection analysis validates the PhD's end-to-end noise-aware approach and identifies encoding as the dominant error source.

---



---

## Links

| Resource | URL |
|---|---|
| `main` branch | https://github.com/sajidalikhanphd/phd-references/tree/main |
| `Reference_Papers/` folder | https://github.com/sajidalikhanphd/phd-references/tree/main/Reference_Papers |
| `previous-uploads` branch | https://github.com/sajidalikhanphd/phd-references/tree/previous-uploads |
| Owner profile | https://github.com/sajidalikhanphd |

---

*108 papers · Summaries generated from actual PDF content · Repository maintained by [@sajidalikhanphd](https://github.com/sajidalikhanphd)*
