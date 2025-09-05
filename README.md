# Docker_Compose

This repository demonstrates how to use Docker Compose to containerize and orchestrate a basic Node.js application with a database. It serves as a practical example for setting up a multi-container Docker environment for development purposes.

## Features

- **Node.js Backend**: Core application logic written in JavaScript.
- **Database Integration**: Connects to an external database (see `db.js` for connection logic).
- **Multi-Container Setup**: Utilizes `docker-compose.yml` to run the backend and database as separate services.
- **Simple Configuration**: Easy to start and stop the entire stack with one command.
- **Sample Dockerfile**: Custom Node.js Docker image setup.

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/)
- Optional: Node.js (for local development)

### Installation

Please refer to [Installation.md](./Installation.md) for detailed setup instructions.

### Quick Start

1. Clone the repository:

    ```bash
    git clone https://github.com/doomerdpk-1802/Docker_Compose.git
    cd Docker_Compose
    ```

2. Start the services using Docker Compose:

    ```bash
    docker-compose up
    ```

3. Access your application as instructed in the logs or configuration.

4. To stop and remove the containers:

    ```bash
    docker-compose down
    ```

## Project Structure

- `index.js`: Main application entry point.
- `db.js`: Database connection logic.
- `Dockerfile`: Instructions to build the Node.js app image.
- `docker-compose.yml`: Multi-container orchestration file.
- `.dockerignore`, `.gitignore`: Ignore patterns for Docker and Git.
- `package.json`, `package-lock.json`: Node.js dependencies.
