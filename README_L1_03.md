
# README - Quantum Ripple Carry Adder (L1_03.ipynb)

## Overview
This notebook demonstrates the implementation of a **Quantum Ripple Carry Adder** using Qiskit, a Python library for quantum computing. The Ripple Carry Adder is a classical adder circuit that has been adapted to run on a quantum computer, leveraging quantum gates to perform binary addition.

### Features:
- Adds two binary numbers using quantum circuits.
- Implements a ripple carry logic using controlled quantum gates.
- Provides a sample example to add two 3-bit binary numbers.

## Dependencies
The following libraries are required to run the notebook:
- **qiskit**: For creating quantum circuits and simulating them.
- **numpy**: For handling binary arrays and numerical operations.
- **matplotlib**: For plotting visualizations (if any).
  
Install the dependencies using:
```
!pip install qiskit numpy matplotlib
```

## Usage
1. **Quantum Ripple Carry Adder Function**:
   The function `quantum_ripple_carry_adder(a, b)` takes two binary numbers as input and performs quantum-based addition.

2. **Example**:
   Example input:
   ```python
   a = [1, 0, 1]  # Binary for 5
   b = [1, 1, 0]  # Binary for 6
   qc = quantum_ripple_carry_adder(a, b)
   ```

3. **Simulation**:
   You can simulate the quantum circuit using Qiskit simulators.

## How to Run
To run the notebook:
1. Install the dependencies listed above.
2. Open the notebook and run the cells to generate a quantum circuit and simulate the adder.

