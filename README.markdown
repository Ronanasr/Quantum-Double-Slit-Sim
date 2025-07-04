# Quantum Double-Slit Simulation

## Overview
This project simulates the quantum double-slit experiment using Qiskit, a leading quantum computing framework. The simulation demonstrates fundamental quantum mechanics concepts, including **superposition** and **interference**, through a simple quantum circuit. The circuit applies a Hadamard gate to create superposition, a phase gate to induce interference, and measurements to visualize the resulting probability distribution. The output includes a circuit diagram, a histogram of measurement probabilities, and the quantum state vector, providing a clear illustration of quantum interference patterns.

This project is ideal for showcasing quantum computing skills and understanding of core quantum principles, making it a valuable addition to a technical portfolio or resume.

## Features
- **Quantum Circuit Design**: Implements a single-qubit circuit with Hadamard (`H`) and phase (`P`) gates to simulate the double-slit experiment.
- **Visualization**: Generates a circuit diagram (graphical or text-based) and a probability histogram.
- **State Analysis**: Computes and displays the quantum state vector to verify superposition and interference.
- **Reproducible Results**: Uses Qiskit’s AerSimulator with 10,000 shots for accurate probability distributions.
- **Jupyter Notebook**: Provided as an interactive `.ipynb` file for easy execution and modification.

## Prerequisites
To run this project, ensure you have the following installed:
- Python 3.8+
- Jupyter Notebook
- Required Python packages:
  ```bash
  pip install qiskit qiskit-aer matplotlib pylatexenc
  ```

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/quantum-double-slit-sim.git
   cd quantum-double-slit-sim
   ```

2. **Set Up a Virtual Environment** (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install qiskit qiskit-aer matplotlib pylatexenc
   ```

4. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
   Open the `double_slit_simulation.ipynb` file in the Jupyter interface.

## Usage
1. **Run the Notebook**:
   - Open `double_slit_simulation.ipynb` in Jupyter Notebook.
   - Execute all cells (`Cell > Run All`) to generate the circuit, simulation results, and visualizations.

2. **Expected Outputs**:
   - **Circuit Diagram**: A graphical (or text-based) representation of the quantum circuit.
   - **Probability Histogram**: A plot showing the measurement probabilities for states |0⟩ and |1⟩, saved as `histogram.png`.
   - **Quantum State**: The state vector before measurement, demonstrating superposition and interference.
   - Example state vector: `Statevector([0.70710678+0.j, 0.62054458+0.33900505j], dims=(2,))`.

3. **Customization**:
   - Modify the phase angle in the `P` gate (e.g., `qc.p(phase, 0)`) to explore different interference patterns.
   - Extend to a two-qubit circuit by adding entanglement (e.g., CNOT gate) for a more complex simulation.

## Results
The simulation produces:
- A quantum circuit with a Hadamard gate for superposition, a phase gate (0.5 radians) for interference, and a measurement operation.
- A histogram visualizing the probability distribution, typically showing near-equal probabilities for |0⟩ and |1⟩ with slight variations due to the phase-induced interference.
- A state vector confirming the expected superposition and phase effects.
- https://raw.githubusercontent.com/Ronanasr/quantum-double-slit-sim/main/outputs/filename.png

Saved outputs (`histogram.png` and `circuit.png`) can be used for presentations or documentation.

## Project Structure
```
quantum-double-slit-sim/
├── double_slit_simulation.ipynb  # Main Jupyter Notebook with the simulation code
├── histogram.png                # Saved probability histogram
├── circuit.png                  # Saved circuit diagram (if graphical rendering is enabled)
└── README.md                    # Project documentation
```

## Contributing
Contributions are welcome! Please submit a pull request or open an issue for suggestions, bug reports, or enhancements.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Built with [Qiskit](https://qiskit.org/), an open-source quantum computing framework.
- Inspired by the quantum double-slit experiment, a cornerstone of quantum mechanics.
