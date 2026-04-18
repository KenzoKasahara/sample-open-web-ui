# sample-open-web-ui

This project runs both Ollama and Open WebUI as Docker containers using Docker Compose. You can easily set up a local LLM environment with a web interface.

## Setup

1. Create required directories for persistent data.

    ```sh
    mkdir -p data/ollama data/open-webui
    ```

2. Start the containers.

    ```sh
    docker-compose up -d
    ```

3. Install "LLM: gemma4:e4b" in the docker container.

    ```sh
    docker exec ollama ollama pull gemma4:e4b
    ```

4. Access to [http://localhost:3000/](http://localhost:3000/)

5. Sign up for an admin account.

## License / Usage

This project itself imposes no special restrictions on use, modification, or redistribution. Please note that the included software (Ollama, Open WebUI, and any models) may have their own licenses or terms of use—refer to their official documentation for details.
