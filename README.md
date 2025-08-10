# Pd-Ag-Cu-Nanoclusters-by-DRL

### Accelerating the Global Minimum Search in Pd-Ag-Cu Nanoclusters Using Deep Reinforcement Learning 



### How to Run the Code

1. **Set Up the Environment:**
   - Install the required Conda environment using the provided YAML file:
     ```bash
     conda env create -f PdAgCu.yml
     ```

2. **Configure the Nanocluster Composition:**
   - Edit `PdAgCu.py` to select the nanocluster composition.

   - **Monometallic Nanocluster:** For simulating a cluster of 13 atom silver (Ag):
     ```python
     eleNames = ['Ag']
     eleNums = [13]

     Any monometallic atomic configuration can be achieved by specifying the chemical element `eleNames` and the number of atoms `eleNums`.
     ```
   - **Bimetallic Nanoclusters:** For simulating a bimetallic cluster of silver (Ag) and palladium (Pd) atoms:
     ```python
     eleNames = ['Pd', 'Ag']
     eleNums = [6, 7]

     Any bimetallic atomic configuration can be achieved by specifying the chemical element `eleNames` and the number of atoms `eleNums`.
     ```

   - **Trimetallic Nanoclusters:** For simulating a trimetallic cluster of palladium (Pd), silver (Ag), and copper (Cu) atoms:
     ```python
     eleNames = ['Pd', 'Ag', 'Cu']
     eleNums = [4, 4, 5]

     Any trimetallic atomic configuration can be achieved by specifying the chemical element `eleNames` and the number of atoms `eleNums`.
     ```

3. **Run the Simulation:**
   - Execute the script using Python. 
     ```bash
     python PdAgCu.py  
