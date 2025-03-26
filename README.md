# Ollama AI Models & Open WebUI: Docker Setup for Seamless Model Management

This project sets up an AI-powered environment using **Ollama** and **Open WebUI**. The setup leverages Docker Compose to easily deploy and manage the containers.

## Overview

### What is Ollama?

[Ollama](https://ollama.com) is a lightweight and efficient framework for running AI models locally. It provides a simple API to interact with large language models (LLMs) without requiring extensive hardware or cloud-based services. With **Ollama**, you can run various AI models like **LLaMA, Mistral, Gemma, and TinyLLaMA** on your machine.

### What is Open WebUI?

[Open WebUI](https://github.com/open-webui/open-webui) is a user-friendly web-based interface for managing AI models running in Ollama. It allows you to:
- Load and interact with different AI models.
- Perform real-time text generation and inference.
- Manage multiple models seamlessly.
- Run AI-powered applications in a browser.


## Prerequisites

Before running this project, ensure that you have the following installed on your machine:

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Steps to Run the Project

Follow these steps to clone the repository and run the project using Docker:

### 1. Clone the Repository

Clone this repository to your local machine using the following command:

```bash
git clone https://github.com/assidiwassim/ollama-webui-demo.git
```

### 2. Navigate to the Project Directory
Change into the project directory:

```bash
cd ollama-webui-demo
```

### 3. Start the Docker Containers
Use Docker Compose to start the services defined in the docker-compose.yml file. The -d flag will run the containers in detached mode:

```bash
docker compose up -d
```

### 4. Verify the Containers are Running
To verify that the containers are up and running, use the following command:

```bash
docker ps
```

### 5. Access the Services
To verify that the containers are up and running, use the following command:

- The Ollama API is available at http://localhost:11434.

- The Open WebUI is available at http://localhost:8080.


### 6. Stop the Containers
If you want to stop the running containers, use the following command:

```bash
docker compose down
```

### Add More Models to Ollama
You can add additional models to the Ollama service by using the following commands. These commands will download the models inside the running Ollama container:

```bash
docker exec -it ollama ollama pull llama3:8b   
docker exec -it ollama ollama pull mistral:7b  
docker exec -it ollama ollama pull gemma:2b    
docker exec -it ollama ollama pull tinyllama:1.1b   
```

### Troubleshooting
If you encounter issues with the containers not starting, check the logs with:


```bash
docker logs <container_name>

```


