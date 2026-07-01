# About the repository

This repository is a quantum computing portfolio built mainly with Qiskit and Pennylane. It contains a collection of notebooks that implement and explain different quantum computing protocols, algorithms, and techniques.

The repository is organized progressively, starting from more basic concepts and moving towards more advanced topics. The goal is to cover a broad range of areas in quantum computing, including quantum key distribution, entanglement-based protocols, quantum algorithms, error correction, random circuit sampling, quantum optimization and quantum machine learning.

Each notebook is designed to combine theoretical intuition with practical implementation, showing how the main ideas can be translated into executable quantum circuits. The goal is not to provide an extensive or fully rigorous theoretical explanation, but rather to present clear and practical implementations of the main concepts.



## Project Requirements

First, create a virtual environment:

```bash
python -m venv .venv
```

Then activate it:

```bash
# Windows
.venv\Scripts\activate
```

```bash
# macOS/Linux
source .venv/bin/activate
```

Finally, install all required dependencies:

```bash
pip install -r requirements.txt
```


## Usage

Each notebook is independent and can be opened separately. However, the repository is numbered so that the notebooks can be followed in a natural learning order, from introductory topics to more advanced implementations.

Inside each notebook, the cells should be executed sequentially from top to bottom, since later cells may depend on variables, circuits, or functions defined earlier in the notebook.

The recommended workflow is:

1. Create and activate a virtual environment.
2. Install the dependencies from `requirements.txt`.
3. Open the notebooks with Jupyter Notebook, JupyterLab, VS Code, or another compatible environment.
4. Run each notebook cell by cell in order.


## Running on IBM Quantum

To run experiments on real hardware you need an IBM Quantum account and an API token. Install `qiskit-ibm-runtime` and configure your credentials:

```python
from qiskit_ibm_runtime import QiskitRuntimeService
# Store account locally (one-time)
QiskitRuntimeService.save_account(
    token="API_KEY",
    set_as_default = True
    )
# Then instantiate the service in the notebook
service = QiskitRuntimeService()
```

## Sources

- Qiskit documentation: https://quantum.cloud.ibm.com/docs 
- PennyLane documentation: https://docs.pennylane.ai 
- PyTorch documentation: https://pytorch.org/docs/stable/index.html 
- A Practical Guide to Quantum Computing. Elías F. Combarro, Samuel González-Castillo. Packt (2025).
- A Practical Guide to Quantum Machine Learning and Quantum Optimization. Elías F. Combarro, Samuel González-Castillo. Packt (2023).


## License

This project is licensed under the MIT License.