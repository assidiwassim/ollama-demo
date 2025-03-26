# Ollama & Open WebUI Demo Project

This project sets up an environment with two services: **Ollama** and **Open WebUI**. The setup uses Docker Compose to easily spin up and manage the containers.

## Prerequisites

Before running this project, ensure that you have the following installed on your machine:

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Steps to Run the Project

Follow these steps to clone the repository and run the project using Docker:

### 1. Clone the Repository

Clone this repository to your local machine using the following command:

``bash
git clone https://github.com/assidiwassim/ollama-demo.git

### 2. Navigate to the Project Directory
Change into the project directory:

``bash
cd ollama-demo

### 3. Start the Docker Containers
Use Docker Compose to start the services defined in the docker-compose.yml file. The -d flag will run the containers in detached mode:

``bash
docker compose up -d

### 4. Verify the Containers are Running
To verify that the containers are up and running, use the following command:

``bash
docker ps

### 5. Access the Services
To verify that the containers are up and running, use the following command:

- The Ollama API is available at http://localhost:11434.

- The Open WebUI is available at http://localhost:8080.


### 6. Stop the Containers
If you want to stop the running containers, use the following command:

``bash
docker compose down

