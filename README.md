# PhD Reference Papers — sajidalikhanphd

A curated collection of **108 research papers** supporting PhD research on
**Quantum Machine Learning (QML), NISQ devices, noise characterisation &
mitigation, variational quantum algorithms, and data encoding** — compiled by
[@sajidalikhanphd](https://github.com/sajidalikhanphd).

---

## Repository Structure

| Branch | Contents |
|---|---|
| [`main`](https://github.com/sajidalikhanphd/phd-references/tree/main) | 108 latest reference papers in `Reference_Papers/` + this README |
| [`previous-uploads`](https://github.com/sajidalikhanphd/phd-references/tree/previous-uploads) | Prior sessions: `pdfs/downloaded/`, `methodology-analysis/`, `library.bib` |

📁 **Direct folder link:**
[`Reference_Papers/`](https://github.com/sajidalikhanphd/phd-references/tree/main/Reference_Papers)
— 108 PDF files

---

## Paper Summaries by Theme

> Each entry links directly to the PDF in the repository.
> Papers are grouped thematically; the number prefix matches the original filename.

---

### 1 · Variational Quantum Algorithms & Ansatz Design

| # | Paper | Summary |
|---|---|---|
| 001 | [Review on Ansatz Architectures of VQAs for Continuous Optimization](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/001%20-%20Review%20on%20Ansatz%20Architectures%20of%20Variational%20Quantum%20Algorithms%20for%20Continuous%20Optimization%20-%20From%20Fixed%20Structures%20to%20Adaptive%20Evolution.pdf) | Comprehensive survey of fixed and adaptive ansatz designs for variational quantum algorithms, covering expressibility, trainability, and hardware constraints. |
| 022 | [Noisy Intermediate-Scale Quantum Algorithms](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/022%20-%20Noisy%20intermediate-scale%20quantum%20algorithms.pdf) | Foundational review of NISQ-era algorithms including VQE and QAOA, discussing their structure, applications, and near-term viability. |
| 039 | [Variational Quantum Algorithms (Cerezo, 2021)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/039.%20Variational%20quantum%20algorithms%20%28%5B39%5D%20Cerezo%29%20%282021%29%20%283%29.pdf) | Seminal comprehensive review of the VQA landscape — cost functions, optimisers, noise effects, and open research questions. |
| 047 | [Quantum Circuit Architecture Search for VQAs](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/047%20-%20Quantum%20circuit%20architecture%20search%20for%20variational%20quantum%20algorithms.pdf) | Proposes automated architecture search for VQA circuits, balancing expressibility and hardware noise constraints. |
| 054 | [Variational Quantum Circuits for Deep Reinforcement Learning](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/054%20-%20Variational%20quantum%20circuits%20for%20deep%20reinforcement%20learning.pdf) | Applies parameterised quantum circuits as function approximators in deep RL settings, benchmarking against classical baselines. |
| 080 | [Escaping Barren Plateau: Co-Exploration of Circuit Parameters and Architectures](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/080%20-%20Escaping%20Barren%20Plateau-%20Co-Exploration%20of%20Quantum%20Circuit%20Parameters%20and%20Architectures.pdf) | Joint optimisation of circuit structure and parameters to avoid barren plateaus, demonstrating improved trainability. |
| 113 | [TensorHyper-VQC: Tensor-Train-Guided Hypernetwork for Scalable VQC](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/113%20-%20TensorHyper-VQC-%20a%20tensor-train-guided%20hypernetwork%20for%20robust%20and%20scalable%20variational%20quantum%20computing.pdf) | Introduces a tensor-train hypernetwork framework to scale variational quantum circuits while maintaining noise robustness. |

---

### 2 · Data Encoding for Quantum Machine Learning

| # | Paper | Summary |
|---|---|---|
| 004 | [Effect of Data Encoding on Expressive Power of VQC Models (Schuld, 2021)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/004.%20Effect%20of%20data%20encoding%20on%20the%20expressive%20power%20of%20variational%20quantum-machine-learning%20models%20%28%5B4%5D%20Schuld%29%20%282021%29%20%283%29.pdf) | Analyses how the choice of encoding scheme determines the Fourier frequency spectrum a VQC can represent, linking encoding to model expressibility. |
| 005 | [Beyond Bits: A Review of Quantum Embedding Techniques](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/005%20-%20Beyond_Bits_A_Review_of_Quantum_Embedding_Techniques_for_Efficient_Information_Processing.pdf) | Surveys amplitude, angle, basis, and higher-order embedding strategies, evaluating their trade-offs for QML tasks. |
| 006 | [EnQode: Fast Amplitude Embedding for QML Using Classical Data](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/006%20-%20EnQode_Fast_Amplitude_Embedding_for_Quantum_Machine_Learning_Using_Classical_Data.pdf) | Presents an efficient algorithm for amplitude embedding that reduces circuit depth, enabling practical QML on classical datasets. |
| 007 | [Pulsed Learning for Quantum Data Re-Uploading Models](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/007%20-%20Pulsed%20learning%20for%20quantum%20data%20re-uploading%20models.pdf) | Extends the re-uploading framework using pulse-level control to improve data expressibility beyond gate-level encoding. |
| 010 | [Evaluating Angle and Amplitude Encoding Strategies for VQC (Tudisco, 2026)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/010.%20Evaluating%20Angle%20and%20Amplitude%20Encoding%20Strategies%20for%20Variational%20Quantum%20Machine%20Learning%20Their%20Impact%20on%20Model%27s%20Accuracy%20%28%5B10%5D%20Tudisco%29%20%282026%29%20%283%29.pdf) | Empirical comparison of angle vs. amplitude encoding across classification benchmarks, measuring accuracy and circuit cost. |
| 023 | [Quantum Data Encoding: A Comparative Analysis](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/023%20-%20Quantum%20data%20encoding%20-%20A%20comparative%20analysis%20of%20classicalto-quantum%20mapping%20techniques%20and%20their%20impact%20on%20machine%20learning%20accuracy.pdf) | Systematic comparison of classical-to-quantum mapping methods and their downstream effect on ML accuracy. |
| 024 | [QML: Exploring the Role of Data Encoding Techniques](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/024%20-%20Quantum%20machine%20learning%20-%20Exploring%20the%20role%20of%20data%20encoding%20techniques%2C%20challenges%2C%20and%20future%20directions.pdf) | Reviews encoding challenges and future directions, highlighting the central role encoding plays in QML model performance. |
| 027 | [Data Re-Uploading for a Universal Quantum Classifier](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/027%20-%20Data%20re-uploading%20for%20a%20universal%20quantum%20classifier.pdf) | Introduces the data re-uploading scheme, showing that repeated encoding of classical data enables universal quantum classification. |
| 028 | [Practical Insights on Encodings, Ansätze and Measurements in QCNNs (Lozano-Cruz, 2026)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/028.%20Practical%20insights%20on%20the%20effect%20of%20different%20encodings%2C%20ans%C3%A4tze%20and%20measurements%20in%20quantum%20and%20hybrid%20convolutional%20neural%20networks%20%28%5B28%5D%20Lozano-Cruz%29%20%282026%29.pdf) | Practical ablation study across encoding, ansatz, and measurement choices in quantum and hybrid CNNs. |
| 029 | [In-Depth Comparative Study of Quantum-Classical Encoding for Network Intrusion Detection](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/029%20-%20An_In-Depth_Comparative_Study_of_Quantum-Classical_Encoding_Methods_for_Network_Intrusion_Detection.pdf) | Applies and benchmarks multiple encoding methods on a cybersecurity intrusion detection task. |
| 030 | [Comparative Study of Encoding Strategies for Quantum Convolutional Neural Networks](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/030%20-%20A%20Comparative%20Study%20of%20Encoding%20Strategies%20for%20Quantum%20Convolutional%20Neural%20Networks.pdf) | Investigates how different encoding choices affect the accuracy and trainability of QCNNs. |
| 041 | [Drastic Circuit Depth Reductions with Preserved Adversarial Robustness via Approximate Encoding](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/041%20-%20Drastic%20circuit%20depth%20reductions%20with%20preserved%20adversarial%20robustness%20by%20approximate%20encoding%20for%20quantum%20machine%20learning.pdf) | Proposes approximate encoding to aggressively reduce circuit depth while retaining adversarial robustness of QML models. |
| 060 | [Empirical Power of Quantum Encoding Methods for Binary Classification](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/060%20-%20Empirical%20power%20of%20quantum%20encoding%20methods%20for%20binary%20classification.pdf) | Empirical evaluation of the discriminative power of various encoding strategies on binary classification benchmarks. |
| 061 | [Comparative Analysis of Quantum Encoding Techniques for Biomarker Classification](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/061%20-%20Comparative%20Analysis%20of%20Quantum%20Encoding%20Techniques%20for%20Biomarker%20Classification.pdf) | Applies and compares encoding strategies on biomedical biomarker datasets for disease classification. |
| 062 | [Data Encoding for VQC in Qiskit: A Comparison with Novel Hybrid Encoding](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/062%20-%20Data%20Encoding%20for%20VQC%20in%20Qiskit%2C%20A%20Comparison%20With%20Novel%20Hybrid%20Encoding.pdf) | Implements and benchmarks standard Qiskit encodings against a proposed hybrid encoding scheme. |

---

### 3 · Noise Characterisation & Mitigation

| # | Paper | Summary |
|---|---|---|
| 025 | [Scalable Mitigation of Measurement Errors on Quantum Computers](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/025%20-%20Scalable%20mitigation%20of%20measurement%20errors%20on%20quantum%20computers.pdf) | Introduces a scalable readout error mitigation scheme applicable to large qubit registers without full tomography. |
| 033 | [Software Mitigation of Crosstalk on NISQ Computers](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/033%20-%20Software%20mitigation%20of%20crosstalk%20on%20noisy%20intermediate-scale%20quantum%20computers.pdf) | Proposes compiler-level crosstalk mitigation using gate scheduling and qubit allocation strategies. |
| 034 | [Error Mitigation for Short-Depth Quantum Circuits (Temme, 2017)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/034.%20Error%20mitigation%20for%20short-depth%20quantum%20circuits%20%28%5B34%5D%20Temme%29%20%282017%29%20%283%29.pdf) | Foundational paper introducing quasi-probability decomposition and zero-noise extrapolation for error mitigation. |
| 035 | [Probabilistic Error Cancellation with Sparse Pauli–Lindblad Models](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/035%20-%20Probabilistic%20error%20cancellation%20with%20sparse%20Pauli%E2%80%93Lindblad%20models%20on%20noisy%20quantum%20processors.pdf) | Advances probabilistic error cancellation using sparse noise models learned from device calibration data. |
| 037 | [Modeling and Simulating the Noisy Behavior of Near-Term Quantum Computers](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/037%20-%20Modeling%20and%20simulating%20the%20noisy%20behavior%20of%20near-term%20quantum%20computers.pdf) | Develops noise models for NISQ devices and validates them against real hardware, guiding realistic simulation. |
| 040 | [Quantum Noise in the Flow of Time: A Temporal Study](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/040%20-%20Quantum%20noise%20in%20the%20flow%20of%20time%20-%20A%20temporal%20study%20of%20the%20noise%20in%20quantum%20computers.pdf) | Studies how qubit noise characteristics drift over time, motivating temporally-adaptive calibration strategies. |
| 046 | [Analytic Model of Fidelity under Depolarizing Noise (Escofet, 2025)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/046.%20An%20accurate%20and%20efficient%20analytic%20model%20of%20fidelity%20under%20depolarizing%20noise%20oriented%20to%20large%20scale%20quantum%20system%20design%20%28%5B46%5D%20Escofet%29%20%282025%29%20%283%29.pdf) | Derives an efficient closed-form fidelity model under depolarizing noise for large-scale system design space exploration. |
| 053 | [Adaptive Quantum Error Mitigation Using Machine Learning in NISQ Systems](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/053%20-%20Adaptive%20Quantum%20Error%20Mitigation%20Using%20Machine%20Learning%20in%20Noisy%20Intermediate-Scale%20Quantum%20Systems.pdf) | Uses ML to adaptively select and tune error mitigation techniques based on real-time noise characterisation. |
| 057 | [Noisy Quantum Kernel Machines](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/057%20-%20Noisy%20quantum%20kernel%20machines.pdf) | Analyses how hardware noise degrades quantum kernel methods and derives conditions under which they remain classically simulable. |
| 064 | [Quantifying the Effects of Noise in a Quantum Convolutional Neural Network](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/064%20-%20Quantifying%20the%20effects%20of%20noise%20in%20a%20quantum%20convolutional%20neural%20network.pdf) | Systematic noise impact study on QCNN architectures, quantifying accuracy degradation under realistic noise models. |
| 065 | [Performance Analysis and Noise Impact of a Novel Quantum KNN Algorithm](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/065%20-%20Performance%20Analysis%20and%20Noise%20Impact%20of%20a%20Novel%20Quantum%20KNN%20Algorithm%20for%20Machine%20Learning.pdf) | Introduces a quantum k-nearest-neighbours algorithm and analyses its sensitivity to gate and readout noise. |
| 067 | [Machine Learning for Practical Quantum Error Mitigation](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/067%20-%20Machine%20learning%20for%20practical%20quantum%20error%20mitigation.pdf) | Trains classical ML models on circuit-execution data to predict and correct quantum errors without full tomography. |
| 077 | [Optimized Noise Suppression for Quantum Circuits](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/077%20-%20Optimized%20noise%20suppression%20for%20quantum%20circuits.pdf) | Develops circuit-level noise suppression techniques by jointly optimising gate sequences and dynamical decoupling pulses. |
| 111 | [Estimating the Effect of Crosstalk Error on Circuit Fidelity on NISQ Devices](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/111%20-%20Estimating%20the%20effect%20of%20crosstalk%20error%20on%20circuit%20fidelity%20using%20noisy%20intermediate-scale%20quantum%20devices.pdf) | Develops an analytical model to estimate fidelity loss from crosstalk, enabling better qubit-mapping decisions. |
| 114 | [Tackling Coherent Noise via Cross-Layer Compiler Optimization](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/114%20-%20Tackling%20coherent%20noise%20in%20quantum%20computing%20via%20cross-layer%20compiler%20optimization.pdf) | Addresses coherent noise sources through cross-layer compiler strategies spanning gate synthesis and pulse scheduling. |

---

### 4 · Barren Plateaus

| # | Paper | Summary |
|---|---|---|
| 011 | [Barren Plateaus in Quantum Neural Network Training Landscapes](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/011%20-%20Barren%20plateaus%20in%20quantum%20neural%20network%20training%20landscapes.pdf) | Original paper identifying the barren plateau problem — exponentially vanishing gradients in deep random quantum circuits. |
| 012 | [Barren Plateaus in Variational Quantum Computing](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/012%20-%20Barren%20plateaus%20in%20variational%20quantum%20computing.pdf) | Comprehensive review of barren plateau causes, diagnostics, and mitigation strategies across VQC architectures. |
| 069 | [Noise-Induced Barren Plateaus in Variational Quantum Algorithms](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/069%20-%20Noise-induced%20barren%20plateaus%20in%20variational%20quantum%20algorithms.pdf) | Shows that hardware noise independently causes barren plateaus even in shallow circuits, independent of random initialisation. |
| 071 | [Emergence of Noise-Induced Barren Plateaus in Arbitrary Layered Noise Models](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/071%20-%20Emergence%20of%20noise-induced%20barren%20plateaus%20in%20arbitrary%20layered%20noise%20models.pdf) | Proves that noise-induced barren plateaus arise under general layered noise models, extending the theoretical framework. |
| 072 | [Cost Function Dependent Barren Plateaus in Shallow Parametrized Quantum Circuits](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/072%20-%20Cost%20function%20dependent%20barren%20plateaus%20in%20shallow%20parametrized%20quantum%20circuits.pdf) | Demonstrates that the choice of cost function — local vs. global — determines whether shallow circuits suffer barren plateaus. |
| 073 | [Connecting Ansatz Expressibility to Gradient Magnitudes and Barren Plateaus](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/073%20-%20Connecting%20ansatz%20expressibility%20to%20gradient%20magnitudes%20and%20barren%20plateaus.pdf) | Establishes a formal link between a circuit's expressibility measure and the magnitude of its training gradients. |
| 074 | [A Lie Algebraic Theory of Barren Plateaus for Deep Parameterized Quantum Circuits](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/074%20-%20A%20lie%20algebraic%20theory%20of%20barren%20plateaus%20for%20deep%20parameterized%20quantum%20circuits.pdf) | Provides a Lie algebraic characterisation of when deep circuits exhibit barren plateaus, enabling architecture-level avoidance. |
| 075 | [Investigating and Mitigating Barren Plateaus in VQCs: A Survey](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/075%20-%20Investigating%20and%20mitigating%20barren%20plateaus%20in%20variational%20quantum%20circuits-%20a%20survey-%20J.pdf) | Survey of diagnostics, theoretical results, and practical mitigation techniques for barren plateaus across VQC settings. |

---

### 5 · Transpilation, Qubit Mapping & Circuit Compilation

| # | Paper | Summary |
|---|---|---|
| 003 | [Just-in-Time Quantum Circuit Transpilation Reduces Noise (Wilson, 2020)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/003.%20Just-in-time%20quantum%20circuit%20transpilation%20reduces%20noise%20%28%5B3%5D%20Wilson%29%20%282020%29%20%283%29.pdf) | Introduces just-in-time transpilation that re-compiles circuits using the most recent device calibration data to minimise noise. |
| 008 | [QuantumNAS: Noise-Adaptive Search for Robust Quantum Circuits (Wang, 2022)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/008.%20Quantumnas%20Noise-adaptive%20search%20for%20robust%20quantum%20circuits%20%28%5B8%5D%20Wang%29%20%282022%29%20%283%29.pdf) | Neural architecture search framework that jointly searches for circuit structure and qubit mapping to maximise noise resilience. |
| 009 | [Noise-Adaptive Compiler Mappings for NISQ Computers](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/009%20-%20Noise-adaptive%20compiler%20mappings%20for%20noisy%20intermediate-scale%20quantum%20computers.pdf) | Develops noise-aware qubit-to-hardware mapping strategies at compile time to reduce gate error rates. |
| 031 | [Hardware-Aware Calibration Protocol for Quantum Computers](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/031%20-%20Hardware-aware%20calibration%20protocol%20for%20quantum%20computers.pdf) | Presents a calibration protocol that adapts to hardware characteristics, improving gate fidelity through targeted tuning. |
| 043 | [Addressing Temporal Variations in Qubit Quality Metrics (Alam, 2019)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/043.%20Addressing%20temporal%20variations%20in%20qubit%20quality%20metrics%20for%20parameterized%20quantum%20circuits%20%28%5B43%5D%20Alam%29%20%282019%29%20%283%29.pdf) | Proposes recalibration-aware scheduling to handle time-varying qubit coherence and gate fidelity on real hardware. |
| 048 | [Noise-Aware Quantum Architecture Search Based on NSGA-II](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/048%20-%20Noise-Aware%20Quantum%20Architecture%20Search%20Based%20on%20NSGA-II%20Algorithm.pdf) | Multi-objective evolutionary architecture search balancing circuit expressibility and hardware noise sensitivity. |
| 049 | [Revisiting Noise-Adaptive Transpilation: How Much Impact Does it Have?](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/049%20-%20Revisiting%20Noise-adaptive%20Transpilation%20in%20Quantum%20Computing%20-%20How%20Much%20Impact%20Does%20it%20Have.pdf) | Empirical reassessment of noise-adaptive transpilation gains on modern IBM hardware, questioning previously reported benefits. |
| 076 | [A Hardware-Aware Heuristic for the Qubit Mapping Problem in the NISQ Era](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/076%20-%20A%20hardware-aware%20heuristic%20for%20the%20qubit%20mapping%20problem%20in%20the%20nisq%20era.pdf) | Proposes a heuristic qubit-mapping algorithm that accounts for hardware topology and gate error rates. |
| 079 | [Pulse-Efficient Circuit Transpilation for Cross-Resonance-Based Hardware](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/079%20-%20Pulse-efficient%20circuit%20transpilation%20for%20quantum%20applications%20on%20cross-resonance-based%20hardware.pdf) | Optimises circuit execution at the pulse level on IBM cross-resonance hardware, reducing effective gate error. |

---

### 6 · Quantum Kernel Methods & Support Vector Machines

| # | Paper | Summary |
|---|---|---|
| 017 | [Supervised Learning with Quantum-Enhanced Feature Spaces (Havlíček, 2019)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/017.%20Supervised%20learning%20with%20quantum-enhanced%20feature%20spaces%20%28%5B17%5D%20Havl%C3%AD%C4%8Dek%29%20%282019%29.pdf) | Demonstrates quantum-enhanced kernel estimation on real hardware, proposing quantum feature maps for SVMs. |
| 020 | [Universal Expressiveness of Variational Quantum Classifiers and Quantum Kernels for SVMs](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/020%20-%20Universal%20expressiveness%20of%20variational%20quantum%20classifiers%20and%20quantum%20kernels%20for%20support%20vector%20machines.pdf) | Proves universal expressiveness of quantum kernel SVMs and VQCs under mild circuit depth conditions. |
| 056 | [Quantum SVMs for Classification and Regression on a Trapped-Ion Quantum Computer](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/056%20-%20Quantum%20support%20vector%20machines%20for%20classification%20and%20regression%20on%20a%20trapped-ion%20quantum%20computer.pdf) | Experimental demonstration of quantum SVMs on trapped-ion hardware for both classification and regression tasks. |
| 058 | [Comprehensive Comparative Analysis of VQC and Quantum Kernel SVM Under NISQ Noise](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/058%20-%20Comprehensive%20Comparative%20Analysis%20of%20Variational%20Quantum%20Classifier%20and%20Quantum%20Kernel%20SVM%20Under%20NISQ%20Noise%20with%20Classical%20Baseline%20and%20Statistical%20Significance%20Evaluation.pdf) | Head-to-head comparison of VQC and quantum kernel SVM under realistic NISQ noise with statistical significance testing. |
| 112 | [Comparative Analysis of Quantum Kernel Methods and VQCs for Financial Fraud Detection](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/112%20-%20Comparative%20Analysis%20and%20Noise%20Robustness%20Study%20of%20Quantum%20Kernel%20Methods%20and%20Variational%20Quantum%20Classifiers%20for%20Financial%20Fraud%20Detection.pdf) | Applies and compares quantum kernel and VQC approaches to financial fraud detection under hardware noise. |

---

### 7 · QML Training, Optimisation & Neural Networks

| # | Paper | Summary |
|---|---|---|
| 018 | [Evaluating Analytic Gradients on Quantum Hardware (Schuld, 2019)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/018.%20Evaluating%20analytic%20gradients%20on%20quantum%20hardware%20%28%5B18%5D%20Schuld%29%20%282019%29%20%283%29.pdf) | Derives the parameter-shift rule for computing exact gradients of quantum circuits on real hardware. |
| 019 | [Expressibility and Entangling Capability of Parameterized Quantum Circuits (Sim, 2019)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/019.%20Expressibility%20and%20entangling%20capability%20of%20parameterized%20quantum%20circuits%20for%20hybrid%20quantum%E2%80%90classical%20algorithms%20%28%5B19%5D%20Sim%29%20%282019%29.pdf) | Defines and measures expressibility and entangling capability metrics for PQC benchmarking. |
| 021 | [A Novel Spatial-Temporal VQC to Enable Deep Learning on NISQ Devices](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/021%20-%20A_Novel_Spatial-Temporal_Variational_Quantum_Circuit_to_Enable_Deep_Learning_on_NISQ_Devices.pdf) | Designs a spatial-temporal VQC architecture enabling deep-learning-like representation on NISQ hardware. |
| 038 | [Layerwise Learning for Quantum Neural Networks](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/038%20-%20Layerwise%20learning%20for%20quantum%20neural%20networks.pdf) | Proposes progressive layer-by-layer training to avoid barren plateaus and improve convergence of deep QNNs. |
| 059 | [A Comparative Analysis and Noise Robustness Evaluation in Quantum Neural Networks](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/059%20-%20A%20comparative%20analysis%20and%20noise%20robustness%20evaluation%20in%20quantum%20neural%20networks.pdf) | Benchmarks multiple QNN architectures under varying noise levels, ranking their robustness to hardware imperfections. |
| 063 | [QML with Qiskit: Evaluating Regression Accuracy and Noise Impact](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/063%20-%20Quantum%20machine%20learning%20with%20Qiskit-%20Evaluating%20regression%20accuracy%20and%20noise%20impact.pdf) | Implements QML regression models in Qiskit and measures how noise levels affect prediction accuracy across datasets. |
| 068 | [Variational Quantum Machine Learning with Quantum Error Detection](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/068%20-%20Variational%20quantum%20machine%20learning%20with%20quantum%20error%20detection.pdf) | Integrates error detection codes into VQC training loops to improve model reliability on noisy hardware. |
| 078 | [Machine Learning of Noise-Resilient Quantum Circuits](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/078%20-%20Machine%20learning%20of%20noise-resilient%20quantum%20circuits.pdf) | Uses classical ML to discover circuit structures that are inherently robust to specific hardware noise profiles. |
| 066 | [NAC-QFL: Noise-Aware Clustered Quantum Federated Learning](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/066%20-%20NAC-QFL-%20Noise%20aware%20clustered%20quantum%20federated%20learning.pdf) | Extends federated learning to quantum settings with noise-aware client clustering to improve aggregation quality. |
| 070 | [Domain-Aware Quantum Circuit for QML](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/070%20-%20Domain-Aware%20Quantum%20Circuit%20for%20QML.pdf) | Incorporates domain-specific inductive biases into quantum circuit design to improve sample efficiency and accuracy. |

---

### 8 · Quantum ML Foundations & Reviews

| # | Paper | Summary |
|---|---|---|
| 013 | [Quantum Machine Learning (Biamonte, 2017)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/013.%20Quantum%20machine%20learning%20%28%5B13%5D%20Biamonte%29%20%282017%29.pdf) | Landmark Nature paper reviewing the intersection of quantum computing and machine learning, outlining prospects and caveats. |
| 014 | [Quantum Computation and Quantum Information — Book](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/014%20-%20Quantum%20computation%20and%20quantum%20information%20-%20Book.pdf) | Nielsen & Chuang's definitive textbook covering quantum gates, algorithms, error correction, and complexity theory. |
| 036 | [A Primer on Quantum Machine Learning](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/036%20-%20A%20primer%20on%20quantum%20machine%20learning.pdf) | Accessible introduction to QML covering supervised, unsupervised, and reinforcement learning paradigms on quantum hardware. |
| 044 | [A Comprehensive Review of QML: From NISQ to Fault Tolerance](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/044%20-%20A%20comprehensive%20review%20of%20quantum%20machine%20learning-%20from%20NISQ%20to%20fault%20tolerance.pdf) | Broad literature review spanning NISQ-era QML models through to fault-tolerant quantum learning algorithms. |
| 045 | [Better Than Classical? The Subtle Art of Benchmarking QML Models](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/045%20-%20Better%20than%20classical%20the%20subtle%20art%20of%20benchmarking%20quantum%20machine%20learning%20models.pdf) | Critical analysis of benchmarking methodology for QML, identifying common pitfalls that overstate quantum advantage. |
| 055 | [QML on Near-Term Quantum Devices: Current State of Supervised and Unsupervised Techniques](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/055%20-%20Quantum%20machine%20learning%20on%20near-term%20quantum%20devices-%20Current%20state%20of%20supervised%20and%20unsupervised%20techniques%20for%20real-world%20applications.pdf) | Reviews the state of supervised and unsupervised QML on NISQ hardware, cataloguing real-world application attempts. |
| 002 | [Evidence for the Utility of Quantum Computing Before Fault Tolerance](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/002%20-%20Evidence%20for%20the%20utility%20of%20quantum%20computing%20before%20fault%20tolerance.pdf) | IBM's landmark 127-qubit experiment showing practical quantum utility on classically intractable Ising model simulations. |
| processes | [Processes-14-02095: QML Process Study](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/processes-14-02095%20%284%29.pdf) | Published process-oriented study (MDPI *Processes*) examining QML workflow integration within scientific computing pipelines. |

---

### 9 · Adversarial Robustness in QML

| # | Paper | Summary |
|---|---|---|
| 026 | [Towards Quantum-Enhanced Adversarial Robustness in ML (West, 2023)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/026.%20Towards%20quantum%20enhanced%20adversarial%20robustness%20in%20machine%20learning%20%28%5B26%5D%20West%29%20%282023%29%20%283%29.pdf) | Investigates whether quantum models offer inherent adversarial robustness advantages over classical counterparts. |

---

### 10 · Superconducting Qubits & Hardware

| # | Paper | Summary |
|---|---|---|
| 016 | [A Quantum Engineer's Guide to Superconducting Qubits](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/016%20-%20A%20quantum%20engineer%27s%20guide%20to%20superconducting%20qubits.pdf) | In-depth engineering guide covering qubit types, fabrication, control electronics, and decoherence sources. |
| 110 | [Superconducting Quantum Computers — Who is Leading the Future?](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/110%20-Superconducting%20quantum%20computers%20-%20who%20is%20leading%20the%20future.pdf) | Comparative review of superconducting quantum computer roadmaps from IBM, Google, Rigetti, and others. |
| 116 | [Comparative Analysis of Contemporary Quantum Computer Processors](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/116%20-%20Comparative%20analysis%20of%20contemporary%20quantum%20computer%20processors-%20architectures%2C%20performance%20and%20perspectives.pdf) | Cross-platform benchmarking of quantum processors covering architecture differences, gate fidelities, and connectivity. |

---

### 11 · QML in Healthcare & Medicine

| # | Paper | Summary |
|---|---|---|
| 050 | [A Systematic Review of QML for Digital Health](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/050%20-%20A%20systematic%20review%20of%20quantum%20machine%20learning%20for%20digital%20health.pdf) | Systematic literature review of QML applications in digital health, covering imaging, genomics, and clinical data. |
| 051 | [QML in Medical Image Analysis: From Diagnostics to Surgery Planning](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/051%20-%20Quantum%20Machine%20Learning%20in%20Medical%20Image%20Analysis-%20From%20Diagnostics%20to%20Surgery%20Planning.pdf) | Reviews QML approaches to medical image analysis tasks including classification, segmentation, and surgical planning. |
| 052 | [QML and Data Re-Uploading: Evaluation on Benchmark and Laboratory Medicine Data Sets](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/052%20-%20Quantum%20Machine%20Learning%20and%20Data%20Re-Uploading-%20Evaluation%20on%20Benchmark%20and%20Laboratory%20Medicine%20Data%20Sets.pdf) | Applies re-uploading models to laboratory medicine datasets, evaluating performance against classical baselines. |
| 093 | [Investigating QML in Breast Cancer: A Systematic Review](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/093%20-%20Investigating%20the%20application%20of%20quantum%20machine%20learning%20in%20breast%20cancer%20-%20a%20systematic%20review%20-%20quantum%20machine%20learning%20in%20bc.pdf) | Systematic review of QML applications specifically in breast cancer detection, staging, and prognosis. |
| 094 | [Quantum Computing Revolution in Healthcare: A Systematic Review](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/094%20-%20Quantum%20computing%20revolution%20in%20healthcare-%20a%20systematic%20review%20of%20applications%2C%20issues%20and%20future%20directions.pdf) | Broad systematic review of quantum computing across healthcare — drug discovery, diagnostics, and personalised medicine. |
| 095 | [Applications of Quantum Computing in Clinical Care](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/095%20-%20Applications%20of%20quantum%20computing%20in%20clinical%20care.pdf) | Surveys quantum computing applications in clinical workflows including optimisation, scheduling, and outcome prediction. |

---

### 12 · Quantum Computing Industry, Society & Education

| # | Paper | Summary |
|---|---|---|
| 096 | [Industry Quantum Computing Applications](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/096%20-%20Industry%20quantum%20computing%20applications.pdf) | Overview of quantum computing use cases across finance, logistics, energy, and manufacturing sectors. |
| 099 | [Quantum for Good and the Societal Impact of Quantum Computing](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/099%20-%20Quantum%20for%20good%20and%20the%20societal%20impact%20of%20quantum%20computing.pdf) | Discusses the broader societal, ethical, and geopolitical implications of quantum computing development. |
| 100 | [The Economics of an Open-Source Quantum Computer](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/100%20-%20The%20Economics%20of%20an%20Open-Source%20Quantum%20Computer.pdf) | Analyses the economic model and open-source ecosystem around publicly accessible quantum computing platforms. |
| 101 | [Mapping Quantum Industry Demands to Education](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/101%20-%20Mapping%20quantum%20industry%20demands%20to%20education-%20a%20critical%20analysis%20of%20skills%2C%20qualifications%2C%20and%20modalities.pdf) | Critical analysis of the skills gap between quantum industry requirements and existing educational qualifications. |
| 104 | [Advancing Quantum Technology Workforce: Industry Insights](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/104%20-%20Advancing%20quantum%20technology%20workforce%20-%20industry%20insights%20into%20qualification%20and%20training%20needs.pdf) | Industry survey of training and qualification needs for building a skilled quantum technology workforce. |
| 105 | [Assessing the Needs of the Quantum Industry](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/105%20-%20Assessing%20the%20needs%20of%20the%20quantum%20industry.pdf) | Policy-oriented assessment of infrastructure, talent, and regulatory needs for quantum industry development. |
| 107 | [Evolution of Quantum Computing: Theoretical and Innovation Management Implications](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/107%20-%20Evolution%20of%20quantum%20computing-%20Theoretical%20and%20innovation%20management%20implications%20for%20emerging%20quantum%20industry.pdf) | Studies the innovation management and technology trajectory of quantum computing from a management science perspective. |
| 115 | [Exploring Quantum Technologies for Industrial and Real-World Use Cases](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/115%20-%20Exploring%20the%20application%20of%20quantum%20technologies%20to%20industrial%20and%20real-world%20use%20cases-%20E.pdf) | Documents real-world pilot deployments of quantum technologies across industrial sectors with lessons learned. |

---

### 13 · Quantum Benchmarking

| # | Paper | Summary |
|---|---|---|
| 097 | [Metriq: A Collaborative Platform for Benchmarking Quantum Computers](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/097%20-%20Metriq-%20A%20Collaborative%20Platform%20for%20Benchmarking%20Quantum%20Computers.pdf) | Describes the Metriq open platform for community-driven, reproducible benchmarking of quantum devices. |
| 098 | [Benchmarking Quantum Computers](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/098%20-%20Benchmarking%20quantum%20computers.pdf) | Reviews established and emerging benchmarking methodologies including quantum volume, randomised benchmarking, and application benchmarks. |
| 102 | [QASMbench: A Low-Level Quantum Benchmark Suite for NISQ Evaluation](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/102%20-%20Qasmbench-%20A%20low-level%20quantum%20benchmark%20suite%20for%20nisq%20evaluation%20and%20simulation.pdf) | Presents QASMbench, a low-level OpenQASM benchmark suite covering diverse application domains for NISQ device evaluation. |
| 103 | [SupermarQ: A Scalable Quantum Benchmark Suite](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/103%20-%20Supermarq-%20A%20scalable%20quantum%20benchmark%20suite.pdf) | Introduces SupermarQ, a feature-vector-based benchmark suite that correlates circuit features with hardware performance. |
| 106 | [Application-Oriented Performance Benchmarks for Quantum Computing](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/106%20-%20Application-oriented%20performance%20benchmarks%20for%20quantum%20computing.pdf) | Proposes application-level benchmarks that measure end-to-end quantum computing performance on practical problem instances. |
| 108 | [IBM Quantum Computers: Evolution, Performance, and Future Directions](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/108%20-%20IBM%20quantum%20computers-%20evolution%2C%20performance%2C%20and%20future%20directions-%20M.pdf) | Tracks IBM's quantum hardware evolution from 5-qubit systems to 100+ qubit processors, analysing performance trends. |
| 109 | [Quantum Volume in Practice: What Users Can Expect from NISQ Devices](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/109%20-%20Quantum%20volume%20in%20practice-%20What%20users%20can%20expect%20from%20NISQ%20devices.pdf) | Practical analysis of the quantum volume metric across multiple NISQ devices, helping users set realistic performance expectations. |

---

### 14 · Research Methodology & Systematic Reviews

| # | Paper | Summary |
|---|---|---|
| 083 | [FEDS: A Framework for Evaluation in Design Science Research](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/083%20-%20FEDS-%20a%20framework%20for%20evaluation%20in%20design%20science%20research.pdf) | Presents the FEDS framework for systematically planning and reporting evaluation in design science research projects. |
| 084 | [Design Science Methodology for IS and Software Engineering (Wieringa, 2014)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/084.%20Design%20science%20methodology%20for%20information%20systems%20and%20software%20engineering%20%28%5B84%5D%20Wieringa%29%20%282014%29%20%283%29.pdf) | Foundational design science research methodology textbook covering problem investigation, design, and validation cycles. |
| 085 | [The PRISMA 2020 Statement: Updated Guideline for Systematic Reviews](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/085%20-%20The%20PRISMA%202020%20statement-%20an%20updated%20guideline%20for%20reporting%20systematic%20reviews.pdf) | Updated PRISMA reporting guidelines for systematic reviews and meta-analyses, including new flow diagram and checklist items. |
| 088 | [Methodology to Select and Adjust Quantum Noise Models (Bravo-Montes, 2024)](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/088.%20A%20methodology%20to%20select%20and%20adjust%20quantum%20noise%20models%20through%20emulators%20benchmarking%20against%20real%20backends%20%28%5B88%5D%20Bravo-Montes%29%20%282024%29%20%283%29.pdf) | Defines a methodology for selecting and calibrating quantum noise models using emulator-to-hardware benchmarking. |
| 090 | [Evaluation Metrics and Statistical Tests for Machine Learning](https://github.com/sajidalikhanphd/phd-references/blob/main/Reference_Papers/090%20-%20Evaluation%20metrics%20and%20statistical%20tests%20for%20machine%20learning.pdf) | Reference guide for ML evaluation metrics and statistical hypothesis tests appropriate for comparing model performance. |

---

## Links

| Resource | URL |
|---|---|
| `main` branch | https://github.com/sajidalikhanphd/phd-references/tree/main |
| `Reference_Papers/` folder | https://github.com/sajidalikhanphd/phd-references/tree/main/Reference_Papers |
| `previous-uploads` branch | https://github.com/sajidalikhanphd/phd-references/tree/previous-uploads |
| Owner profile | https://github.com/sajidalikhanphd |

---

*108 papers · Last updated: 2025 · Repository maintained by [@sajidalikhanphd](https://github.com/sajidalikhanphd)*
