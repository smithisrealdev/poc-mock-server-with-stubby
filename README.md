# POC Mock Server with Stubby

## Introduction
This repository provides a Proof of Concept (POC) for setting up a mock server using [Stubby](https://github.com/jsmartx/stubby4j) and Docker Compose. The purpose of this POC is to demonstrate how to configure and run a mock server in your local development environment.

## Prerequisites
Before running the mock server, please ensure that you have the following installed on your machine:
- Docker
- Docker Compose

## Installation and Setup
1. Clone the repository from GitHub:
   ```
   git clone https://github.com/your-username/poc-mock-server-with-stubby.git
   ```

2. Navigate to the repository directory:
   ```
   cd poc-mock-server-with-stubby
   ```

3. Build the Docker image:
   ```
   docker-compose build
   ```

## Usage
To start the mock server, use the following command:
```
docker-compose up -d
```

The server will now be accessible at `http://localhost:8882`. You can verify if the server is running by accessing this URL in your browser.

## Configuration
The mock server configuration is defined in the `stubby.yml` file located in the `config` directory. Modify this file according to your needs to define the desired response behavior for different API endpoints.

## Testing
To test the mock server, send requests to the defined API endpoints using tools like cURL or Postman. The responses returned by the mock server will mimic the behavior specified in the configuration file.

## Shutting Down the Mock Server
To stop the mock server, run the following command:
```
docker-compose down
```

## Conclusion
This POC demonstrates how to quickly set up a mock server using Stubby and Docker Compose. Feel free to explore and modify the configuration to simulate various scenarios in your local development environment.

## License
This project is licensed under the [MIT License](LICENSE).