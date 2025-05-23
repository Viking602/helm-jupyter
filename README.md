# Helm-Jupyter

Deploy Jupyter via Helm

## Overview

- **Default Python Version**: 3.12

- **Default Password**: `jupyter`

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

