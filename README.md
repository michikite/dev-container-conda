# VSCode dev-container (Docker) setup with Miniconda and Jupyter Notebooks

This is a [**containerized dev setup**](https://code.visualstudio.com/docs/remote/containers) to work on machine learning problems using **Anaconda with VSCode**.

It installs [`conda/miniconda3:latest`](https://hub.docker.com/r/conda/miniconda3/) as a base image and installs ipykernel,
so it supports Jupyter notebooks (installed as a VSCode extension), as well as debugging *.py files directly.

A conda environment is created within the dev container and can easily be configured with the desired dependencies/packages.
Various VSCode extensions are installed automatically in the container as well.

Mac OS Install Instructions:

- Install Docker Desktop `brew install --cask docker`
- Install VSCode `brew install --cask visual-studio-code`
- Open VSCode
- Install VSCode remote container extension: [ms-vscode-remote.remote-containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- Start dev container:  F1 + "Open folder in container ..." 
- Open demo.ipynb or demo.py to try the setup


Optional Steps:

- Add/remove VSCode extensions in .devcontainer/devcontainer.json
- Change Anaconda environment in .devcontainer/environment.yml
- Update gitignore to match your setup