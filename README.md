Quantum AI Robustness Benchmarking under Depolarizing Noise ⚛️

This project presents a detailed robustness benchmarking of fundamental quantum algorithms under depolarizing noise using **Qiskit simulators** and **real IBM Quantum hardware**.  
The study focuses on understanding how noise affects quantum algorithm reliability on current **NISQ devices**.



## 📌 Project Overview & Motivation

Quantum computers are inherently noisy, and real-world quantum hardware deviates significantly from ideal simulations.  
For Quantum AI and near-term quantum applications, it is crucial to evaluate **algorithm robustness under realistic noise conditions**.

This project benchmarks the behavior of selected quantum algorithms under depolarizing noise to analyze:
- Noise sensitivity
- Performance degradation
- Simulator vs real hardware gaps


## 🧠 Algorithms Implemented

The following quantum algorithms were implemented and analyzed:

- **Bernstein–Vazirani Algorithm**
- **Simon’s Algorithm**
- **Grover’s Search Algorithm**

These algorithms were chosen due to their differing circuit depths, interference patterns, and sensitivity to noise.


## 🧪 Experimental Setup

- **Quantum SDK:** Qiskit  
- **Simulator:** Qiskit Aer (ideal & noisy simulation)  
- **Hardware:** IBM Quantum backends  
- **Noise Model:** Depolarizing noise  
- **Evaluation Metrics:**
  - Success probability
  - Accuracy degradation
  - Noise sensitivity trends
  - Simulator vs hardware comparison


## 📊 Key Results & Observations

- Bernstein–Vazirani demonstrated **high robustness** due to shallow circuit depth.
- Simon’s algorithm showed **moderate degradation** caused by interference sensitivity.
- Grover’s algorithm was **most noise-sensitive**, with rapid breakdown of amplitude amplification.
- Real quantum hardware exhibited **higher error rates** compared to simulations, highlighting NISQ limitations.


## 📁 Repository Structure

Quantum-AI-Robustness-Benchmark/
│
├── quantum/
│ ├── bv.py
│ ├── bv_noise.py
│ ├── bv_noise_graph.py
│ ├── bv_real_hardware.py
│ ├── bv_sim_vs_real.py
│ ├── grover.py
│ ├── grover_noise_graph.py
│ ├── simon.py
│ ├── simon_noise_graph.py
│
├── bv_circuit.png
├── grover_circuit.png
├── simon_circuit.png
├── .gitignore
├── README.md


## 🚀 How to Run the Project

### 1️⃣ Clone the repository
git clone https://github.com/shlok926your-username/Quantum-AI-Robustness-Benchmark.git
cd Quantum-AI-Robustness-Benchmark

2️⃣ Install required dependencies
pip install qiskit qiskit-aer qiskit-ibm-runtime matplotlib numpy

3️⃣ Run the algorithms
python quantum/bv_noise.py
python quantum/grover.py
python quantum/simon.py


🔐 Security & API Key Management (IMPORTANT)
API keys are NOT stored in this repository.

To run experiments on real IBM Quantum hardware:

Store your API key as an environment variable

Do NOT hardcode credentials in source files

Example (Windows PowerShell)
powershell
Copy code
setx IBM_QUANTUM_API_KEY "your_api_key_here"
Secure usage in code
python
Copy code
import os
from qiskit_ibm_runtime import QiskitRuntimeService

service = QiskitRuntimeService(
    channel="ibm_quantum",
    token=os.getenv("IBM_QUANTUM_API_KEY")
)

📈 Results & Visualization
Noise vs accuracy graphs generated using matplotlib

Circuit diagrams included for clarity

Simulator vs real hardware performance comparison highlights real-world noise effects


🔮 Future Scope
Implementation of error mitigation techniques (ZNE, readout mitigation)

Robustness benchmarking for VQE and Quantum Machine Learning models

Backend-wise comparative analysis

Noise-aware circuit optimization


🎓 Academic & Interview Relevance
This project demonstrates:

Practical quantum algorithm implementation

Noise modeling and benchmarking

Real quantum hardware execution

Secure credential management

Research-oriented analysis approach


📜 License / Disclaimer
This project is intended for academic and research purposes.


## ✅ FINAL CONFIRMATION (Checklist Match)

| Checklist Item | Covered |
|---------------|--------|
| Project title | ✅ |
| Description | ✅ |
| Motivation | ✅ |
| Algorithms | ✅ |
| Experimental setup | ✅ |
| Results | ✅ |
| Repo structure | ✅ |
| How to run | ✅ |
| Security section | ✅ |
| Future scope | ✅ |
| Academic relevance | ✅ |
