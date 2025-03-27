# Initiative Ethical Academic Ties at KIT - Website

Website for the Initiative Ethical Academic Ties at KIT.

## Development and Content Maintenance Guide

This website is built using [MkDocs](https://www.mkdocs.org/) with the theme [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

MkDocs is a popular static website generator written in Python, mostly used for documentation, and Material for MkDocs is a popular theme for this framework.

### Running the website locally

This section has a short set of instructions on how to run the website locally for testing and content maintenance.

In any of the options, close this git repository, navigate to the root of the repository on your terminal and execute the instructions the sub-heading that better represents your development environment.

#### With a container environment

The easiest way to run the website locally is by using a container environment with support to Docker Compose (e.g. Docker Desktop, Podman Desktop).

On a terminal on the root of the repository, run the following command:

```
docker compose up
```

Once the container image is downloaded and the container is running, you will be able to access the website on the url <http://localhost:8000>, and do modifications.

#### With a native Python 3 environment

If you have a working Python 3 environment, you can use this instructions.

To avoid conflict with your existing environment, the instructions make you of virtual environments. You can learn more about Python virtual environments at <https://docs.python.org/3/library/venv.html>.

On a terminal on the root of the repository, run the following commands:

1. `python3 -m venv .devenv`
2. On Windows Command Line (check <https://docs.python.org/3/library/venv.html#how-venvs-work> for instructions for other systems): `.devenv\Scripts\activate.bat`
3. `pip3 install mkdocs-material==9.5.33`
4. `mkdocs serve`

If everything went well, the page should be running locally and you will be able to access the website on the url <http://localhost:8000>, and do modifications.

### Updating the website content

The theme customization and the content structure (also known as _navigation_) is maintained on the file `mkdocs.yml`. The content of the webpages presented on the website are maintained in the different Markdown (`.md`) files under the `docs` folder.

### Deployment of the website

The website is deployed automatically, using GitHub Actions, once new commits are made to the `main` branch of this repository.
