# Setting up M1 for TensorFlow

## Install Conda

```
wget https://github.com/conda-forge/miniforge/releases/download/4.12.0-2/Mambaforge-4.12.0-2-MacOSX-arm64.sh
chmod +x Mambaforge-4.12.0-2-MacOSX-arm64.sh
./Mambaforge-4.12.0-2-MacOSX-arm64.s
```

## Install Python Dependencies

```shell
# Create an environment for TensorFlow
conda create -y --name env_tensor_flow python=3.9
conda activate env_tensor_flow
```

```shell
# Install all the things
conda activate env_tensor_flow
conda install -c apple tensorflow-deps jupyter jupyterlab -y
python -m pip install -r extra-requirements.txt
python -m pip freeze > requirements.frozen.txt
```

ll
