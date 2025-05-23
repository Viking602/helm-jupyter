# Helm-jupyter
Helm Install Jupyter

## Description

Default Python Version is 3.12

Default Password is "jupyter"

Change Python Version in values.yaml pythonVersion


## Install

```bash
1.
git clone https://github.com/Viking602/helm-jupyter.git
```
2.
```bash
cd helm-jupyter/uv-jupyter
```
3.
```bash
helm install <release-name> -f values.yaml .
```

## Uninstall
```bash
helm uninstall <release-name>
```
