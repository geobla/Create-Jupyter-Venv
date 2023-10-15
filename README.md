# Create Virtual environment for Jupyter Notebook
Creating separate virtual environments (venvs) for each Jupyter notebook is a good practice to avoid package conflicts and maintain clean, isolated environments for different projects.<br> 

Here's a step-by-step guide on how to achieve this using the command line `bash`, or from inside `Jupyter`:

## Create a Virtual Environment from Command Line

### Install Virtualenv:

If you haven't already installed virtualenv, do so with:

```bash
pip install virtualenv
```
### Create a New Virtual Environment:

Navigate to the directory where you want to store your venv and create a new one:

```bash
virtualenv my_notebook_venv
```
Replace `my_notebook_venv` with a name that's relevant to your notebook.

### Activate the Virtual Environment:

On macOS and Linux:

```bash
source my_notebook_venv/bin/activate
```

On Windows (using Command Prompt):

```bash
.\my_notebook_venv\Scripts\activate
```

### Install Jupyter Within the Virtual Environment:

```bash
pip install jupyter
```

### Launch Jupyter Notebook:

```bash
jupyter notebook
```

### Deactivate the Virtual Environment:

Once you're done, you can deactivate the virtual environment by simply running:

```bash
deactivate
```

## Create a Virtual Environment from inside Jupyter

<code>python -m venv name_of_your_venv</code>

```bash
!python -m venv tradingview_venv
```

### Activate the Virtual Environment:"

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
