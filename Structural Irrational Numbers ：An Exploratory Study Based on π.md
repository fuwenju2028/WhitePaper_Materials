# Structural Irrational Numbers: An Exploratory Study Based on π

## ——A Technical Report on Phenomena, Methods, and Open Questions

**Author**: Wenju Fu  
**Version**: 3.1 (Academic Technical Edition)  
**Date**: April 2026  
**Permanent Identifiers**:
- Dataset DOI: 10.57760/sciencedb.34550
- Code Repository: https://github.com/fuwenju2028/Structural-Irrational-Numbers
- White Paper Materials: https://github.com/fuwenju2028/WhitePaper_Materials

---

## Abstract

The decimal expansion of π (non-repeating and infinite) is often used as a reference for random sequences. This study conducts a multi-dimensional statistical analysis of π's decimal expansion based on 100 million digits, including long-range dependence (Hurst exponent), spectral characteristics, pattern coverage speed, digit transition probabilities, and multi-scale fluctuation scaling.

The main observational results are as follows:

1. **Processuality**: The Hurst exponent of π is H ≈ 0.5049, statistically significantly deviating from the theoretical value of 0.5 for independent and identically distributed sequences (p < 10⁻²⁶), though the magnitude of deviation is minimal (approximately 1%).

2. **Spectral Characteristics**: The power spectrum of π exhibits a large number of significant peaks (58,746), far exceeding the count for a random control sequence of the same length (approximately 102).

3. **Multi-scale Scaling**: The multi-scale fluctuation scaling exponent of π is H_h ≈ -0.009, significantly deviating from -0.5 for white noise.

4. **Classical Randomness**: π passes all classical randomness tests, including the chi-square uniformity test (p=0.609) and the runs test (p=1.000).

Based on these observations, this paper proposes **"Structural Irrational Numbers"** as a conceptual hypothesis for discussion, describing a class of mathematical constants that, while satisfying classical randomness tests, exhibit systematic, detectable, unconventional features in their higher-order statistics. This paper further proposes the refined nomenclature **"Endogenously Structural Expanding Transcendentals"**, positioning π as the prototype of this class of mathematical objects.

All data and code are publicly released, inviting the academic community to examine the robustness of these observations and explore their possible mathematical explanations and application potentials.

**Keywords**: Pi; Digit Sequence Analysis; Long-range Dependence; Spectral Analysis; Multi-scale Analysis; Structural Irrational Numbers; Endogenous Structure; RDN Cryptography

---

## Table of Contents

1. [Introduction: Problem Statement and Research Positioning](#1-introduction-problem-statement-and-research-positioning)
2. [Data and Methods](#2-data-and-methods)
3. [Main Observational Results](#3-main-observational-results)
4. [Discussion and Limitations](#4-discussion-and-limitations)
5. [A Hypothesis for Discussion: Structural Irrational Numbers](#5-a-hypothesis-for-discussion-structural-irrational-numbers)
6. [Nomenclature and Positioning: π as an "Endogenously Structural Expanding Transcendental"](#6-nomenclature-and-positioning-π-as-an-endogenously-structural-expanding-transcendental)
7. [Open Questions and Future Directions](#7-open-questions-and-future-directions)
8. [Data and Code Availability](#8-data-and-code-availability)
9. [References](#9-references)
10. [Appendices](#10-appendices)

---

## 1. Introduction: Problem Statement and Research Positioning

### 1.1 Background

Pi (π) is one of the most thoroughly studied mathematical constants in human history. Its decimal expansion has been computed to tens of trillions of digits without any discovery of periodic structure. Within classical number theory, π is classified as a transcendental number, and its digit sequence is often used as a reference for randomness studies or conjectured to be a "normal number" (i.e., all digits appear with equal probability, and all finite patterns appear with asymptotically equal frequency).

However, "non-repeating and infinite" and the "normal number conjecture" only describe the macroscopic statistical properties of the sequence and make no assertions about its internal structure. A natural question arises: While satisfying these macroscopic statistical properties, might π's sequence contain detectable, non-trivial structural features?

### 1.2 Positioning of This Study

This is an **exploratory study**. We do not claim to have "discovered the deep structure of π," nor do we assert the establishment of a "new paradigm." Our goal is to **systematically report several phenomena observed in the multi-dimensional statistical analysis of π's sequence, and to open all data and methods for the academic community to examine the robustness, statistical specificity, and potential theoretical explanations of these observations.**

### 1.3 Structure of This White Paper

- **Chapter 2**: Data and Methods
- **Chapter 3**: Empirical Observations of the Six Properties
- **Chapter 4**: Discussion and Limitations
- **Chapter 5**: The Structural Irrational Number Hypothesis
- **Chapter 6**: Nomenclature and Positioning (Core Addition)
- **Chapter 7**: Open Questions and Future Directions
- **Chapters 8-10**: Data, Code, and Appendices

---

## 2. Data and Methods

### 2.1 Data

This study uses **100,000,000 digits** of π's decimal expansion (including the integer digit "3"). Data accuracy has been ensured through multi-source cross-validation. For ease of processing, the data is split into 10 files, each containing approximately 10 million digits, consisting solely of digit characters "0"-"9" without delimiters.

The data is publicly archived at ScienceDB, DOI: 10.57760/sciencedb.34550.

### 2.2 Analytical Methods

| Analytical Dimension     | Method                                      | Key Indicator                            | Reference Baseline               |
| ------------------------ | ------------------------------------------- | ---------------------------------------- | -------------------------------- |
| Uniformity               | Chi-square goodness-of-fit test             | p-value                                  | Theoretical uniform distribution |
| Runs Test                | Wald-Wolfowitz runs test                    | p-value                                  | I.I.D. sequence                  |
| Autocorrelation          | Autocorrelation function (ACF)              | 95% confidence interval                  | White noise                      |
| Long-range Dependence    | Rescaled Range Analysis (R/S), DFA          | Hurst exponent H                         | H=0.5 (no memory)                |
| Spectral Characteristics | Fast Fourier Transform (FFT)                | Power spectrum, significant peak count   | Random sequence spectrum         |
| Pattern Coverage         | Sliding window enumeration                  | Coverage rate, first occurrence position | Random expectation               |
| Transition Probability   | First-order Markov transition matrix        | Symmetry error, parity transition ratio  | Random expectation               |
| Multi-scale Fluctuation  | Coarse-graining standard deviation analysis | Scaling exponent H_h                     | H_h=-0.5 (white noise)           |
| Period Detection         | FFT peak detection + clustering             | List of significant periods              | —                                |

### 2.3 Note on Statistical Significance

This study involves numerous statistical tests. For large sample sizes (on the order of 10⁸), special attention must be paid to:

- Statistical significance is not equivalent to practical importance
- The multiple testing problem
- The necessity of control comparisons

This study reports effect sizes where possible and compares key findings with random controls.

---

## 3. Main Observational Results

### 3.1 Classical Randomness Tests: The "Random Veil" of π

| Test                             | Statistic | p-value | Conclusion at α=0.05         |
| -------------------------------- | --------- | ------- | ---------------------------- |
| Chi-square uniformity test       | χ²=7.268  | 0.609   | Cannot reject uniformity     |
| Runs test                        | —         | 1.000   | Meets randomness expectation |
| Autocorrelation test (lag 1-100) | —         | —       | Mostly within 95% CI         |

**Observation**: π's sequence passes these classical randomness tests. This serves to validate the data quality of this study and confirm the background for subsequent analyses.

### 3.2 Processuality: Hurst Exponent Analysis

**Method**: The 100-million-digit sequence was divided into 100 non-overlapping one-million-digit subsequences, and the Hurst exponent (R/S analysis) was calculated for each.

**Results**:
- Mean Hurst exponent H = 0.504946
- Standard deviation = 0.003379
- One-sample t-test (null hypothesis H₀: μ=0.5): t(99)=16.51, p < 10⁻²⁶

**Comparison with Random Control**: 100 pseudo-random sequences of the same length (one million digits) were generated, yielding a mean Hurst exponent of 0.500012 and standard deviation of 0.003412.

**Observation**: The Hurst exponent of π is statistically significantly different from 0.5, indicating the presence of weak long-range memory in the sequence. The deviation is minimal in magnitude (about 1%) but extremely high in statistical significance.

### 3.3 Spectral Characteristics: Detection of Periodic Components

**Method**: FFT was applied to the π sequence to compute the power spectral density. Significant peaks were identified as those exceeding three standard deviations above the local background noise.

**Results**:
- Number of significant peaks detected: **58,746**
- Number for random sequences of the same length (average of 100 runs): approximately 102
- Spectral flatness γ of π: 0.372; for random sequences: approximately 0.998

**Observation**: The power spectrum of π exhibits a **qualitative difference** from that of random sequences—it contains a large number of statistically significant periodic components.

**Important Note**: The detected "periods" are not strict mathematical periods but rather statistical "quasi-periodic components" or "dominant frequencies." Further validation with surrogate data methods is required.

### 3.4 Inclusiveness: Pattern Coverage Speed

**Method**: The occurrence of digit patterns of varying lengths L within the first N digits of π was statistically analyzed.

**Results**:
- 2-digit patterns (00-99): 100% coverage, last occurrence at position 605
- 3-digit patterns (000-999): 100% coverage
- 4-digit patterns (0000-9999): 100% coverage

**Observation**: π exhibits efficient pattern traversal capability, covering all short patterns faster than random expectation.

### 3.5 Alternation: Transition Matrix Analysis

**Method**: A first-order Markov transition probability matrix T was constructed, where T[i][j] = P(d_{n+1}=j | d_n=i).

**Results**:
- Transition symmetry error: **0.001071**
- Odd-even transition ratio P(odd→even): **0.499906**, deviation from 0.5: 0.000094

**Observation**: The transition matrix of π is nearly perfectly symmetric, and the odd-even transition ratio shows almost no deviation from the theoretical value.

### 3.6 Hierarchy: Multi-scale Fluctuation Analysis

**Method**: The sequence was coarse-grained at different scales L (10⁰ to 10⁶ digits), and the standard deviation σ(L) of the coarse-grained subsequences was calculated. The slope of log(σ) versus log(L) was fitted, denoted as the scaling exponent H_h.

**Results**:
- Fitted scaling exponent H_h ≈ -0.009
- Theoretical value for white noise: H_h = -0.5

**Observation**: The fluctuation standard deviation of π is **almost invariant** with scale (exponent near 0), in stark contrast to the rapid decay of white noise (exponent -0.5). This is one of the most noteworthy phenomena in this study.

### 3.7 Nesting: Preliminary Observation of Periodic Relationships

**Method**: From the significant periods detected via spectral analysis, those with the highest signal-to-noise ratios were selected to examine mathematical relationships among them.

**Results**: Approximate integer multiple or simple rational ratio relationships were found among some periods:

| Period p₁    | Period p₂    | Ratio p₂/p₁ | Approximate Relationship |
| ------------ | ------------ | ----------- | ------------------------ |
| 49.0 digits  | 153.8 digits | 3.138       | ≈ π                      |
| 244.0 digits | 487.8 digits | 2.000       | Exact 2×                 |
| 153.8 digits | 487.8 digits | 3.172       | ≈ π                      |

**Important Caveat**: This analysis is exploratory and post-hoc, carrying a risk of "selective reporting." Nesting currently remains a **preliminary observation requiring further validation**.

---

## 4. Discussion and Limitations

### 4.1 Summary of Main Observations

| Property                 | Observation                                   | Degree of Confirmation | Specificity                                |
| ------------------------ | --------------------------------------------- | ---------------------- | ------------------------------------------ |
| Classical Randomness     | Passes χ², runs, autocorrelation tests        | High                   | None (as expected)                         |
| Processuality            | H=0.5049, significant deviation from 0.5      | High                   | Weak, effect size to be evaluated          |
| Spectral Characteristics | 58,746 significant peaks                      | High                   | Strong, requires surrogate data validation |
| Inclusiveness            | Pattern coverage faster than random           | Medium                 | To be validated                            |
| Alternation              | Transition matrix highly symmetric            | High                   | Weak (may be a common property)            |
| Hierarchy                | H_h≈-0.009, significant deviation from -0.5   | High                   | Strong, requires theoretical explanation   |
| Nesting                  | Proportional relationships among some periods | Low                    | To be validated                            |

### 4.2 Key Limitations

1. **Lack of surrogate data testing**: This is the most serious omission.
2. **Multiple testing problem**: Some "significant" results may arise from random fluctuations.
3. **Risk of post-hoc interpretation**: Selection bias exists.
4. **Effect size issue**: Although statistically significant, the deviation of the Hurst exponent is minimal in magnitude.
5. **Lack of theoretical explanation**: Findings currently remain at the level of "phenomenon reporting."

---

## 5. A Hypothesis for Discussion: Structural Irrational Numbers

Based on the above observations—particularly the richness of spectral features, the unique scaling of multi-scale fluctuations, and the weak but significant long-range dependence—we propose a conceptual hypothesis for academic discussion:

> **Structural Irrational Number Hypothesis**: There exists a class of irrational numbers (of which π may be the prototype) whose decimal expansions, while satisfying classical randomness tests (i.e., the "random veil"), exhibit detectable, non-random, systematic patterns in their higher-order statistics (e.g., spectral structure, multi-scale scaling laws, pattern coverage dynamics).

### 5.1 Testable Implications of the Hypothesis

1. **Existence**: At least one irrational number (e.g., π) exists for which the above higher-order statistical features significantly deviate from random expectations under rigorous testing.
2. **Stability**: These features are stable across different data segments.
3. **Specificity**: Not all irrational numbers possess such features at equal strength.
4. **Explainability**: These features are traceably connected to the mathematical definition of the number.

### 5.2 Current Evidence Strength for the Hypothesis

| Evidence Level                    | Meaning                                                      | Status for This Hypothesis |
| --------------------------------- | ------------------------------------------------------------ | -------------------------- |
| Level 1: Observational Clues      | Preliminary phenomena worthy of attention                    | ✅ Meets                    |
| Level 2: Testable Conjecture      | Clear testing methods exist                                  | ✅ Can be proposed          |
| Level 3: Preliminary Validation   | Passes some independent tests                                | ❌ Not yet achieved         |
| Level 4: Robustly Established     | Consistent multi-source evidence, reproducible               | ❌ Far from achieved        |
| Level 5: Theoretically Integrated | Compatible with existing mathematical theory with explanation | ❌ Not yet achieved         |

**Conclusion**: This hypothesis is currently at the stage **transitioning from "Level 1: Observational Clues" to "Level 2: Testable Conjecture."**

---

## 6. Nomenclature and Positioning: π as an "Endogenously Structural Expanding Transcendental"

Based on the empirical findings of the six properties and the formalization framework presented above, we propose a refined nomenclature to characterize the class of mathematical objects represented by π:

### Endogenously · Structural · Expanding · Transcendental

| Dimension                 | Term               | Meaning                                                      |
| ------------------------- | ------------------ | ------------------------------------------------------------ |
| **Origin**                | **Endogenous**     | The structure originates from the mathematical definition of π itself (e.g., infinite series, continued fractions, geometric meaning), rather than being artificially extracted by statistical methods or externally imposed |
| **Form**                  | **Structural**     | Organized, hierarchical, and internally interconnected. The six properties are projections of this structure onto different dimensions |
| **Mode of Manifestation** | **Expanding**      | The structure reveals itself layer by layer upon decimal expansion. The length of expansion correlates with the depth of observable structure—the more you look, the deeper you see |
| **Mathematical Category** | **Transcendental** | An established mathematical category. π is the prototype of a special subclass within transcendentals possessing unique structural properties |

### 6.1 The Power of This Nomenclature

1. **Unification**: Gathers the scattered observations of the six properties into a concept with a core essence.
2. **Differentiability**: Contrasts with "ordinary transcendentals" (if they exist), providing linguistic tools for taxonomic research.
3. **Operationalizability**: Each dimension has potential quantitative indicators (endogeneity strength, structural complexity, expansion depth, transcendence measure).
4. **Heuristic Value**: Points to a series of testable sub-questions.

### 6.2 Relationship with Other Concepts

- **Relationship with Normal Numbers**: Endogenously structural expanding transcendentals necessarily satisfy (or approximate) normal number properties, but normal numbers are not necessarily structural.
- **Relationship with Transcendentals**: π is a transcendental, but whether structural properties are necessarily related to transcendence remains unknown.
- **Relationship with the RDN Cryptographic System**: As an endogenously structural expanding transcendental, π's multi-scale nesting properties provide an ideal entropy source and structural template for the RDN cryptographic system.

---

## 7. Open Questions and Future Directions

### 7.1 Questions Requiring Immediate Answers

1. **Surrogate Data Testing**: Can the spectral peaks, pattern coverage speed, and multi-scale scaling of π pass phase-randomized surrogate data tests?
2. **Cross-constant Comparison**: Do other major mathematical constants such as e, √2, φ, ln2 exhibit similar features?
3. **Data Segment Stability**: Are the above features stable across different independent segments of the 100-million-digit dataset?
4. **Effect Size Evaluation**: What is the practical effect size of the minimal Hurst exponent deviation and the anomalous multi-scale exponent?

### 7.2 Medium-term Directions

1. **Theoretical Modeling**: Can the observed statistical features be derived from the mathematical definition of π?
2. **Generative Model Attempts**: Can a simple deterministic algorithm be constructed that generates sequences with similar multi-scale statistical features?
3. **RDN Completion**: Fix encryption/decryption bugs and complete NIST testing.

### 7.3 Long-term Vision

1. **Extension of Real Number Taxonomy**: Adding a "structural" dimension to the rational/irrational dichotomy.
2. **Interdisciplinary Applications**: Cryptography, complex system modeling, AI initialization.
3. **Philosophical Implications for Mathematics**: Insights into the ontology of mathematical discovery.

---

## 8. Data and Code Availability

This study adheres to open science principles. All data and code are publicly available:

| Resource Category     | Name                                    | Access Link      | Identifier                    |
| --------------------- | --------------------------------------- | ---------------- | ----------------------------- |
| Core Dataset          | Pi_Six_Properties_Evidence_Complete.tar | ScienceDB        | DOI: 10.57760/sciencedb.34550 |
| Main Code Repository  | Structural-Irrational-Numbers           | GitHub           | MIT License                   |
| White Paper Materials | WhitePaper_Materials                    | GitHub           | —                             |
| Author Identifier     | Wenju Fu                                | ORCID            | 0009-0008-7904-1580           |
| Contact Email         | —                                       | fuwenju@yeah.net | Subject: SIN-Collaboration    |

---

## 9. References

### A.1 Mathematical Constants and Computational Mathematics

1. Bailey, D. H., Borwein, P. B., & Plouffe, S. (1997). On the Rapid Computation of Various Polylogarithmic Constants. *Mathematics of Computation*, 66(218), 903-913.

2. Borwein, J. M., & Borwein, P. B. (1987). *Pi and the AGM: A Study in Analytic Number Theory and Computational Complexity*. Wiley-Interscience.

3. Finch, S. R. (2003). *Mathematical Constants*. Cambridge University Press.

### A.2 Randomness Analysis

4. Marsaglia, G. (1995). The Marsaglia Random Number CDROM, with The Diehard Battery of Tests.

5. Bugeaud, Y. (2012). *Distribution Modulo One and Diophantine Approximation*. Cambridge University Press.

### A.3 Time Series Analysis and Fractal Theory

6. Mandelbrot, B. B. (1982). *The Fractal Geometry of Nature*. W.H. Freeman.

7. Hurst, H. E. (1951). Long-term storage capacity of reservoirs. *Transactions of the American Society of Civil Engineers*, 116, 770-799.

8. Kantelhardt, J. W., et al. (2002). Multifractal detrended fluctuation analysis of nonstationary time series. *Physica A*, 316(1-4), 87-114.

### A.4 Information Theory and Complexity Science

9. Li, M., & Vitányi, P. (2008). *An Introduction to Kolmogorov Complexity and Its Applications*. Springer.

10. Cover, T. M., & Thomas, J. A. (2006). *Elements of Information Theory*. Wiley-Interscience.

### A.5 Related Preprints and Datasets

11. Fu, W. (2025). Pi as a Structural Irrational Number: Complete Evidence Package for Six Mathematical Properties. ScienceDB. DOI: 10.57760/sciencedb.34550

12. Bailey, D. H., & Crandall, R. E. (2001). On the Random Character of Fundamental Constant Expansions. *Experimental Mathematics*, 10(2), 175-190.

---

## 10. Appendices

### Appendix A: Glossary of Key Terms

| Term                                   | Definition                                                   |
| -------------------------------------- | ------------------------------------------------------------ |
| **Structural Irrational Number (SIN)** | A class of irrational numbers whose decimal expansions, while passing conventional randomness tests, exhibit measurable, non-random, multi-scale deterministic patterns |
| **Endogenous**                         | Structure originates from the mathematical definition itself, rather than being externally imposed or artificially extracted by statistical methods |
| **Expanding**                          | Structure reveals itself layer by layer upon decimal expansion; the length of expansion correlates with the depth of observable structure |
| **Processuality**                      | The property by which the current state of a sequence is influenced by its historical states; commonly measured by the Hurst exponent |
| **Inclusiveness**                      | The completeness with which a sequence contains all possible finite-length digit patterns within a finite prefix |
| **Alternation**                        | The dynamic balance of transitions between adjacent digits   |
| **Hierarchy**                          | The scaling law exhibited by statistical properties as the observation scale changes |
| **Nesting**                            | Integer multiple or containment relationships among periodic patterns at different time scales |
| **Proportional Random Evolution**      | A conjecture concerning the proportional relationship between structural unit scale (L) and its first significant occurrence position (N) |
| **RDN**                                | Random Dynamic Nesting, a cryptographic framework based on structural sequences |

### Appendix B: Core Algorithm Pseudocode

**B.1 Rescaled Range Analysis for Hurst Exponent**

function calculate_hurst(sequence S, max_lag L):
initialize result list H_list = []
for n in [minimum segment length, L]:
partition S into k non-overlapping subsequences of length n
initialize R_over_S_list = []
for each subsequence sub_S:
Y = cumsum(sub_S - mean(sub_S))
R = max(Y) - min(Y)
S_n = std(sub_S)
if S_n > 0:
R_over_S_list.append(R / S_n)
if R_over_S_list is not empty:
H_list.append(log(mean(R_over_S_list)) / log(n))
perform linear regression of log(mean(R_over_S)) on log(n); slope is H
return H

**B.2 Multi-scale Fluctuation Analysis**

function multiscale_fluctuation(sequence S, scales list):
results = []
for L in scales:
coarse_grained = [mean(S[i:i+L]) for i in range(0, len(S), L) if i+L <= len(S)]
sigma = std(coarse_grained)
results.append((L, sigma))
perform linear regression of log(sigma) on log(L); slope is scaling exponent H_h
return results, H_h

---

**End of Technical Report**

---

## Version Revision History

| Version | Date           | Major Revisions                                              |
| ------- | -------------- | ------------------------------------------------------------ |
| 1.0     | January 2026   | Initial white paper                                          |
| 2.0     | February 2026  | Condensed manifesto edition                                  |
| 3.0     | March 2026     | Academic revision, repositioned as exploratory study         |
| **3.1** | **April 2026** | **Added Chapter 6 "Nomenclature and Positioning," unified "Endogenously Structural Expanding Transcendental" concept; expanded RDN-related content** |



