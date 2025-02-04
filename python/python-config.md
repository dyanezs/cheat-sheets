# Python Config Commands Cheat Sheet

## Create a virtual environment
Commands to create a virtual environment and access it.

```bash
python -m venv <name-venv>
source ./name-venv/bin/activate
```

- The first is to crete the environment.
- The second to activate it.

## Use a venv inside Jupyter


```bash
python3 -m ipykernel install --name=<name-venv>
```

- You may need to install ipykernel.
- Once you execute this, you will be able to choose the environment in Jupyter.

If we need to uninstall the Kernel:
```bash
jupyter kernelspec uninstall <name-venv>
```

and then
```bash
jupyter kernelspec uninstall <name-venv>
```
