# Trotter_Method_Superconducting_Qubits

# Trotterized Simulation of Superconducting Qubits

This repository contains Jupyter notebooks demonstrating **Trotterized time evolution** of 2-qubit and 3-qubit superconducting systems using Qiskit. It explores:

- Second-order Trotter decomposition
- Expectation values of observables (e.g., ⟨Z₀⟩)
- Entanglement entropy as a function of time
- Fidelity comparison with exact unitary evolution

---

## Contents

| Notebook | Description |
|----------|-------------|
| `Trotter_2_Qubit_Simulation.ipynb` | Simulates dynamics and entropy in a 2-qubit system using Trotter evolution |
| `Trotter_3_Qubit_Simulation.ipynb` | Extends simulation to a 3-qubit system and explores richer entanglement structures |

---

## Physics Background

The simulations are based on the Hamiltonian:
$$\\[
H = J \sum Z_i Z_{i+1} + h \sum X_i
\\]$$
where:
- \\( J \\) is the ZZ interaction (qubit-qubit coupling)
- \\( h \\) is the transverse field (coherent drive)

Each Trotter step approximates:
\\[
U(\delta t) \approx e^{-i H_X \delta t / 2} \cdot e^{-i H_Z \delta t} \cdot e^{-i H_X \delta t / 2}
\\]

