## Mlflow Tracking, Experiments, Model, and Projects Tutorial

This tutorial was created and tested on macOS Monterey version 12.1 Macbook Pro, 2.2 GHz Quad-Core Intel Core i7, Memory 16GB DDR3
Here is the **installation instructions** using Conda environment
> 1. Make sure that you have the Conda environment installed. In my case, I had Conda 4.10.3 installed in MacOS version specified above
> 2. Copy the github repo from the url below from the MacOS terminal where the contents will be saved in the directory called mlflow
  ```
  $ git clone https://github.com/maximuslee1226/mlflow.git
  ```
> 3. Create a conda virtual environment by typing the below command
  ```
  $ conda env create -f conda.yaml
  ```
> 4. Activate Conda virtual environment called mlflowtest
  ```
  $ conda activate -f mlflow test
  ```
> 5. Launch MLFlow server from the conda environment by typing
  ```
  $ mlflow server --backend-store uri="sqlite:////Users/brandonl/projects/mlflow/fastcamp/backend/mlflow_data.db" \
                  --default-artifact-root="file:///Users/brandonl/projects/mlflow/fastcamp/artifact_store"
  ```
  ***Note: make sure that you have four slashes after sqlite***
> 6. Launch Jupyter notebook from the conda environment by typing
  ```
  $ jupyter notebook
  ```
  ***Note: if the jupyter notebook does not launch in a web browser, copy the jupyter notebook url that was created by jupyter notebook command and manually past that into your browser of interest***
> 7. Test the MLFlow client using the following url in your web browser
  ```
  http://127.0.0.1:5000/
  ```
> 8. You should be able to see MLFlow UI upon typing the address above

Now you are ready to fully utilize MLFlow server in your local environment. Please go to notebook folder to start having fun!
