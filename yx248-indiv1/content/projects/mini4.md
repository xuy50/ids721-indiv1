+++
title = "mini-projecct 4"
description = "https://gitlab.com/dukeaiml/IDS721/yx248-mini4"
+++

# Mini-Project: Containerize a Rust Actix Web Service

This project involves creating a container for a simple Rust Actix web application. The goal is to understand the basics of containerization and how to deploy a Rust-based web service using Docker.

## Requirements

- **Containerize a simple Rust Actix web app:** The core of this project is to take a basic web service written in Rust using the Actix framework and containerize it. This involves creating a suitable environment within a container where the web app can run independently of the host system's configuration.
- **Build Docker image:** You'll need to create a Dockerfile that specifies how to build the Docker image for the Rust Actix web app. This includes setting up the Rust environment, copying the necessary code into the image, and compiling the app within the container.
- **Run container locally:** After building the Docker image, you should be able to run the container on your local machine. This step verifies that the containerization process was successful and that the web service is accessible.

## Deliverables

1. **Dockerfile:** Submit the Dockerfile used to build the image of your Rust Actix web app. The Dockerfile should include comments explaining each step of the build process.
2. **Screenshots or demo video showing container running:** Provide visual evidence that your containerized app is running successfully. This could be in the form of screenshots showing the app responding to requests or a short video demonstrating the functionality of the web service within the container.
3. **Writeup of process:** Accompany your submission with a detailed writeup of the process you followed. This should include any challenges you faced while containerizing the Rust Actix web app, how you resolved them, and any insights or lessons learned from the project.
