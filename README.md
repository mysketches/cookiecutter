# Cookiecutter Langgraph project template

## Description
This repository is meant to help you bootstrap your Langgraph project. Once the structure of your project is pulled by cookiecutter, don't forget to set the environment variables in the .env file

## Quickstart

Install the latest version of CookieCutter:

```commandline
pip install -U cookiecutter
```

Generate your new Langgraph project:

```commandline
python -m cookiecutter https://github.com/mysketches/cookiecutter-langgraph.git
```

or
```commandline
cookiecutter https://github.com/mysketches/cookiecutter-langgraph.git
```

Build your Docker image
```commandline
docker build -t langgraph .
```

Build your Docker image
```commandline
docker run --rm -p 2024:2024 -p 8501:8501 -v <personal_folder>:/home/project --name langgraph-project langgraph
```