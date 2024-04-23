# Odoo Docker Image Repository

This repository contains the Dockerfile and necessary scripts to build a Docker image for the Odoo ERP system.

## Workflow

The repository uses a GitHub Actions workflow to automatically build and push the Docker image to Docker Hub whenever there's a push to the `master` branch.

Here's what the workflow does:

1. Checks out the repository's code.
2. Logs in to Docker Hub using the provided Docker username and password (stored as secrets in the repository settings).
3. Builds and pushes the Docker image with the tag `username/Image_name:version`.

## Dockerfile

The Dockerfile in this repository is used to create an Odoo Docker image. It includes instructions to set up all the necessary dependencies and configuration needed to run Odoo.

## Usage

To use the Docker image, you can pull it from Docker Hub using the following command:

```bash
docker pull mwking0/odoo:latest
xx
