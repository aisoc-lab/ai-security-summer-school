# AI and Security Summer School

Welcome to the code repository for the [CASA RC Trust Summer School 2025 on AI and Security](https://casa.rub.de/veranstaltungen/casa-summer-school/casa-rct-summer-school-2025). This repository contains various code examples, exercises, and resources that will be used throughout the tutorial sessions. 
Below, we provide a setup guide to help you prepare your environment for the summer school.
To ensure a smooth experience during the summer school, please follow the setup guide below to prepare your environment and install the necessary dependencies before the sessions begin.


Each tutorial session has its own directory with relevant code, examples, and instructions.
The sessions may require additional setup (e.g., downloading models, datasets), which will be detailed in the respective directories.


## Setup Guide
We will use Jupyter notebooks for the exercises and tutorials. Jupyter notebooks allow us to run Python code interactively. 
If you are not familiar with Jupyter notebooks, you can find a [quick introduction here](https://www.dataquest.io/blog/jupyter-notebook-tutorial/) and the [official documentation here](https://jupyter.org/documentation).
You can run these notebooks either on your local machine or on Google Colab, which provides free access to GPUs for more intensive computations. We will provide instructions for both options below.


### 1. Local Setup
Most exercises and notebooks will run fine on your local machine. Here's how to set it up:



#### Setup Instructions

1. **Install Miniconda/Anaconda**:

   Miniconda/Anaconda is a package manager that simplifies the installation of Python packages and their dependencies. 
   If you don't have Miniconda or Anaconda installed yet, you can download it from the [official website](https://docs.conda.io/en/latest/miniconda.html) and follow the installation instructions for your operating system.

2. **Clone the repository**:
   ```bash
   git clone https://github.com/aisoc-lab/ai-security-summer-school.git
    cd ai-security-summer-school
    ```
3. **Create a conda environment**:
    ```bash
    conda create -n aisec python=3.12
    ```
4. **Activate the environment**:
    ```bash
    conda activate aisec
    ```
5. **Install the project with pip**:
    ```bash
    python -m pip install -e .
    ```
6. **Start jupyter notebook**:
    ```bash
    jupyter notebook
    ```
   This will open Jupyter in your web browser, and you can navigate to the tutorial directories to start working on the exercises.
   To run the code from within our aisec environment, you may need to add the conda environment as a kernel in Jupyter manually. You can do this by running the following command in your terminal:
   ```bash
   python -m ipykernel install --user --name=aisec --display-name "Python (aisec)"
   ```
   Then, you can select the "Python (aisec)" kernel in Jupyter Notebook when you open a notebook (click on "Kernel" > "Change kernel" > "Python (aisec)").


NOTE: Some exercises may require additional setup, such as downloading specific models or datasets. Check the README files in each tutorial directory for specific instructions.

### 2. Running on Google Colab
As we progress, we may hit the compute limits of our local machines. We have designed the exercises to also run on Google Colab, which provides free GPU access.

#### Stepsto Run on Colab
1. **Open Google Colab**:
   Go to [Google Colab](https://colab.research.google.com/).
2. **Upload the Notebook**:
   - Click on "File" > "Upload Notebook" and select the notebook you want to work on from the `ai-security-summer-school` directory, as well as the `requirements.txt` file.
3. **Runtime Configuration**:
   - Go to "Runtime" > "Change runtime type" and select "GPU" as the hardware accelerator.
4. **Install Dependencies**:
    - In a new code cell, run:
      ```python
      !pip install -r requirements.txt
      ```
5. **Run the Notebook**:
   - You can now run the cells in the notebook as you would normally do in Jupyter. If you are new to Colab, you can find a [quick introduction here](https://colab.research.google.com/notebooks/intro.ipynb).


## Important Notes and Pitfalls

### Shut Down Your Colab Instance
Colab notebooks have a limited runtime and may disconnect after a period of inactivity.
Don't forget to manually save your work and important outputs to Google Drive or download them locally. 
Colab also has limits on GPU usage, so remember to shut down your Colab instance when you are done working or taking a break to avoid hitting the limits.

### Avoiding Common Errors
* Always activate the correct environment before running the notebooks locally.
* If you install new packages inside a notebook on Colab, use `!pip install` to ensure they are installed in the Colab environment. You may need to restart the runtime after installing new packages.
* Be mindful of version mismatches between your local environment and Colab. Check pacakge versions if things break.

We are happy to help you with any issues you encounter during the setup or while running the exercises.


