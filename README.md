# CASA RC Trust Summer School 2025: AI and Security

Welcome to the code repository for the CASA RC Trust Summer School 2025 on AI and Security. This repository contains various code examples, exercises, and resources that will be used throughout the tutorial sessions. 
Below, we provide a setup guide to help you prepare your environment for the summer school.
To ensure a smooth experience during the summer school, please follow the setup guide below to prepare your environment and install the necessary dependencies before the sessions begin.


Each tutorial session has its own directory with relevant code, examples, and instructions.
The sessions may require additional setup (e.g., downloading models, datasets, etc.), which will be detailed in the respective directories.


## Setup Guide
To get started, please follow these steps:

### 1. Local Setup
Most exercises and notebooks will run fine on your local machine. Here's how to set it up:

#### Prerequisites
- Python 3.8 or higher
- Miniconda or Anaconda

#### Setup Instructions
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/aisoc-lab/casa-summer-school-25.git
    cd casa-summer-school-25
    ```
2. **Create a Conda Environment**:
    ```bash
    conda create -n casa-summer-school python=3.8
    ```
3. **Activate the Environment**:
    ```bash
    conda activate casa-summer-school
    ```
4. **Install Required Packages**:
    ```bash
    pip install -r requirements.txt
    ```
5. **Start Jupyter Notebook**:
    ```bash
    jupyter notebook
    ```
   This will open Jupyter in your web browser, and you can navigate to the tutorial directories to start working on the exercises.


NOTE: Some exercises may require additional setup, such as downloading specific models or datasets. Check the README files in each tutorial directory for specific instructions.

### 2. Running on Google Colab
As we progress, we may hit the compute limits of our local machines. We have designed the exercises to also run on Google Colab, which provides free GPU access.

#### Stepsto Run on Colab
1. **Open Google Colab**:
   Go to [Google Colab](https://colab.research.google.com/).
2. **Upload the Notebook**:
   - Click on "File" > "Upload Notebook" and select the notebook you want to work on from the `casa-summer-school-25` directory, as well as the `requirements.txt` file.
3. **Runtime Configuration**:
   - Go to "Runtime" > "Change runtime type" and select "GPU" as the hardware accelerator.
4. **Install Dependencies**:
    - In a new code cell, run:
      ```python
      !pip install -r requirements.txt
      ```
5. **Run the Notebook**:
   - You can now run the cells in the notebook as you would normally do in Jupyter.


## Important Notes and Pitfalls

### Resource Management
Colab notebooks have a limited runtime and may disconnect after a period of inactivity.
Don't forget to manually save your work and important outputs to Google Drive or download them locally. 
Colab also has limits on GPU usage, so remember to shut down your Colab instance when not in use to free up memory.

### Avoiding Common Errors
* Always activate the correct environment before running the notebooks locally.
* If you install new packages inside a notebook on Colab, use `!pip install` to ensure they are installed in the Colab environment. You may need to restart the runtime after installing new packages.
* Be mindful of version mismatches between your local environment and Colab. Check pacakge versions if things break.

We are happy to help you with any issues you encounter during the setup or while running the exercises.


