+++
title = "Individual-projecct 1"
description = "https://gitlab.com/dukeaiml/IDS721/yx248-indiv1"
+++

[My Zola Web](https://yx248-indiv1-dukeaiml-ids721-0dbfac262998dd8f7067eb4b9326dbe700.gitlab.io/)

<br>

# Continuous Delivery of Personal Website

This project focuses on the creation and continuous delivery of a personal website. The website is built using Zola, a fast and efficient static site generator written in Rust. The goal is to automate the build and deployment process, allowing updates to be pushed live automatically with each commit to the main branch of the project's GitLab repository.


## Introduction

A personal website serves as a digital portfolio showcasing your work, skills, and professional identity. By leveraging Zola and continuous delivery principles, we can ensure that the website is always up-to-date with the latest content and changes.

### Why Zola?
- **Speed:** Zola generates pages at an incredibly fast rate, enhancing the development workflow.
- **Simplicity:** With Zola, you can manage your content without the overhead of databases or heavy frameworks.
- **Flexibility:** Zola supports Markdown for content creation, making it easier to write and maintain website content.


## Project Setup

### Requirements
- **Static Site Generator:** Zola
- **Source Control:** GitLab
- **Hosting:** Options include Vercel, Netlify, AWS Amplify, or AWS S3.

### Initial Setup
1. **Install Zola:** Follow the [official Zola installation guide](https://www.getzola.org/documentation/getting-started/installation/) to set up Zola on your local machine.
2. **Create a New Zola Site:** Run `zola init my_personal_website` to create a new site. Replace `my_personal_website` with your desired project name.
3. **Project Structure:** Customize the project structure by adding templates for the home page and portfolio project page. Ensure your site is styled using CSS for a polished look.


## Continuous Deployment

### GitLab Workflow
1. **Repository Setup:** Store the source code in a GitLab repo within the Duke GitLab organization. Ensure the repository is set up with the main branch as the default branch for deployments.
2. **GitLab CI/CD Configuration:**
   - Create a `.gitlab-ci.yml` file in the root of your repository.
   - Define a pipeline that installs Zola, builds the site, and deploys it to your hosting provider upon each push to the main branch.

Example `.gitlab-ci.yml` snippet for building with Zola:

```yml
image: "registry.gitlab.com/pages/zola:latest"

pages:
  script:
    - zola build
  artifacts:
    paths:
      - public
```


## Hosting Setup

- Vercel/Netlify/AWS: Follow the hosting provider's documentation to set up continuous deployment from your GitLab repository. This usually involves linking your GitLab account, selecting the repository, and configuring build commands and publish directories.


## Deliverables
- **Live Site**: Submit the URL of your live site. If hosting setup is pending, provide screenshots showing the site running locally.
- **GitLab Repository**: Link to the GitLab repository containing your project source code, including the `.gitlab-ci.yml` file demonstrating the continuous delivery setup.
