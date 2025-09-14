# Docker Essentials

▶ **Introduction**

This project demonstrates the basics of using Docker to containerize and run applications. It is designed to show how Docker can simplify development, deployment, and scaling of software by packaging everything needed to run an app into a single container.

▶ **Table of Contents**

- Overview[#overview]
- Concepts[#concepts]
- Example[#example]
- Installation[#installation]
- Author[#author]

▶ **Overview**

A simple example of running a Python web server inside a Docker container, making it easy to start, stop, and share your app anywhere Docker runs.


▶ **Concepts**

- **Docker containers**: Lightweight, standalone, and executable packages that include everything needed to run a piece of software, including code, runtime, system tools, and libraries.
- **Dockerfile**: A text file with instructions to build a Docker image, specifying the base image, dependencies, files to copy, and commands to run.
- **Port mapping**: The process of linking a port on the host machine to a port inside the Docker container, allowing external access to services running in the container.
- **Containerized web server**: A web server; like Flask or Nginx, runs inside a Docker container, isolated from the host system and easily portable.

▶ **Example**

```dockerfile
FROM python:3.10-slim
WORKDIR /app
COPY app.py .
RUN pip install flask
EXPOSE 5000
CMD ["python", "app.py"]
```

▶ Installation

Clone this repository in your terminal:

```bash
git clone https://github.com/kamisos3/holbertonschool-softy-pinko-docker.git
```

▶ Author

Kami Sostre [https://github.com/kamisos3]