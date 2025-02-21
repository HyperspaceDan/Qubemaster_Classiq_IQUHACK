# Qubmaster_Classiq_IQUHACK
This repository contains the solution (an attempt) for the Classiq challenge at the MIT iQuHack 2025. This challenge focuses on Gaussian State preparation using the Classiq SDK.

# Our Approach

Our approach to the Classiq Challenge at the MIT iQuHack Hackathon 2025 involves preparing a Gaussian state over a specified domain using the Classiq SDK. The solution is implemented in the Jupyter notebook [`classiq_iQuHack_2025_final.ipynb`](QubMaster.ipynb). Here is a detailed description of our approach and the code we developed:

## Gaussian State Preparation

1. **Gaussian Distribution Generation**:
   - We defined a function to generate a Gaussian distribution over the interval \([-2, 2)\) with a specified resolution.
   - The Gaussian distribution is normalized to ensure the sum of probabilities equals one.

2. **Quantum State Preparation**:
   - We implemented a function to prepare a quantum state that encodes the normalized Gaussian distribution using recursive amplitude encoding with controlled rotations.
   - The `prepare_gaussian` function applies a Hadamard transform followed by controlled rotations to encode the Gaussian amplitudes into the quantum state.
