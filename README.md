# QDFT
Quantum Density Functional Theory: a quantum algorithm to solve the Kohn-Sham self-consistent equations.

# Installation

Install Psi4 from [here](https://psicode.org/installs/v182/):
1. Select `Installer`, `wget` install script listed in the box below "Run this command": E.g. `wget http://vergil.chemistry.gatech.edu/psicode-download/Psi4conda-1.8.2-py311-Linux-x86_64.sh`.
2. Execute install script with `bash downloaded_install_script.sh -b -p $HOME/psi4conda` and change `downloaded_install_script.sh` to the name of the downloaded install script. This installs Psi4 into the folder `psi4conda` in the home directory which is a conda environment.
3. Activate conda environment with `. $HOME/psi4conda/etc/profile.d/conda.sh` and then `conda activate`
4. Test intallation with `psi4 --test`
5. Python is also installed in this conda environment. This can be checked with `which python` which prints the location of the python executable in the current environment. You can now import psi4 in python: Run `python` then type `import psi4`. This should execute without errors. Pip is also installed (check with `which pip`).

export QDFT_DIR=`pwd`

pip install -e .

# execution

cd examples

python3 DFT_Hchain.py

python3 QDFT_Hchain.py

python3 QDFT_Hubbard.py



For Hubbard, one requires to clone and install git@github.com:bsenjean/SOFT.git
