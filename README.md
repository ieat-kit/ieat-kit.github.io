# Initiative Ethical Academic Ties at KIT - Website

Website for the Initiative Ethical Academic Ties at KIT.

## Development and Content Maintenance Guide

> [!NOTE]  
> This is still a work in progress.

This website is built using [MkDocs](https://www.mkdocs.org/) with the theme [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

MkDocs is a popular static website generator written in Python, mostly used for documentation, and Material for MkDocs is a popular theme for this framework.

### Running the website locally

The easiest way to run the website locally is by using a container environment with support to Docker Compose (e.g. Docker Desktop, Podman Desktop).

In such an environment, clone this repository, navigate to the root of the repository on your terminal and run the following command:

```
docker compose up
```

Once the container image is downloaded and the container is running, you will be able to access the website on the url <http://localhost:8000>, and do modifications.

### Updating the website content

The theme customization and the content structure (also known as _navigation_) is maintained on the file `mkdocs.yml`. The content of the webpages presented on the website are maintained in the different Markdown (`.md`) files under the `docs` folder.

### Deployment of the website

The website is deployed automatically, using GitHub Actions, once new commits are made to the `main` branch of this repository.
