# Selenium Grid Docker Setup

This repository provides a basic setup for running Selenium Grid with Docker, including a Selenium Hub and a Chrome Node for automated browser testing.

## Files Included

- `docker-compose.yml`: Configures the Selenium Hub and Chrome Node services.
- `Dockerfile.hub`: Defines the Selenium Hub image.
- `Dockerfile.node`: Defines the Chrome Node image.

## Getting Started

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/your-repo.git
    cd your-repo
    ```

2. Build the Docker images for Selenium Hub and Chrome Node:

    ```bash
    docker build -t your-selenium-hub -f Dockerfile.hub .
    docker build -t your-selenium-chrome -f Dockerfile.node .
    ```

3. Use Docker Compose to start the Selenium Grid:

    ```bash
    docker-compose up
    ```

    This command will launch both the Selenium Hub and Chrome Node, exposing the Selenium Grid on port 4444.

4. Open your browser and go to `http://localhost:4444` to access the Selenium Grid console.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
