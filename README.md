***Projects settings***

All needed libs are in math-env.yml
Check your enviroment is math-env before work

1) To create new enviroment:

    conda env create -f math-env.yml

2) To load libs from .yml in existing enviroment:

    conda env update -f math-env.yml --prune

3) To configure Jupyter to use the conda environment as kernel (in new env!!!):

    ipython kernel install --user --name=math-env-kernel

***For authors***

1) To add last enviroment configuration in math-env.yml:

    conda env export > math-env.yml

***Install Jupyter***

To install Jupyter run jupyter from the system installation or a different conda environment:

    1) conda install ipykernel                                    # install Python kernel in new conda env
    2) ipython kernel install --user --name=base-env-kernel       # configure Jupyter to use Python kernel
    3) conda install jupyter                                      # might be installed already in system 'apt install jupyter'

You can add kernel for new enviroments this way (without install) after commands:

    1)conda create -n env-name
    2)conda activate env-name