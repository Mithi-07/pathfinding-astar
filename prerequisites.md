If you don't have python installed in your computer or you don't have any one of the libraries installed, you can run the program in Google Collab to get the output.

## Installation

### Prerequisites

Before installing, make sure you have Python installed. You can download Python from [python.org](https://www.python.org/).

### Installing Required Libraries

You can install the necessary libraries using `pip`. Open your terminal or command prompt and execute the following commands:

1. **matplotlib**:
   ```bash
   pip install matplotlib

2. **ipywidgets (for Jupyter notebooks)**:
   ```bash
   pip install ipywidgets
   jupyter nbextension enable --py widgetsnbextension

3. **If you are using JupyterLab, also run**:
   ```bash
   jupyter labextension install @jupyter-widgets/jupyterlab-manager

4. **numpy**:
   ```bash
   pip install numpy

5. **Verify Installation: To verify that the installation was successful, you can try importing the libraries in a Python script or in a Jupyter notebook:**:
   ```bash
   import matplotlib.pyplot as plt
   import ipywidgets as widgets
   import numpy as np

   
