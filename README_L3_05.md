
# L3-05: Quantum Phase Estimation Implementation

## NEHAL MAHENDRA RANE

### Problem Statement:
Implement Quantum Phase Estimation (QPE) to approximate eigenvalues.

### Steps:
1. **Install Libraries**:
    - Install `qiskit`, `numpy`, and `matplotlib`.
    ```bash
    !pip install qiskit
    !pip install numpy
    !pip install matplotlib
    ```

2. **Imports**:
    ```python
    from qiskit import QuantumCircuit
    from qiskit import transpile
    ```

3. **Controlled Unitary Function**:
    A function that creates a controlled unitary operation.
    ```python
    def controlled_unitary(circuit, theta, control_qubit, target_qubit):
        # Function body here
    ```

4. **Quantum Phase Estimation Function**:
    A function that implements the QPE algorithm.
    ```python
    def quantum_phase_estimation(theta, num_qubits):
        circuit = QuantumCircuit(num_qubits + 1, num_qubits)
    ```

5. **Parameters**:
    Parameters such as angle (`theta`) and the number of qubits.
    ```python
    theta = np.pi / 4
    num_qubits = 3
    ```

6. **Simulation**:
    The circuit is transpiled and run on a Qiskit Aer simulator.
    ```python
    simulator = Aer.get_backend('qasm_simulator')
    result = simulator.run(transpiled_circuit).result()
    counts = result.get_counts(circuit)
    print(counts)
    ```

7. **Visualization**:
    Plotting the results using a histogram.
    ```python
    plot_histogram(counts)
    ```
