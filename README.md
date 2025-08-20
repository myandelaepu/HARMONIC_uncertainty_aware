# HARMONIC_uncertainty_aware
HARMONIC: Bayesian Neural Network for uncertainty-aware HPC job scheduling. Multi-objective optimization balancing performance, energy efficiency, and resilience. Validated on ALCF traces with significant energy improvements over FCFS, EASY, E-HEFT, and DeepRM baselines. 

The system addresses three critical challenges:
•	Uncertainty Quantification: Bayesian inference for prediction uncertainty
•	Multi-objective Optimization: Balancing performance, energy efficiency, and system resilience
•	Scalable Decision Making: Real-time scheduling for large-scale HPC systems

# Installation
Prerequisites
•	Python 3.8 or higher
•	CUDA-capable GPU (optional, for accelerated training)
Setup
1.	Clone the repository:
git clone https://github.com/username/harmonic-hpc-scheduler.git
cd harmonic-hpc-scheduler
2.	Create virtual environment:
python -m venv harmonic_env
source harmonic_env/bin/activate  # On Windows: harmonic_env\Scripts\activate
3.	Install dependencies:
pip install -r requirements.txt
Repository Structure
harmonic-hpc-scheduler/
├── src/
│   ├── harmonic_main.py           
│   ├── models/
│   │   ├── bayesian_nn.py         
│   │   └── uncertainty.py         
│   ├── schedulers/
│   │   ├── harmonic_scheduler.py  
│   │   └── baselines.py          
│   ├── data/
│   │   ├── loader.py             
│   │   └── preprocessing.py      
│   └── visualization/
│       ├── plots.py              
│       └── analysis.py           
├── data/                         
├── results/                     
├── tests/                        
├── docs/                         
├── requirements.txt              
├── setup.py                      
└── README.md


# Data Requirements
The implementation supports multiple data sources:
Production Datasets (Recommended)
•	Argonne National Laboratory (ALCF) traces: 
•	Download: Available from the Parallel Workloads Archive
•	DOI: https://doi.org/10.21227/bhfr-wx19



