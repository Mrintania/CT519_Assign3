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
```

### 2. Run the Containers

2.1 Run Container for mrintania/assign2_image

This container will serve content on port 8080:

```
sudo docker run -d -p 8080:80 mrintania/assign2_image
```

•	Port 8080: This port on the host machine will be mapped to port 80 inside the mrintania/assign2_image container.

•	To view the content: Open your browser and go to http://localhost:8080.

2.2 Run Container for research_topics_page

This container will serve the research topics page on port 80:
```
sudo docker run -d -p 80:80 research_topics_page
```
•	Port 80: This port on the host machine will be mapped to port 80 inside the research_topics_page container.

•	To view the content: Open your browser and go to http://localhost:80.

### 3. Access the Web Pages

•	Research Topics Page: Open your browser and go to http://localhost:80.

•	Assign2 Image Content: Open your browser and go to http://localhost:8080.

You can navigate between these pages using the link provided on the Research Topics Page.