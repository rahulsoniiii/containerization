# Docker Project

In this project, I used Docker to containerize a multi-tier web app. The app consists of a web server, a database, and a cache server. I also created a Dockerfile that can be used to build the container images for each tier.


## Prerequisites

Before getting started, ensure that the following dependencies are installed on your system:

- Docker: [Installation Guide](https://docs.docker.com/get-docker/)
- Docker Compose: [Installation Guide](https://docs.docker.com/compose/install/)

## Usage

### Step 1: Clone the repository

First, clone this repository to your local machine:

```bash
git clone https://github.com/rahulsoniiii/containerization.git
cd containerization
```

### Step 2: Execute Docker Compose file

To execute the Docker Compose file, run the following command:

```bash
docker-compose up
```

This command will build the necessary Docker images and start the containers defined in the `docker-compose.yml` file.

### Step 3: Execute the production Docker Compose file 

```bash
docker-compose -f docker-compose.prod.yml up
```

The `-f` flag is used to specify the path to the Docker Compose file.

## Additional Information

For more details on Docker and Docker Compose, refer to the official documentation:

- Docker Documentation: [https://docs.docker.com/](https://docs.docker.com/)
- Docker Compose Documentation: [https://docs.docker.com/compose/](https://docs.docker.com/compose/)

## Contributing

If you'd like to contribute to this project, please follow these steps:

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Commit your changes
5. Push to the branch
6. Open a pull request

## License

This project is licensed under the [MIT License](LICENSE).