# The Saas housekeeper Containers Library

## Get an image

The recommended way to get any of the saasHousekeeper Images is to pull the prebuilt image from the [Docker Hub Registry](https://hub.docker.com/u/saashousekeeper).

```console
docker pull saashousekeeper/APP
```

To use a specific version, you can pull a versioned tag.

```console
docker pull saashousekeeper/APP:[TAG]
```

If you wish, you can also build the image yourself by cloning the repository, changing to the directory containing the Dockerfile and executing the `docker build` command.

```console
git clone https://github.com/saashousekeeper/containers.git
cd saashousekeeper/APP/VERSION/OPERATING-SYSTEM
docker build -t saashousekeeper/APP .
```

> Remember to replace the `APP`, `VERSION` and `OPERATING-SYSTEM` placeholders in the example command above with the correct values.

## Run the application using Docker Compose

The main folder of each application contains a functional `docker-compose.yml` file. Run the application using it as shown below:

```console
curl -sSL https://raw.githubusercontent.com/saashousekeeper/containers/main/saashousekeeper/APP/docker-compose.yml > docker-compose.yml
docker-compose up -d
```

> Remember to replace the `APP` placeholder in the example command above with the correct value.




