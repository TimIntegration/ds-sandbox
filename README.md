boilerplate to bootstrap a development container for a data science project

# Setup in vscode
- reopen in container
- open the terminal and run the following command
```bash
conda init
```

- if using a jupyter notebook, then Select Kernel: Python Environment in `/opt/conda/bin/python`
- if using .env file, then add .gitignore file using the following command
```bash
echo ".devcontainer/.env" >> .gitignore
```

## Two possible errors in vscode:
- if error regarding conda-libmamba-solver, then use command to copy file
`cp /opt/conda/lib/libarchive.so /opt/conda/lib/libarchive.so.19`

- if vscode detect the wrong version of python, python3.1 then rename the shortcut
`mv /opt/conda/bin/python3.1 /opt/conda/bin/python3.12.2`

- stick with conda (base) environment, create different containers for different projects. May need to clear cache in vscode, `Python: clear cache and restart`