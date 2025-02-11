# AWS Buildkite Ubuntu Agent
This repository contains a Docker image for a Buildkite Agent based on Ubuntu, specifically designed to support AWS deployments.

## Docker Hub Image
You can pull the image from Docker Hub with the following command:

```sh
docker pull hasithaishere/aws-buildkite-ubuntu-agent:latest
```

## Docker Image Push
If you wish to push the image to Docker Hub, you can use the following command:

``` sh
./build.sh
```

## GitHub Repository
Clone this repository using the following command:

``` sh
git clone git@github.com:hasithaishere/aws-buildkite-ubuntu-agent.git
```

## Usage
### Build the Docker image locally
To build the Docker image locally from this repository, you can use the following command:

``` sh
docker build -t aws-buildkite-ubuntu-agent .
```
## Running the Container
To run the Buildkite Agent container locally, use the following command:

``` sh
docker run -d -t --name buildkite-agent aws-buildkite-ubuntu-agent:latest start --token "<REPLACE-FROM-YOUR-TOKEN>"
```

Make sure you replace the image tag with the appropriate version if needed. Also add 

## Custom Configuration
You can add environment variables or bind mount volumes for custom configuration depending on your needs.

## Contributing
If you’d like to contribute to this project, feel free to open a pull request. If you encounter any issues, please file an issue on the GitHub repository.

## License
This project is licensed under the MIT License.
