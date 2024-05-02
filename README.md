# Rask Service

## Description

## Technology Stack

- Language: Python
- Framework: FastAPI
- Database: DynamoDB
- Other Technologies: Redis, SQS, RabbitMQ

## Installation and Setup

### Prerequisites

- Required software and tools, such as Python, Docker

### Running Locally

1. Clone the repository:
   ```bash
   git clone [Repository URL]
   ```

2. Specify the path to your id_rsa (path may vary):

   - For *nix systems:
     ```shell
     export DOCKER_BUILDKIT=1
     export SSH_PRIVATE_KEY_PATH=~/.ssh/id_rsa
     ```
   - For Windows:
     ```shell
     set DOCKER_BUILDKIT=1
     set SSH_PRIVATE_KEY_PATH=C:/Users/<username>/.ssh/id_rsa
     ```

3. Run app by docker-compose

    ```bash
    docker-compose -f docker-compose.yaml -f docker-compose.override.yaml up --build -d  # build and start up the whole application
    docker compose logs -f  # view logs in interactive mode
    docker compose down  # turn off application
    ```


### Run Services

## Testing

To run tests locally:

```bash
poetry run pytest tests
```

## Deployment

Please use `rask-deploy` for deployment