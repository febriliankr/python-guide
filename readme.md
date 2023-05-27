# Guide Python, Windows

- masuk ke C:\Users\[User]\anaconda3\envs
- klik kanan, open Git Bash
- conda create -n nama_project_atau_folder
- `cd nama_project_atau_folder`
- `code .` untuk membuka di vscode (code editor)
- [CTRL + `] untuk membuka terminal di vscode
- `conda activate nama_project_atau_folder` untuk mengaktifkan virtual environment python di terminal vscode
- sekarang, sudah bisa `pip install`, `python`, dan lain-lain

## Requirements

- Python https://www.python.org/downloads/windows/
- Git Bash https://git-scm.com/downloads
- Conda https://conda.io/projects/conda/en/latest/user-guide/install/windows.html

# Guide Python, MacOS

- I'm using miniforge now because it's more recommended: https://github.com/conda-forge/miniforge
- Conda tutorial: https://kirenz.github.io/codelabs/codelabs/miniforge-setup/#3
## Miniforge Conda
- conda create -n <PROJECT_NAME>
- conda activate
  - conda activate <PROJECT_NAME>
  - conda list
    - Now take a look at all the modules in your <PROJECT_NAME> environment
  - conda deactivate
  - conda install <PACKAGE_NAME>
    - alternative: pip install <PACKAGE_NAME>
- Installing
  - brew install miniforge
## Jupyter Notebook
  - 404 Loading forever bug https://stackoverflow.com/ques
  - conda install -c conda-forge nbstripout
  - nbstripout filename.ipynb.
    - Make sure that there is no whitespace in the filenam

## Installing Packages
pip3 install package_name
    - - Using with [[TensorFlow]]: https://github.com/adis

# Getting Started with Keras, Windows

This is a set of instructions on how to use Keras, from setting up the conda environment until getting results from python code with keras.

## How I setup the tensorflow environment

### Creating new environment with Anaconda (conda)

The complete documentation on how we could use conda is here https://docs.anaconda.com/anaconda/user-guide/tasks/tensorflow/

```
conda create -n <folder_name> tensorflow
```

cd into folder

```
conda activate <folder_name>
```

Install your dependencies (tensorflow, keras)

```
pip install tensorflow
pip install keras
```

### Using Jupyter Notebook as Text Editor

https://jupyter.org/install

If you use conda, you can install it with:

```
conda install -c conda-forge jupyterlab
```

If you use pip, you can install it with:

```
pip install jupyterlab
```

If installing using pip install --user, you must add the user-level bin directory to your PATH environment variable in order to launch jupyter lab. If you are using a Unix derivative (FreeBSD, GNU / Linux, OS X), you can achieve this by using export PATH="$HOME/.local/bin:$PATH" command.

Run jupyter lab with

```
jupyter-lab
```

## Use the Documentation

https://keras.io/getting_started/intro_to_keras_for_researchers/

Here are some python project examples:

- https://keras.io/examples/vision/image_classification_from_scratch/
- more on https://keras.io/examples/
