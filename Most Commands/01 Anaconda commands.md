Anaconda commands

| Command                        | Syntax                                        | Usage (Brief Explanation)                                         |
| ------------------------------ | --------------------------------------------- | ----------------------------------------------------------------- |
| Check Conda Version            | `conda --version`                             | Displays the installed Conda version.                             |
| Update Conda                   | `conda update conda`                          | Updates Conda to the latest version.                              |
| Check Conda Info               | `conda info`                                  | Shows information about Conda installation and environment paths. |
| List Environments              | `conda env list` or `conda info --envs`       | Displays all available Conda environments.                        |
| Create Environment             | `conda create --name env_name`                | Creates a new environment with the specified name.                |
| Create Environment with Python | `conda create --name env_name python=3.x`     | Creates an environment with a specific Python version.            |
| Activate Environment           | `conda activate env_name`                     | Activates the selected environment.                               |
| Deactivate Environment         | `conda deactivate`                            | Deactivates the currently active environment.                     |
| Remove Environment             | `conda remove --name env_name --all`          | Deletes an entire environment.                                    |
| List Installed Packages        | `conda list`                                  | Shows all installed packages in the current environment.          |
| Search Package                 | `conda search package_name`                   | Searches for a package in Conda repositories.                     |
| Install Package                | `conda install package_name`                  | Installs a package in the active environment.                     |
| Install Specific Version       | `conda install package_name=version`          | Installs a particular version of a package.                       |
| Update Package                 | `conda update package_name`                   | Updates the specified package.                                    |
| Update All Packages            | `conda update --all`                          | Updates all packages in the environment.                          |
| Remove Package                 | `conda remove package_name`                   | Uninstalls a package from the environment.                        |
| Export Environment             | `conda env export > environment.yml`          | Exports environment configuration to a YAML file.                 |
| Create Environment from File   | `conda env create -f environment.yml`         | Creates an environment using a YAML file.                         |
| Clone Environment              | `conda create --name new_env --clone old_env` | Copies an existing environment into a new one.                    |
| Clean Cache                    | `conda clean --all`                           | Removes unused packages and caches to free space.                 |
| Show Package Info              | `conda info package_name`                     | Displays details about a specific package.                        |
