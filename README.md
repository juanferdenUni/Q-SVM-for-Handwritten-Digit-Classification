# Q-SVM-for-Handwritten-Digit-Classification
Implemented and benchmarked Quantum SVMs for digit classification using Qiskit, comparing their performance to classical SVMs on the MNIST dataset. Developed as part of the *Architecture and Programming of Quantum Computers* course at Complutense University of Madrid, the work benchmarks QSVMs (simulated via Qiskit) against classical SVMs using PCA-reduced data.

## Overview

- **Dataset**: Subset of MNIST (digits 6, 9, 1, 7, 2, 3, 4)
- **Feature Extraction**: PCA to reduce dimensionality to 4 features
- **Classical Models**: SVMs with linear and RBF kernels
- **Quantum Models**: QSVMs with multiple quantum feature maps simulated via Qiskit AerSimulator
- **Tasks**:
  - Binary classification: 6 vs 9, 1 vs 7
  - Multi-class classification: 1 vs 2 vs 3 vs 4

## Results Summary

| Task             | Classical SVM | QSVM (Best Map) |
|------------------|---------------|-----------------|
| 6 vs 9           | 95%           | 90%             |
| 1 vs 7           | 95%           | **100%**        |
| 1 vs 2 vs 3 vs 4 | 90%           | 70%             |

## Key Insights

- QSVMs can match or outperform classical SVMs in small binary tasks with well-chosen feature maps.
- Classical SVMs remain more reliable for multi-class tasks and generalization.
- Kernel design and data dimensionality are critical in quantum ML.

## Technologies

- [Qiskit](https://qiskit.org/)
- Python 3.9+
- NumPy, scikit-learn, matplotlib
- Jupyter Notebook

## References

- Havlíček, V., Córcoles, A. D., Temme, K., Harrow, A. W., Kandala, A., Chow, J. M., & Gambetta, J. M. (2019). *Supervised learning with quantum-enhanced feature spaces*. Nature, 567(7747), 209–212.  
- Bindhani, M., Behera, B. K., & Panigrahi, P. K. (2020). *Handwritten Digit Recognition Using Quantum Support Vector Machine*. Preprint. DOI:10.13140/RG.2.2.36253.74727.  
- Li, K., Zhao, P., Dai, S., et al. (2024). *Exploring the Impact of Quantum Computing on Machine Learning Performance*. Middle East Journal of Applied Science & Technology, January 2024.  
- Rana, A., Vaidya, P., & Gupta, G. (2021). *A comparative study of quantum support vector machine algorithm for handwritten recognition with support vector machine algorithm*. Materials Today: Proceedings, 56(1).  
- Kariya, A., & Behera, B. K. (2021). *Investigation of Quantum Support Vector Machine for Classification in NISQ era*. arXiv preprint arXiv:2112.06912.

## Contact
email: juafer15@ucm.es


