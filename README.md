# Selenium Grid Docker Setup

This repository provides a setup for running Selenium Grid with Docker, including Selenium Hub and multiple browser nodes for automated testing.

## Files Included

- `docker-compose.yml`: Configures the Selenium Hub and browser nodes.
- `Dockerfile.chrome`: Defines the Chrome Node image.
- `Dockerfile.edge`: Defines the Edge Node image.
- `Dockerfile.firefox`: Defines the Firefox Node image.

## Getting Started

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/your-repo.git
    cd your-repo
    ```

2. Build the Docker images for Selenium Hub and browser nodes:

    ```bash
    docker build -t your-selenium-chrome -f Dockerfile.chrome .
    docker build -t your-selenium-edge -f Dockerfile.edge .
    docker build -t your-selenium-firefox -f Dockerfile.firefox .
    ```

3. Use Docker Compose to start the Selenium Grid:

    ```bash
    docker-compose up
    ```

    This will start the Selenium Hub and all specified nodes, exposing the Selenium Grid on port 4444.

4. Open your browser and go to `http://localhost:4444` to access the Selenium Grid console.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
