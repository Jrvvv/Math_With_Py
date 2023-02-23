***Projects settings***

All needed libs are in math-env.yml
Check your enviroment is math-env before work

1) To create new enviroment:

    conda env create -f math-env.yml

2) To load new libs in existing enviroment:

    conda env update -f math-env.yml --prune

3) To configure Jupyter to use the conda environment as kernel:

    ipython kernel install --user --name=math-env-kernel

For authors

1) To add last enviroment configuration in math-env.yml:
    conda env export > math-env.yml