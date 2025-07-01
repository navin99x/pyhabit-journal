## Python Virtual Environment (venv)

`venv` provides isolated python environment, separate from global python installation.

1. Creating Virtual Environment

```bash
python -m venv <name>
```
> Standard venv names include: `venv`, `.venv`, `project-name-env`

2. Access global packages without reinstalling them

```bash
python -m venv --system-site-packages <name>
```

> This behaviour can be toggled through `pyvenv.cfg` file inside `venv`:
>
> ```bash
> include-system-site-packages = true/false
> ```
s
3. Activation

```bash
source <.venv>/bin/activate
```

4. Deactivation

```bash
deactivate
```

5. Delete virtual environment

```bash
rm -rf <.venv>