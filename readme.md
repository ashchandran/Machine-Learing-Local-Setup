# Machine Learning Setup Instructions

## Pre Requsites

You will need to have these two nstalled on your system before starting
- Python
- pip

Then install `virtualenv` globally

````sh
pip install virtualenv
````
## Setup

Once those pre-requsites are up you have to do the following

1. Create folder that should contain the project and dependencies to reside
2. `cd` to that folder in your terminal of choice
3. make a virtual environment there
    ````sh
    virtualenv <PROJ_NAME>
    ````
4. activate virtual environment (this basically just runs the bash or powershell file in your Scripts folder)
    ````sh
    cd <PROJ_NAME>
    Scripts/activate
    ````
5. install dependencies
    ````sh
    pip install -r requirements.txt
    ````
    or if that doesnt work (I havent tried it myself), you can do what i did and maually install the dependencies
    ````sh
    pip install jupyter numpy scipy scikit-learn pandas seaborn 
    ````

## Usage

Now that we have the dependencies locally in the virtual environment we can do the ML bit

run jupyter

````sh
juypter notebook
````

Navigate to the Notebooks folder and open the notebook `First Notebook`. This has the sample Machine learning code that i played with.

The data folder in the root has the dataset i tried running the algorithms on

Create more notbooks in the `Notebooks` folder for other tests. All this can be done directly from jupyter notbooks web interface.

`Ctrl + C` in the terminal to exit the notebook and run the command `deactivate` to exit the virtual environment
