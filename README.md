# Research Topics Page

This project contains a simple web service running in Docker containers. It includes a `Dockerfile` for building an image and instructions for running two containers to demonstrate a basic web service setup.

## Project Overview

This repository contains the following components:
1. A web page to showcase research topics.
2. A Docker image named `research_topics_page` for serving the web content.
3. A Docker image `mrintania/assign2_image` for serving additional content.

## How to Run the Project

### Prerequisites

- Docker must be installed on your system.
- Ensure that you have an active internet connection to pull Docker images.

### 1. Build the Docker Image

To build the Docker image for the `research_topics_page`, run the following command in the root directory of the project:

```bash
sudo docker build -t research_topics_page .