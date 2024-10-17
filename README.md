# Qiksit-Fall-Fest-Hackathon
## Overview
This project combines the implementation of various quantum algorithms and circuits to solve key computational problems. From detecting hidden binary strings to generating true randomness using quantum mechanics, the project journey spans multiple stages, each focusing on a unique quantum concept.

### Key Objectives:
1. Bernstein-Vazirani Algorithm: Discover hidden binary strings using quantum computing.
2. **Quantum Phase Estimation (QPE)**—approximate eigenvalues of unitary operators.
3. **Quantum Ripple-Carry Adder**: Implement multi-qubit addition with a quantum adder.
4. Flip-Flop Using Quantum Entanglement: Simulate a flip-flop circuit using quantum entanglement.
5. **True Random Dice Roll Program**: Generate true random numbers and compare quantum randomness with classical methods.

---

## Phase 1: Setting Up the Quantum Environment
### Steps:
1. **Install Dependencies**:
   To start building these quantum solutions, first install the required Python libraries:
   ```bash
   !pip install qiskit numpy matplotlib
   ```
**Qiskit**: Quantum computing framework.
**Numpy**: For numerical computations.
**Matplotlib**: To visualize quantum states and results.

2. **Initialize Quantum Workspace**:
   Create a Qiskit workspace and test basic quantum circuit functionality to ensure everything is set up correctly.

---

## Phase 2: Implementing Bernstein-Vazirani Algorithm
### Problem:
The goal is to find a hidden binary string using quantum circuits.

### Steps:
1. **Circuit Creation**:
Build a quantum circuit with `n+1` qubits, where `n` is the length of the hidden string.
Apply a Hadamard transform to all qubits to create superpositions.
   
2. **Oracle Application**:
- Encode the hidden string using controlled NOT gates.
   
3. **Measurement**:
Measure the resulting qubits to recover the hidden string.

4. **Outcome**:
You successfully recover the hidden binary string after running the quantum circuit.

---

## Phase 3: Quantum Phase Estimation (QPE)
### Problem:
Estimate the phase (eigenvalue) associated with a unitary operator.

### Steps:
1. **Controlled Unitary**:
Implement a unitary operation controlled by several qubits.

2. **Quantum Fourier Transform (QFT)**:
Apply QFT to obtain a superposition that encodes phase information.

3. **Simulation**:
Run the simulation on a quantum backend and measure the eigenvalue estimation.

4. **Outcome**:
You successfully approximate the eigenvalue, which can be used in various quantum algorithms, such as Shor’s algorithm.

---

## Phase 4: Quantum Ripple-Carry Adder
### Problem:
Perform multi-qubit addition using a ripple-carry adder.

### Steps:
1. **Build the Quantum Adder**:
Construct a quantum circuit in which the binary digits of the numbers to be added are represented by qubits.
   
2. **Carry and Sum Operations**:
Implement logic gates to simulate the carry and sum process of binary addition.

3. **Measurement**:
Measure the output qubits to obtain the sum of two binary numbers.

4. **Outcome**:
   The quantum circuit outputs the correct binary sum after successful multi-qubit addition.

---

## Phase 5: Flip-Flop Using Quantum Entanglement (QE)
### Problem:
Simulate a classical flip-flop circuit using the concept of quantum entanglement.

### Steps:
1. **Entangle Qubits**:
Use controlled operations to create entanglement between two qubits, where flipping one qubit flips the state of the other.

2. **State Change**:
Simulate the flip-flop behavior by changing the state of one qubit and observing the immediate effect on the entangled qubit.

3. **Outcome**:
   Demonstrate how quantum entanglement can mimic classical flip-flop behavior, but with quantum superposition and measurement uncertainties.

---

## Phase 6: True Random Program for Dice Roll (Quantum vs Classical Randomness)
### Problem:
Create a program that generates true random numbers using both quantum and classical methods and compares their results.

### Steps:
1. **Classical Randomness**:
Use Python’s `random` library to generate random numbers.
   
2. **Quantum Randomness**:
Use a quantum circuit to generate true random outcomes based on the measurement of superposition states.

3. **Comparison**:
Roll a die using both methods and compare the randomness distribution using histograms.

4. **Outcome**:
Show the difference between classical pseudo-random numbers and true quantum randomness.

---

## Conclusion
This journey from implementing fundamental quantum algorithms to building quantum circuits demonstrates the power of quantum computing in solving complex problems like binary string detection, eigenvalue approximation, multi-qubit addition, and even true randomness generation. By the end of this project, you will have a deep understanding of how quantum mechanics can be leveraged for computational advancements in multiple domains.
