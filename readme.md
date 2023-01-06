<h2 align="center"><b> DevOps Repo </b></h2>

This repo contains templates for orchestrating pipelines & workflows, builds & releases using tools such as Docker, GitHub Actions, Azure DevOps Pipelines, Gitlab CI/CD - and any similar systems I come across in my work.

| **Script Store** | [Library](/docs/library/)
|--|--
| **Build** | [![build](https://github.com/DNYFZR/DevOps/actions/workflows/build.yml/badge.svg)](https://github.com/DNYFZR/DevOps/actions/workflows/build.yml)
| **Deployment** | [![pages-build-deployment](https://github.com/DNYFZR/DevOps/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/DNYFZR/DevOps/actions/workflows/pages/pages-build-deployment)

<br>

This project has been build using mkdocs & the mkdocs-material theme.

- The site is configured using the [mkdocs.yml](/mkdocs.yml)

- Site pages are managed via the [docs](/docs/) directory

- Build is managed via [GitHub Actions](https://github.com/DNYFZR/DevOps/actions)

<br>

Python has been used to create a development environment, and to install the mkdocs packages within it :

````ps1
# Set up & install
python -m venv <env_name>
cd <env_name>/scripts
./activate

python -m pip install -U pip
python -m pip install mkdocs mkdocs-material

# Setup project
cd ../../
mkdocs new <project_name>

# Launch mkdocs local server 
cd <project_name>
mkdocs serve

````
