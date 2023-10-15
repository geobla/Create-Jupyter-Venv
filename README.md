# Create Virtual environment for Jupyter Notebook
Creating separate virtual environments (venvs) for each Jupyter notebook is a good practice to avoid package conflicts and maintain clean, isolated environments for different projects.<br> 

Here's a step-by-step guide on how to achieve this using the command line `bash`, or from inside `Jupyter`:
## Create a Virtual Environment from inside Jupyter
<code>python -m venv name_of_your_venv</code>
```bash
!python -m venv tradingview_venv
```
## Activate the Virtual Environment:"
```bash
import sys
```
<code>!{sys.executable} -m ipykernel install --user --name=name_of_your_venv</code>
```bash
!{sys.executable} -m ipykernel install --user --name=tradingview_venv
```
## Switch to the New Kernel:
If you're using `Jupyter Notebook`: Click on `Kernel` > `Change kernel` and select `tradingview_venv` from the dropdown list.<br>
If you're using `Jupyter Lab`: Click on the `kernel name` in the top right corner and select `tradingview_venv` from the dropdown list.
