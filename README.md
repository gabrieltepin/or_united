# Setup

## Mac OS
```Bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Windows
```Bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

In VSCode, install the ipynb environment, select the kernel as the _venv/bin/python_ to run the notebook

## Gurobi installation

- In the virtual environment run the command:
```Bash
grbgetkey xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
```
_Where the xxxx... is your gurobi license number_

- Set the path to this workspace, and create a .env file with the path variable for the gurobi module to find the licence (mine is in the version 11.0.0 and it is specified in the requirements.txt file)
```Bash
GRB_LICENSE_FILE=/PATH_TO_YOUR_PROJECT/gurobi.lic
```

# Running the project

Now, with the dependencies configured, just run the main.ipynb file notebook!
