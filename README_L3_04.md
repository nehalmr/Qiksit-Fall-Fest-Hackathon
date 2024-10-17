
# L3-04: Bernstein-Vazirani Algorithm Implementation

## NEHAL MAHENDRA RANE

### Problem Statement:
Implement the Bernstein-Vazirani algorithm for finding hidden binary strings.

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

3. **Bernstein-Vazirani Function**:
    A function that constructs the Bernstein-Vazirani quantum circuit.
    ```python
    def bernstein_vazirani(hidden_string):
        n = len(hidden_string)
        circuit = QuantumCircuit(n + 1, n)
    ```

4. **Example Hidden String**:
    An example of a hidden binary string `'101'`.
    ```python
    hidden_string = '101'
    circuit = bernstein_vazirani(hidden_string)
    transpiled_circuit = transpile(circuit)
    ```

5. **Visualization**:
    You can print the quantum circuit to visualize it.
    ```python
    print(transpiled_circuit.draw())
    ```
