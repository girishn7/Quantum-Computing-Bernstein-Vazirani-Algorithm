# Quantum-Computing-Bernstein-Vazirani-Algorithm

Project Description
The quantum circuit built in this project:

Initializes a quantum register of size length + 1 (6 qubits if length = 5).
Applies an X gate to the last qubit.
Applies Hadamard gates to all qubits to create superposition.
Uses CNOT gates to entangle certain qubits with the last qubit.
Measures the first length qubits.
Visualizes the circuit and the measurement results.
This is typically an example of a quantum algorithm showcasing entanglement and measurement outcomes in a simulated quantum environment.

How It Works
1. Circuit Initialization
Creates a QuantumCircuit with length + 1 qubits and length classical bits.
circuit.x(length) flips the last qubit (qubit 5 in this case).
2. Superposition
circuit.h(range(length + 1)) applies Hadamard gates to all qubits to create superposition.
3. Entanglement with CNOT Gates
Entangles qubits 1, 2, and 4 with the last qubit (qubit 5) via CNOT gates.
4. Measurement
The first length qubits (qubits 0 to 4) are measured into classical bits.
5. Simulation and Visualization
The circuit is simulated on AerSimulator backend.
Measurement results (counts) are collected and plotted as a histogram.
