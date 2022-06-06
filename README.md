# Raspberry Pi Config
This is the configuration that I use to run my local Raspberry Pi at home.

## The main goals of this project include:
1. Automate as much as possible.
	* This is to ensure that I can recreate my setup with minimal effort.
	* This is achieved by the docker-compose.yml file and running all functionality via Docker containers.
1. Keep a history of all changes.
1. Provide others with examples of how they can recreate a similar setup.

## Running this setup
### Environment Variables
To assist in configuring the environment easily, all configuration for the docker-compose.yml file are set via environment variables. Copy the an `.env.example` file and rename it to `.env` and then fill out each line with the necessary values.

## The main functionality that this configuration contains
### Automatic Config Reload on Push
TBD

### Cloudflare Dynamic DNS
Docker Image: [oznu/cloudflare-ddns](https://hub.docker.com/r/oznu/cloudflare-ddns/)

Exposes the Pi to the internet on my own domain to allow it to react to new pushes to this repository.
