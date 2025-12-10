
# Identification of Global Minima (GM) of Pd-Ag-Cu Nanoclusters via Deep Reinforcement Learning

### Accelerating the Global Minimum Search in Pd-Ag-Cu Nanoclusters Using Deep Reinforcement Learning
[Accelerating the global minimum search in Pd-Ag-Cu nanoclusters using DRL_compressed.pdf](https://github.com/user-attachments/files/24066182/Accelerating.the.global.minimum.search.in.Pd-Ag-Cu.nanoclusters.using.DRL_compressed.pdf)

Please cite this article as:  
**Farooq, M. U., & Chen, F. (2025).** Accelerating the global minimum search in Pd-Ag-Cu nanoclusters using deep reinforcement learning. *Applied Surface Science*, 10, 164300. https://doi.org/10.1016/j.apsusc.2025.164300

### How to Run the Code

#### 1. **Set Up the Environment:**
   - Install the required Conda environment using the provided YAML file:
     ```bash
     conda env create -f PdAgCu.yml
     ```

#### 2. **Configure the Nanocluster Composition:**
   - Edit the `PdAgCu.py` file to select the desired nanocluster composition.

   - **Monometallic Nanocluster:** To simulate a cluster of 13 atoms of silver (Ag), set the following configuration:
     ```python
     eleNames = ['Ag']
     eleNums = [13]
     ```

     Any monometallic atomic configuration can be achieved by specifying the chemical element `eleNames` and the number of atoms `eleNums`.

   - **Bimetallic Nanoclusters:**  
     - For a bimetallic cluster of silver (Ag) and palladium (Pd) atoms:
       ```python
       eleNames = ['Pd', 'Ag']
       eleNums = [6, 7]
       ```
     
     - For a bimetallic cluster of palladium (Pd) and copper (Cu) atoms:
       ```python
       eleNames = ['Pd', 'Cu']
       eleNums = [6, 7]
       ```
     
     - For a bimetallic cluster of silver (Ag) and copper (Cu) atoms:
       ```python
       eleNames = ['Ag', 'Cu']
       eleNums = [7, 6]
       ```

     Any bimetallic atomic configuration can be achieved by specifying the chemical elements `eleNames` and the number of atoms `eleNums`.

   - **Trimetallic Nanoclusters:**  
     - For a trimetallic cluster of palladium (Pd), silver (Ag), and copper (Cu) atoms:
       ```python
       eleNames = ['Pd', 'Ag', 'Cu']
       eleNums = [4, 4, 1]
       ```

     - For a trimetallic cluster with different atom numbers:
       ```python
       eleNames = ['Pd', 'Ag', 'Cu']
       eleNums = [4, 4, 3]
       ```

     - Alternatively, another trimetallic configuration:
       ```python
       eleNames = ['Pd', 'Ag', 'Cu']
       eleNums = [4, 4, 5]
       ```

     Any trimetallic atomic configuration can be achieved by specifying the chemical elements `eleNames` and the number of atoms `eleNums`.

#### 3. **Run the Simulation:**
   - Once the nanocluster composition is configured, execute the script using Python:
     ```bash
     python PdAgCu.py
     ```

---

### Open Source Code

This project is open-source, and we encourage you to use and contribute to it. The code is available under the [MIT License](LICENSE). Feel free to fork, modify, and distribute the code as needed. We welcome contributions and feedback from the community to improve the functionality and performance of the model.

