# **Frequently Asked Questions**
- [**Frequently Asked Questions**](#frequently-asked-questions)
- [A Detailed Guide to Running Python Jupyter Notebooks](#a-detailed-guide-to-running-python-jupyter-notebooks)
  - [Steps for Windows](#steps-for-windows)
    - [Step 1: Install `pyenv-win` (Python Version Manager)](#step-1-install-pyenv-win-python-version-manager)
    - [Step 2: Install a Specific Python Version Using `pyenv-win`](#step-2-install-a-specific-python-version-using-pyenv-win)
    - [Step 3: Create and Activate a Virtual Environment](#step-3-create-and-activate-a-virtual-environment)
    - [Step 4: Install JupyterLab and Standard Libraries](#step-4-install-jupyterlab-and-standard-libraries)
    - [Step 5: Run JupyterLab in the Browser](#step-5-run-jupyterlab-in-the-browser)
    - [Step 6: Run `.py` Files from Terminal](#step-6-run-py-files-from-terminal)
  - [Steps for Mac](#steps-for-mac)
    - [Step 1: Install `pyenv` (Python Version Manager)](#step-1-install-pyenv-python-version-manager)
    - [Step 2: Install a Specific Python Version Using `pyenv`](#step-2-install-a-specific-python-version-using-pyenv)
    - [Step 3: Create and Activate a Virtual Environment](#step-3-create-and-activate-a-virtual-environment-1)
    - [Step 4: Install JupyterLab and Standard Libraries](#step-4-install-jupyterlab-and-standard-libraries-1)
    - [Step 5: Run JupyterLab in the Browser](#step-5-run-jupyterlab-in-the-browser-1)
    - [Step 6: Run `.py` Files from Terminal](#step-6-run-py-files-from-terminal-1)
  - [Running Notebooks in Google Colab](#running-notebooks-in-google-colab)
    - [Step 1: Create a Google Account](#step-1-create-a-google-account)
    - [Step 2: Access Google Colab](#step-2-access-google-colab)
    - [Step 3: Create a New Notebook](#step-3-create-a-new-notebook)
    - [Step 4: Importing and Using Datasets in Colab](#step-4-importing-and-using-datasets-in-colab)
    - [Step 5: Using Google Drive with Colab](#step-5-using-google-drive-with-colab)
    - [Step 6: Installing Additional Libraries in Colab](#step-6-installing-additional-libraries-in-colab)
    - [Step 7: Saving and Sharing Notebooks](#step-7-saving-and-sharing-notebooks)
  - [References for Data Sources and Further Reading](#references-for-data-sources-and-further-reading)
    - [Data Sources](#data-sources)
    - [Free Online Books for Further Reading](#free-online-books-for-further-reading)
    - [Computer Science](#computer-science)
  - [FAQ and Potential Issues](#faq-and-potential-issues)
    - [1. Q: How do I deactivate the virtual environment?](#1-q-how-do-i-deactivate-the-virtual-environment)
    - [2. Q: What if `pyenv` commands are not recognized?](#2-q-what-if-pyenv-commands-are-not-recognized)
    - [3. Q: What if JupyterLab doesn’t open automatically in the browser?](#3-q-what-if-jupyterlab-doesnt-open-automatically-in-the-browser)
    - [4. Q: How do I install additional libraries later?](#4-q-how-do-i-install-additional-libraries-later)
    - [5. Q: How do I remove a virtual environment?](#5-q-how-do-i-remove-a-virtual-environment)
    - [6. Q: What if I get permission errors when installing Homebrew on Mac?](#6-q-what-if-i-get-permission-errors-when-installing-homebrew-on-mac)
    - [7. Q: Why isn’t `pyenv` installing Python versions on Mac?](#7-q-why-isnt-pyenv-installing-python-versions-on-mac)

---

# A Detailed Guide to Running Python Jupyter Notebooks

Here's a detailed guide to help a beginner run Python Jupyter Notebooks on both Windows and Mac machines using `pyenv-win` or `pyenv` for managing Python versions, `venv` for virtual environments, and other related tasks.

## Steps for Windows

### Step 1: Install `pyenv-win` (Python Version Manager)
1. **Open PowerShell as Administrator**:
   - Press `Windows + X` and choose **Windows PowerShell (Admin)**.

2. **Install `pyenv-win`**:
   In PowerShell, run the following commands:
   ```bash
   Invoke-WebRequest -UseBasicParsing https://pyenv.run | Invoke-Expression
   ```
   After installation, restart PowerShell and verify by running:
   ```bash
   pyenv --version
   ```

### Step 2: Install a Specific Python Version Using `pyenv-win`
1. List available Python versions:
   ```bash
   pyenv install --list
   ```

2. Install a specific version (e.g., Python 3.10.5):
   ```bash
   pyenv install 3.10.5
   ```

3. Set the global Python version:
   ```bash
   pyenv global 3.10.5
   ```

4. Verify the Python version:
   ```bash
   python --version
   ```

### Step 3: Create and Activate a Virtual Environment
1. Create a new directory for your project (optional):
   ```bash
   mkdir my_project
   cd my_project
   ```

2. Create a virtual environment using `venv`:
   ```bash
   python -m venv venv
   ```

3. Activate the virtual environment:
   ```bash
   .\venv\Scripts\activate
   ```

### Step 4: Install JupyterLab and Standard Libraries
1. Upgrade `pip` (Python package installer):
   ```bash
   python -m pip install --upgrade pip
   ```

2. Install JupyterLab:
   ```bash
   pip install jupyterlab
   ```

3. Install other libraries (e.g., NumPy, Pandas, Matplotlib):
   ```bash
   pip install numpy pandas matplotlib
   ```

### Step 5: Run JupyterLab in the Browser
1. Start JupyterLab:
   ```bash
   jupyter lab
   ```

2. A browser window will automatically open with JupyterLab. If not, copy the URL provided in the terminal and paste it into the browser.

### Step 6: Run `.py` Files from Terminal
1. Navigate to the folder where your `.py` file is located:
   ```bash
   cd path_to_your_script
   ```

2. Run the Python script:
   ```bash
   python your_script.py
   ```

---

## Steps for Mac

### Step 1: Install `pyenv` (Python Version Manager)
1. **Open Terminal**:
   - Use `Cmd + Space`, search for **Terminal**, and open it.

2. **Install Homebrew** (if you don't have it):
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

3. **Install `pyenv`**:
   ```bash
   brew install pyenv
   ```

4. Add `pyenv` to your shell configuration:
   ```bash
   echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.bash_profile
   echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bash_profile
   echo 'eval "$(pyenv init --path)"' >> ~/.bash_profile
   source ~/.bash_profile
   ```

5. Verify `pyenv` installation:
   ```bash
   pyenv --version
   ```

### Step 2: Install a Specific Python Version Using `pyenv`
1. List available Python versions:
   ```bash
   pyenv install --list
   ```

2. Install a specific version (e.g., Python 3.10.5):
   ```bash
   pyenv install 3.10.5
   ```

3. Set the global Python version:
   ```bash
   pyenv global 3.10.5
   ```

4. Verify the Python version:
   ```bash
   python --version
   ```

### Step 3: Create and Activate a Virtual Environment
1. Create a new directory for your project (optional):
   ```bash
   mkdir my_project
   cd my_project
   ```

2. Create a virtual environment using `venv`:
   ```bash
   python -m venv venv
   ```

3. Activate the virtual environment:
   ```bash
   source venv/bin/activate
   ```

### Step 4: Install JupyterLab and Standard Libraries
1. Upgrade `pip` (Python package installer):
   ```bash
   python -m pip install --upgrade pip
   ```

2. Install JupyterLab:
   ```bash
   pip install jupyterlab
   ```

3. Install other libraries (e.g., NumPy, Pandas, Matplotlib):
   ```bash
   pip install numpy pandas matplotlib
   ```

### Step 5: Run JupyterLab in the Browser
1. Start JupyterLab:
   ```bash
  

 jupyter lab
   ```

2. A browser window will automatically open with JupyterLab. If not, copy the URL provided in the terminal and paste it into the browser.

### Step 6: Run `.py` Files from Terminal
1. Navigate to the folder where your `.py` file is located:
   ```bash
   cd path_to_your_script
   ```

2. Run the Python script:
   ```bash
   python your_script.py
   ```

---

## Running Notebooks in Google Colab

Google Colab is a free cloud-based environment that allows you to run Jupyter notebooks without any local setup. Here’s how to get started:

### Step 1: Create a Google Account
- If you don’t have one, create a Google account at [accounts.google.com](https://accounts.google.com).

### Step 2: Access Google Colab
- Go to [Google Colab](https://colab.research.google.com/).

### Step 3: Create a New Notebook
1. Click on **File** > **New Notebook**.
2. A new notebook will open in a new tab.

### Step 4: Importing and Using Datasets in Colab
- Use the following code to import datasets (for example, from a CSV file):
  ```python
  import pandas as pd

  # Load a dataset from a URL
  df = pd.read_csv('https://example.com/your-dataset.csv')
  ```

### Step 5: Using Google Drive with Colab
- To access files from your Google Drive, run the following:
  ```python
  from google.colab import drive
  drive.mount('/content/drive')
  ```

### Step 6: Installing Additional Libraries in Colab
- To install libraries, use `pip` as you would normally:
  ```python
  !pip install your-library
  ```

### Step 7: Saving and Sharing Notebooks
- Notebooks are saved automatically in your Google Drive. You can share them by clicking the **Share** button in the top right corner.

---

## References for Data Sources and Further Reading

### Data Sources
- [Kaggle Datasets](https://www.kaggle.com/datasets)
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)
- [Data.gov](https://www.data.gov/)

### Free Online Books for Further Reading
- [Python for Data Analysis by Wes McKinney](https://www.oreilly.com/library/view/python-for-data/9781449323592/)
- [Think Python: How to Think Like a Computer Scientist](https://greenteapress.com/wp/think-python-2e/)
- [Automate the Boring Stuff with Python](https://automatetheboringstuff.com/)
- [Python Documentation](https://docs.python.org/3/)
- [W3Schools Python](https://www.w3schools.com/python/)
- [Real Python](https://realpython.com/)

### Computer Science
- [Open Source CS with Python](https://github.com/ForrestKnight/open-source-cs-python)
- [MIT Computer Science](https://www.youtube.com/playlist?list=PLUl4u3cNGP63WbdFxL8giv4yhgdMGaZNA)

---

## FAQ and Potential Issues

### 1. Q: How do I deactivate the virtual environment?
- A: Run `deactivate` in the terminal.

### 2. Q: What if `pyenv` commands are not recognized?
- A: Ensure that `pyenv` is properly installed and that your shell configuration is set up correctly. Restart the terminal.

### 3. Q: What if JupyterLab doesn’t open automatically in the browser?
- A: Check the terminal for a URL, copy it, and paste it into your web browser.

### 4. Q: How do I install additional libraries later?
- A: Activate your virtual environment and use `pip install library_name`.

### 5. Q: How do I remove a virtual environment?
- A: Simply delete the directory containing the virtual environment.

### 6. Q: What if I get permission errors when installing Homebrew on Mac?
- A: Run the installation command with `sudo` if you encounter permission issues.

### 7. Q: Why isn’t `pyenv` installing Python versions on Mac?
- A: Ensure that you have the required build tools and libraries installed. Use `brew install openssl readline sqlite3 xz zlib` to install necessary dependencies.

---
