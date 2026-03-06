# A-Novel-Mechanobiological-Model-for-Bone-Healing-Incorporating-Implant-Degradation
Agent-based mechanobiological model simulating scaffold degradation, MSC behavior, and time-dependent bone formation in 3D-printed polymeric scaffolds. Includes full implementation of degradation rules, cell migration, proliferation, differentiation, apoptosis, and Abaqus FE coupling.


This repository contains the computational framework used to simulate scaffold degradation, mechanoregulated tissue differentiation, and bone regeneration in a large bone defect. The model integrates finite element analysis (Abaqus) with an agent-based biological model to simulate the interaction between mechanical environment, scaffold degradation, and cellular behaviour during healing.

Each simulation iteration represents one healing day, during which Abaqus outputs are used to update biological processes including MSC migration, proliferation, differentiation, apoptosis, and scaffold degradation.

Code Structure

The simulation framework consists of four main modules:

1. Reading Files
Reads Abaqus job files, identifies model components (upper bone, lower bone, scaffold, and callus), and extracts node and element coordinates.

2. Grid Creation and Mapping
Creates a 3D lattice grid and maps model parts into the grid, allowing agents to interact with their local mechanical environment.

3. Biological Functions and Degradation
Updates biological processes including MSC migration, proliferation, differentiation, apoptosis, and scaffold degradation based on mechanical stimuli.

4. Main Code
Controls the execution of all modules and manages the time-dependent simulation loop.

Dependencies

Required software:

Python

Jupyter Notebook

Abaqus (Finite Element Analysis)

Python libraries used:

NumPy

SciPy

Pandas

Matplotlib

Running the Model

The simulation is implemented in Jupyter Notebook format (.ipynb).

Install Python and Jupyter Notebook.

Open the notebook file in Jupyter.

Run the cells sequentially to execute the simulation.

The model runs iteratively, updating mechanical and biological processes for each healing day.
