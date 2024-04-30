# Intended Sarcasm Detection


## Introduction
Sarcasm detection is crucial in natural language processing as it enhances the accuracy of sentiment analysis. Our objective is to refine the classification accuracy in identifying sarcastic sentences. We have experimented with various data augmentation techniques and prompt engineering strategies to train the Llama2-7b model for more effective sentence classification.


## How to run the code

The code is written in Jupyter notebooks. The pip installations for necessary packages are provided in the notebook itself. It is highly recommended to run the code in Google Colab as experimented.
In case you want to run the code locally, you can use the provided `requirements.txt` file to install the necessary packages. The instructions for both Conda and Pip + Virtualenv are provided below.


### Conda 

Conda uses the provided `requirements.txt` file.
Make sure you have [Miniconda](https://docs.conda.io/en/latest/miniconda.html) or [Anaconda](https://www.anaconda.com/products/individual) installed on your system.
Once installed, open up your terminal (or Anaconda prompt if you're on Windows).
Install the environment from the specified environment file:

    conda create --name intended-sarcasm-detection --file requirements.txt
    conda activate intended-sarcasm-detection

After you install, register the environment so jupyter can see it:

    python -m ipykernel install --user --name=intended-sarcasm-detection

You should now be able to launch jupyter and see your conda environment:

    jupyter-lab



### Pip + Virtualenv

An alternative to Conda is to use pip and virtualenv to manage your environments.
This may play less nicely with Windows, but works fine on Unix devices.
This method makes use of the `requirements.txt` file.

Ensure you have installed the [virtualenv tool](https://virtualenv.pypa.io/en/latest/installation.html) on your system.
Once installed, create a new virtual environment:

    vitualenv ~/sarcasm-venv
    source ~/sarcasm-venv/bin/activate

Install the packages from a requirements.txt file:

    pip install -r requirements.txt

As before, register the environment so jupyter can see it:

    python -m ipykernel install --user --name=sarcasm-venv

You should now be able to launch jupyter and see your conda environment:

    jupyter-lab

If you want to create a new `requirements.txt` file, you can use `pip freeze`:

    pip freeze > requirements.txt