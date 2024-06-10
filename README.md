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