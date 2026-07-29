# phd-references

> **CADQE PhD Research Programme — Master Reference Library**
> Calibration-Adaptive Data-to-Quantum Encoding: A Framework for Noise-Responsive Encoding Optimisation in Quantum Machine Learning
>
> **Candidate:** Sajid Ali Khan · **GitHub:** [@sajidalikhanphd](https://github.com/sajidalikhanphd)
> **Visibility:** 🌐 Public · **Licence:** CC BY 4.0 (bibliography data and PDFs)

---

## Repository Contents

| Path | Description |
|---|---|
| [`library.bib`](library.bib) | Master BibTeX library — seed entries for all CADQE core references |
| [`pdfs/downloaded/`](pdfs/downloaded/) | 48 peer-reviewed papers (PDFs) supporting the CADQE research programme |

---

## Paper Archive — `pdfs/downloaded/`

48 papers are archived here, drawn from the full 116-paper CADQE reference list. They are organised into **8 thematic categories** that map directly to the CADQE research programme's chapters and experiments.

---

### Category 1 — Foundational QML & NISQ Theory
*Core papers establishing quantum machine learning as a field and the NISQ hardware paradigm.*

| # | File | Reference | Key Contribution |
|---|---|---|---|
| 004 | [004_Evidence_for_the_utility_of_quantum_computing_before_fault_tolerance.pdf](pdfs/downloaded/004_Evidence_for_the_utility_of_quantum_computing_before_fault_tolerance.pdf) | Kim et al. (2023). *Nature*, 618, 500–505. | First empirical demonstration of quantum utility on 127-qubit IBM Eagle before fault tolerance; validates NISQ-era hardware as a meaningful research platform |
| 026 | [026_Quantum_machine_learning.pdf](pdfs/downloaded/026_Quantum_machine_learning.pdf) | Biamonte et al. (2017). *Nature*, 549, 195–202. | **Foundational CADQE paper.** Establishes QML as a research field; identifies data encoding as a fundamental open problem — the nine-year gap that CADQE addresses |
| 028 | [028_Quantum_computation_and_quantum_information.pdf](pdfs/downloaded/028_Quantum_computation_and_quantum_information.pdf) | Nielsen & Chuang (2010). *Cambridge University Press.* | The standard textbook for quantum information theory; provides the Kraus operator formalism, depolarising channel, and density matrix mathematics underlying CADQE's C2 fidelity decay law |
| 072 | [072_A_primer_on_quantum_machine_learning.pdf](pdfs/downloaded/072_A_primer_on_quantum_machine_learning.pdf) | Chang & Cerezo (2025). *arXiv:2511.15969.* | Comprehensive modern survey of QML; situates CADQE within the current landscape of variational and kernel-based quantum algorithms |
| 078 | [078_Variational_quantum_algorithms.pdf](pdfs/downloaded/078_Variational_quantum_algorithms.pdf) | Cerezo et al. (2021). *Nature Reviews Physics*, 3, 625–644. | Seminal VQC survey; establishes the two-stage encoding + variational ansatz architecture that CADQE's C1 breaks by making the encoding stage adaptive |

---

### Category 2 — Data Encoding Strategies & Expressibility
*Papers directly informing CADQE's six candidate encoding families and the encoding selection logic of C1.*

| # | File | Reference | Key Contribution |
|---|---|---|---|
| 008 | [008_Effect_of_data_encoding_on_the_expressive_power_of_variational_quantum_machine_l.pdf](pdfs/downloaded/008_Effect_of_data_encoding_on_the_expressive_power_of_variational_quantum_machine_l.pdf) | Schuld, Sweke & Meyer (2021). *Physical Review A*, 103, 032430. | Formal theory of how encoding choice determines the expressibility and Fourier spectrum of VQC models; theoretical foundation for CADQE's expressibility metric |
| 010 | [010_Beyond_bits_A_review_of_quantum_embedding_techniques_for_efficient_information_p.pdf](pdfs/downloaded/010_Beyond_bits_A_review_of_quantum_embedding_techniques_for_efficient_information_p.pdf) | Khan et al. (2024). *IEEE Access*, 12, 46118–46137. | Comprehensive review of quantum embedding techniques; taxonomy of encoding families used in CADQE's candidate set ℰ |
| 020 | [020_Evaluating_Angle_and_Amplitude_Encoding_Strategies_for_Variational_Quantum_Machi.pdf](pdfs/downloaded/020_Evaluating_Angle_and_Amplitude_Encoding_Strategies_for_Variational_Quantum_Machi.pdf) | Tudisco et al. (2026). *Advanced Quantum Technologies*, 9(4), e00611. | **PRIMARY MOTIVATION PAPER.** Empirically demonstrates 10–41% classification accuracy gap attributable purely to encoding strategy choice across 12 datasets and 5 VQC architectures — the core empirical finding driving the entire CADQE research programme |
| 034 | [034_Supervised_learning_with_quantum_enhanced_feature_spaces.pdf](pdfs/downloaded/034_Supervised_learning_with_quantum_enhanced_feature_spaces.pdf) | Havlíček et al. (2019). *Nature*, 567, 209–212. | Introduces the IQP/ZZ Feature Map encoding and quantum kernel methods; proves a quantum advantage conjecture for the resulting kernel — directly informs CADQE's highest-expressibility encoding candidate |
| 038 | [038_Expressibility_and_entangling_capability_of_parameterized_quantum_circuits_for_h.pdf](pdfs/downloaded/038_Expressibility_and_entangling_capability_of_parameterized_quantum_circuits_for_h.pdf) | Sim, Johnson & Aspuru-Guzik (2019). *Advanced Quantum Technologies*, 2(12), 1900070. | Defines and quantifies expressibility and entangling capability metrics for VQCs; the expressibility scale used by CADQE's C1 selector (0.1–0.9) is grounded in this work |
| 040 | [040_Universal_expressiveness_of_variational_quantum_classifiers_and_quantum_kernels_.pdf](pdfs/downloaded/040_Universal_expressiveness_of_variational_quantum_classifiers_and_quantum_kernels_.pdf) | Jäger & Krems (2023). *Nature Communications*, 14, 576. | Proves PROMISEBQP-completeness of IQP-based kernels — establishes the maximum theoretical expressibility of CADQE's IQP encoding candidate |
| 046 | [046_Quantum_data_encoding_A_comparative_analysis_of_classicalto_quantum_mapping_tech.pdf](pdfs/downloaded/046_Quantum_data_encoding_A_comparative_analysis_of_classicalto_quantum_mapping_tech.pdf) | Rath & Date (2023). *arXiv:2311.10375.* | Comparative analysis of classical-to-quantum mapping techniques across angle, amplitude, and basis encoding families; provides cross-encoding accuracy benchmarks |
| 054 | [054_Data_re_uploading_for_a_universal_quantum_classifier.pdf](pdfs/downloaded/054_Data_re_uploading_for_a_universal_quantum_classifier.pdf) | Pérez-Salinas et al. (2020). *Quantum*, 4, 226. | Introduces data re-uploading encoding; proves universal approximation capability; CADQE's re-uploading candidate with adaptive L = 1–3 layer scheduling derives from this work |
| 056 | [056_Practical_insights_on_the_effect_of_different_encodings_ansätze_and_measurements.pdf](pdfs/downloaded/056_Practical_insights_on_the_effect_of_different_encodings_ansätze_and_measurements.pdf) | Lozano-Cruz et al. (2026). *Quantum Machine Intelligence*, 8(1), 49. | Practical empirical study of encoding × ansatz × measurement interactions; confirms encoding as the dominant performance driver in hybrid convolutional QNNs |

---

### Category 3 — Noise, Fidelity & NISQ Hardware Characterisation
*Papers directly informing CADQE's Contribution C2: the Unified Fidelity Decay Law and d_max formula.*

| # | File | Reference | Key Contribution |
|---|---|---|---|
| 006 | [006_Just_in_time_quantum_circuit_transpilation_reduces_noise.pdf](pdfs/downloaded/006_Just_in_time_quantum_circuit_transpilation_reduces_noise.pdf) | Wilson, Singh & Mueller (2020). *IEEE QCE*, pp. 345–355. | Demonstrates 3–304% accuracy improvement by querying fresh calibration data just before circuit execution; key empirical evidence for CADQE's runtime-adaptive design philosophy |
| 036 | [036_Evaluating_analytic_gradients_on_quantum_hardware.pdf](pdfs/downloaded/036_Evaluating_analytic_gradients_on_quantum_hardware.pdf) | Schuld et al. (2019). *Physical Review A*, 99, 032331. | Establishes the parameter-shift rule for computing exact gradients on quantum hardware; foundational for the VQC training framework within which CADQE operates |
| 086 | [086_Addressing_temporal_variations_in_qubit_quality_metrics_for_parameterized_quantu.pdf](pdfs/downloaded/086_Addressing_temporal_variations_in_qubit_quality_metrics_for_parameterized_quantu.pdf) | Alam, Ash-Saki & Ghosh (2019). *IEEE ISLPED*, pp. 1–6. | Quantifies temporal drift in qubit quality metrics (T₁, T₂, gate error) for VQCs; directly motivates CADQE's re-evaluation of d_max every 10 training epochs |
| 092 | [092_An_accurate_and_efficient_analytic_model_of_fidelity_under_depolarizing_noise_or.pdf](pdfs/downloaded/092_An_accurate_and_efficient_analytic_model_of_fidelity_under_depolarizing_noise_or.pdf) | Escofet et al. (2025). *Quantum Science and Technology*, 10, 035061. | Derives an accurate analytic fidelity model under depolarising noise; most directly related to CADQE's C2 Unified Fidelity Decay Law F(d) = (1−p₂Q)^d · exp(−d·t_g·n·(1/T₁+1/T₂)) |
| 152 | [152_A_hardware_aware_heuristic_for_the_qubit_mapping_problem_in_the_nisq_era.pdf](pdfs/downloaded/152_A_hardware_aware_heuristic_for_the_qubit_mapping_problem_in_the_nisq_era.pdf) | Niu et al. (2020). *IEEE Transactions on Quantum Engineering*, 1, 1–14. | Hardware-aware qubit mapping heuristic for NISQ processors; informs CADQE's C3 Kuhn–Munkres qubit assignment algorithm design |
| 176 | [176_A_methodology_to_select_and_adjust_quantum_noise_models_through_emulators_benchm.pdf](pdfs/downloaded/176_A_methodology_to_select_and_adjust_quantum_noise_models_through_emulators_benchm.pdf) | Bravo-Montes et al. (2024). *EPJ Quantum Technology*, 11, 71. | Methodology for selecting and calibrating quantum noise models via emulator benchmarking; validates CADQE's noise model estimation approach for M2 |

---

### Category 4 — Noise-Adaptive QML Frameworks (Prior Work)
*Papers representing the closest prior work to CADQE; analysed in Ch1 Section 1.5 "Why Existing Solutions Are Insufficient".*

| # | File | Reference | Key Contribution |
|---|---|---|---|
| 016 | [016_Quantumnas_Noise_adaptive_search_for_robust_quantum_circuits.pdf](pdfs/downloaded/016_Quantumnas_Noise_adaptive_search_for_robust_quantum_circuits.pdf) | Wang et al. (2022). *IEEE HPCA*, pp. 692–708. | **QuantumNAS** — most technically sophisticated noise-adaptive QML framework prior to CADQE. Performs evolutionary co-search of VQC architecture and qubit mapping. Critical limitation: encoding circuit is held fixed throughout. CADQE + QuantumNAS forms the optimal two-layer noise-adaptive pipeline |
| 076 | [076_Layerwise_learning_for_quantum_neural_networks.pdf](pdfs/downloaded/076_Layerwise_learning_for_quantum_neural_networks.pdf) | Skolik et al. (2021). *Quantum Machine Intelligence*, 3, 5. | Layerwise learning strategy for QNNs that progressively trains circuit layers; reduces barren plateau risk; one of the 5 VQC architectures in CADQE's experiment matrix |
| 094 | [094_Quantum_circuit_architecture_search_for_variational_quantum_algorithms.pdf](pdfs/downloaded/094_Quantum_circuit_architecture_search_for_variational_quantum_algorithms.pdf) | Du et al. (2022). *npj Quantum Information*, 8, 62. | Quantum circuit architecture search (QCAS); noise-aware NAS for VQAs; complementary to CADQE's encoding-layer focus |
| 052 | [052_Towards_quantum_enhanced_adversarial_robustness_in_machine_learning.pdf](pdfs/downloaded/052_Towards_quantum_enhanced_adversarial_robustness_in_machine_learning.pdf) | West et al. (2023). *Nature Machine Intelligence*, 5, 581–589. | Approximate amplitude encoding using MPS-based circuits achieving 25–50 CNOT gates with >95% state fidelity; enables CADQE to include amplitude encoding as a feasible candidate when d_max ≥ 25 |

---

### Category 5 — Barren Plateaus & Trainability
*Papers underpinning CADQE's Theorem T4.3 (Barren Plateau Onset Delay).*

| # | File | Reference | Key Contribution |
|---|---|---|---|
| 022 | [022_Barren_plateaus_in_quantum_neural_network_training_landscapes.pdf](pdfs/downloaded/022_Barren_plateaus_in_quantum_neural_network_training_landscapes.pdf) | McClean et al. (2018). *Nature Communications*, 9, 4812. | **Foundational barren plateau paper.** Proves gradient variance scales as O(2⁻ⁿ) for random VQCs; theoretical basis for CADQE's Theorem T4.3 |
| 138 | [138_Noise_induced_barren_plateaus_in_variational_quantum_algorithms.pdf](pdfs/downloaded/138_Noise_induced_barren_plateaus_in_variational_quantum_algorithms.pdf) | Wang et al. (2021). *Nature Communications*, 12, 6961. | Proves noise-induced barren plateaus are distinct from expressibility-induced ones; shows hardware noise compounds barren plateau onset — directly motivates CADQE's depth constraint as a trainability preservation mechanism |
| 144 | [144_Cost_function_dependent_barren_plateaus_in_shallow_parametrized_quantum_circuits.pdf](pdfs/downloaded/144_Cost_function_dependent_barren_plateaus_in_shallow_parametrized_quantum_circuits.pdf) | Cerezo et al. (2021). *Nature Communications*, 12, 1791. | Cost-function-dependent barren plateaus in shallow circuits; establishes that local cost functions avoid barren plateaus in shallow layers |
| 148 | [148_A_lie_algebraic_theory_of_barren_plateaus_for_deep_parameterized_quantum_circuit.pdf](pdfs/downloaded/148_A_lie_algebraic_theory_of_barren_plateaus_for_deep_parameterized_quantum_circuit.pdf) | Ragone et al. (2024). *Nature Communications*, 15, 7172. | Lie algebraic theory of barren plateaus; unifies all BP phenomena under dynamical Lie algebra (DLA) framework; foundation for CADQE's formal proof of Theorem T4.3 |
| 150 | [150_Investigating_and_mitigating_barren_plateaus_in_variational_quantum_circuits_a_s.pdf](pdfs/downloaded/150_Investigating_and_mitigating_barren_plateaus_in_variational_quantum_circuits_a_s.pdf) | Cunningham & Zhuang (2025). *Quantum Information Processing*, 24, 48. | Comprehensive survey of barren plateau investigation and mitigation strategies; contextualises CADQE's depth-constraint approach within the broader landscape of BP mitigation |

---

### Category 6 — Error Mitigation
*Papers on measurement-layer noise mitigation, representing the third layer of CADQE's three-layer QML noise management architecture.*

| # | File | Reference | Key Contribution |
|---|---|---|---|
| 068 | [068_Error_mitigation_for_short_depth_quantum_circuits.pdf](pdfs/downloaded/068_Error_mitigation_for_short_depth_quantum_circuits.pdf) | Temme, Bravyi & Gambetta (2017). *Physical Review Letters*, 119, 180509. | Introduces Zero-Noise Extrapolation (ZNE) — the primary error mitigation method for the measurement layer in CADQE's three-layer architecture |
| 136 | [136_Variational_quantum_machine_learning_with_quantum_error_detection.pdf](pdfs/downloaded/136_Variational_quantum_machine_learning_with_quantum_error_detection.pdf) | Adermann, Suzuki & Usman (2026). *Quantum Machine Intelligence*, 8, 1. | Integrates quantum error detection directly into VQC training; demonstrates compatibility with CADQE's encoding-layer adaptation |

---

### Category 7 — Research Methodology
*Papers supporting CADQE's Design Science Research (DSR) methodology, PRISMA systematic review, and statistical validation protocols.*

| # | File | Reference | Key Contribution |
|---|---|---|---|
| 168 | [168_Design_science_methodology_for_information_systems_and_software_engineering.pdf](pdfs/downloaded/168_Design_science_methodology_for_information_systems_and_software_engineering.pdf) | Wieringa (2014). *Springer-Verlag.* | **Primary DSR methodology reference.** CADQE's research paradigm (artefact construction + formal proof + empirical validation) follows the DSR framework defined here |
| 180 | [180_Evaluation_metrics_and_statistical_tests_for_machine_learning.pdf](pdfs/downloaded/180_Evaluation_metrics_and_statistical_tests_for_machine_learning.pdf) | Rainio, Teuho & Klén (2024). *Scientific Reports*, 14, 6086. | Evaluation metrics and statistical tests for ML experiments; justifies CADQE's use of Wilcoxon signed-rank tests, Bonferroni correction, and bootstrap confidence intervals |

---

### Category 8 — Healthcare, Industry & Application Domains
*Papers demonstrating QML application contexts and motivating real-world impact of the CADQE framework.*

| # | File | Reference | Key Contribution |
|---|---|---|---|
| 100 | [100_A_systematic_review_of_quantum_machine_learning_for_digital_health.pdf](pdfs/downloaded/100_A_systematic_review_of_quantum_machine_learning_for_digital_health.pdf) | Gupta et al. (2025). *npj Digital Medicine*, 8, 237. | Systematic review of QML in digital health; demonstrates clinical applications where encoding accuracy improvements (CADQE's contribution) translate directly to patient outcome improvements |
| 108 | [108_Variational_quantum_circuits_for_deep_reinforcement_learning.pdf](pdfs/downloaded/108_Variational_quantum_circuits_for_deep_reinforcement_learning.pdf) | Chen et al. (2020). *IEEE Access*, 8, 141007–141024. | VQCs applied to deep reinforcement learning; demonstrates that encoding choice affects convergence — extends CADQE's relevance beyond classification to RL |
| 112 | [112_Quantum_support_vector_machines_for_classification_and_regression_on_a_trapped_i.pdf](pdfs/downloaded/112_Quantum_support_vector_machines_for_classification_and_regression_on_a_trapped_i.pdf) | Suzuki et al. (2024). *Quantum Machine Intelligence*, 6, 31. | QSVMs on IonQ Aria trapped-ion hardware; provides experimental context for CADQE's E5 cross-platform generalisation experiment |
| 118 | [118_A_comparative_analysis_and_noise_robustness_evaluation_in_quantum_neural_network.pdf](pdfs/downloaded/118_A_comparative_analysis_and_noise_robustness_evaluation_in_quantum_neural_network.pdf) | Ahmed et al. (2025). *Scientific Reports*, 15, 33654. | Comparative analysis of noise robustness across QNN architectures; confirms encoding strategy as the dominant noise-sensitivity factor |
| 186 | [186_Investigating_the_application_of_quantum_machine_learning_in_breast_cancer_a_sys.pdf](pdfs/downloaded/186_Investigating_the_application_of_quantum_machine_learning_in_breast_cancer_a_sys.pdf) | Kaveh et al. (2025). *Archives of Breast Cancer*, 12(2), 130–142. | Systematic review of QML in breast cancer detection; one of the real-world application domains for CADQE's benchmark datasets (Breast Cancer Wisconsin) |
| 188 | [188_Quantum_computing_revolution_in_healthcare_a_systematic_review_of_applications_i.pdf](pdfs/downloaded/188_Quantum_computing_revolution_in_healthcare_a_systematic_review_of_applications_i.pdf) | Bukkarayasamudram et al. (2025). *Artificial Intelligence Review*, 58, 1–35. | Systematic review of quantum computing in healthcare; contextualises CADQE's accuracy improvements within clinical decision-support applications |
| 190 | [190_Applications_of_quantum_computing_in_clinical_care.pdf](pdfs/downloaded/190_Applications_of_quantum_computing_in_clinical_care.pdf) | Fairburn et al. (2025). *Frontiers in Medicine*, 12, 1573016. | Applications of quantum computing in clinical care settings; demonstrates deployment pathway for CADQE-enhanced QML classifiers |
| 192 | [192_Industry_quantum_computing_applications.pdf](pdfs/downloaded/192_Industry_quantum_computing_applications.pdf) | QUTAC et al. (2021). *EPJ Quantum Technology*, 8, 25. | Industry quantum computing applications across finance, logistics, chemistry; motivates CADQE's hardware-agnostic design for enterprise deployment |
| 202 | [202_Mapping_quantum_industry_demands_to_education_a_critical_analysis_of_skills_qual.pdf](pdfs/downloaded/202_Mapping_quantum_industry_demands_to_education_a_critical_analysis_of_skills_qual.pdf) | Devendrababu et al. (2025). *EPJ Quantum Technology*, 12, 105. | Maps quantum industry skills requirements to education; contextualises CADQE's practical IBM Quantum implementation within workforce development |
| 208 | [208_Advancing_quantum_technology_workforce_industry_insights_into_qualification_and_.pdf](pdfs/downloaded/208_Advancing_quantum_technology_workforce_industry_insights_into_qualification_and_.pdf) | Greinert et al. (2024). *EPJ Quantum Technology*, 11, 82. | Industry insights into quantum technology qualification needs |
| 210 | [210_Assessing_the_needs_of_the_quantum_industry.pdf](pdfs/downloaded/210_Assessing_the_needs_of_the_quantum_industry.pdf) | Hughes et al. (2022). *IEEE Transactions on Education*, 65(4), 592–601. | Assesses quantum industry workforce needs; benchmarks the competencies required to implement and deploy frameworks like CADQE |
| 216 | [216_IBM_quantum_computers_evolution_performance_and_future_directions_M.pdf](pdfs/downloaded/216_IBM_quantum_computers_evolution_performance_and_future_directions_M.pdf) | AbuGhanem (2025). *The Journal of Supercomputing*, 81(5), 687. | Comprehensive review of IBM Quantum processors (Falcon, Eagle, Heron, Condor) — evolution, performance metrics, and roadmap; primary hardware reference for CADQE's Table 1.1 |
| 220 | [220_Superconducting_quantum_computers_who_is_leading_the_future.pdf](pdfs/downloaded/220_Superconducting_quantum_computers_who_is_leading_the_future.pdf) | AbuGhanem (2025). *EPJ Quantum Technology*, 12, 102. | Landscape of superconducting quantum computers; contextualises IBM's position relative to Google Willow, Rigetti Ankaa, and IQM — all CADQE validation platforms |
| 226 | [226_TensorHyper_VQC_a_tensor_train_guided_hypernetwork_for_robust_and_scalable_varia.pdf](pdfs/downloaded/226_TensorHyper_VQC_a_tensor_train_guided_hypernetwork_for_robust_and_scalable_varia.pdf) | Qi et al. (2026). *npj Quantum Information*, 12, 70. | TensorHyper-VQC: tensor-train hypernetwork for robust VQC scaling; represents an alternative approach to CADQE's noise-adaptive pipeline using tensor methods |
| 230 | [230_Exploring_the_application_of_quantum_technologies_to_industrial_and_real_world_u.pdf](pdfs/downloaded/230_Exploring_the_application_of_quantum_technologies_to_industrial_and_real_world_u.pdf) | Osaba et al. (2025). *The Journal of Supercomputing*, 81(7), 829. | Explores quantum technology applications in industrial/real-world use cases; provides the applied motivation for CADQE's accuracy recovery on real hardware |

---

## BibTeX Library

[`library.bib`](library.bib) contains seed BibTeX entries for the core CADQE references. It is structured to expand to all 116 papers in the full reference list.

To import into **Zotero**: File → Import → BibTeX  
To import into **Mendeley**: File → Import Library → BibTeX  
To import into **LaTeX**: `\bibliography{library}` with `\bibliographystyle{IEEEtranN}`

---

## Paper Statistics

| Category | Papers in Archive | Papers in Full Reference List |
|---|---|---|
| Foundational QML & NISQ Theory | 5 | 8 |
| Data Encoding Strategies | 9 | 22 |
| Noise, Fidelity & Hardware | 6 | 18 |
| Noise-Adaptive QML Frameworks | 4 | 9 |
| Barren Plateaus & Trainability | 5 | 8 |
| Error Mitigation | 2 | 5 |
| Research Methodology | 2 | 7 |
| Healthcare, Industry & Applications | 15 | 19 |
| **Total** | **48** | **116** |

---

## Related Repositories

| Repository | Relationship |
|---|---|
| [`phd-literature-review`](https://github.com/sajidalikhanphd/phd-literature-review) | Per-paper summaries, PRISMA screening log, annotated bibliography |
| [`phd-introduction`](https://github.com/sajidalikhanphd/phd-introduction) | Chapter 1 cites papers in this archive (encoding dominance, NISQ characterisation) |
| [`phd-research-methodology`](https://github.com/sajidalikhanphd/phd-research-methodology) | Chapter 3 cites methodology papers (DSR, statistical tests) |
| [`phd-drafts-and-versions`](https://github.com/sajidalikhanphd/phd-drafts-and-versions) | `full-thesis/bibliography/references.bib` is built from `library.bib` here |
| [`cadqe`](https://github.com/sajidalikhanphd/cadqe) | The open-source implementation of C1/C2/C3 described by the papers in this repo |

---

## Citation

If you use this reference archive or the CADQE framework in your work:

```bibtex
@software{cadqe2026,
  title   = {{CADQE}: Calibration-Adaptive Data-to-Quantum Encoding},
  author  = {Khan, Sajid Ali},
  year    = {2026},
  url     = {https://github.com/sajidalikhanphd/cadqe},
  note    = {PhD Research Programme, 2026--2030}
}
```

---

*Maintained by Sajid Ali Khan · PhD Candidate · [@sajidalikhanphd](https://github.com/sajidalikhanphd)*
*Research AI Assistant: JARVIS (IBM Bob)*
