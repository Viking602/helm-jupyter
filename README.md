# Helm-Jupyter

Deploy Jupyter via Helm

## Overview

- **Default Install Python Version**: 3.12

- **Default Password**: `jupyter`

- **Default Storage**: 50Gi

- **Default Jupyter Root Dir**: `/workspace`

- **Default venv Dir**: `/workspace/.venv`

- **Default Jupyter Config Dir**: `/workspace/.jupyter/.config`

- **Default Jupyter Data Dir**: `/workspace/.jupyter/.data`

- **Customize Python Version**: Edit `pythonVersion` in `values.yaml`

- **Customize Password**: Edit `password` in `values.yaml`

- **Environments**: Use `uv` to manage Python environments [docs](https://docs.astral.sh/uv/)


## Install

1. Clone the repository:

```bash
git clone https://github.com/Viking602/helm-jupyter.git
```

2. Navigate to the chart directory:

```bash
cd helm-jupyter/uv-jupyter
```

3. Install the Helm chart

```bash
helm install <release-name> -f values.yaml .
```

## Uninstall
```bash
helm uninstall <release-name>
```

