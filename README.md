# Docker For Dev (React)


## Building the Docker Image

To build the Docker image for your React application, use the following command:

```bash

docker-compose -f .docker/docker-compose.yml build
```

This command reads the configurations from the specified docker-compose.yml file and builds the Docker image according to the defined services.

## Running the Docker Containers
**Option 1: Run Containers in the Foreground**

To start the containers and run them in the foreground (showing logs in the terminal), use:

```bash
docker-compose -f .docker/docker-compose.yml up
```

This command will launch the services defined in your docker-compose.yml file, and you'll see the output logs in the terminal.


**Option 2: Run Containers in the Background**

To start the containers and run them in the background, use the following command:

```bash
docker-compose -f .docker/docker-compose.yml up -d
```

The -d flag detaches the containers, allowing you to continue using the terminal while the services run in the background.

**Option 3: Rebuild and Run Containers in the Background**

If you've made changes to your code or dependencies and want to rebuild the Docker image before starting the containers, use the following command:

```bash
docker-compose -f .docker/docker-compose.yml up -d --build
```

This command not only starts the containers in the background but also triggers a rebuild of the Docker image before launching the services.

## React Application Documentation

For detailed information about the React application, project structure, and specific development instructions, please refer to the [React README](docs/README.md) file.

Feel free to add more details or customize the documentation based on your specific project structure and requirements. Additionally, you may want to include information on how to access the React application in a web browser and any other relevant details for your development environment.
