# Explain

`Explain` is a Docker image that provides ChatGPT explanation for Linux terminal commands.

## Table of contents

- [Usage](#usage)

## Usage
- You must have an openai api key, which you can get from [this site](https://platform.openai.com/account/api-keys).
- Get the docker image from [Dockerhub](https://hub.docker.com/r/adrancarnavale/explain) (ensure you get the one tagged as `latest`)
- Run is as follows:

```bash
docker run -e PROMPT="YOUR_PROMPT" -e API_KEY="YOUR_API_KEY" adrancarnavale/explain:latest
```

- your prompt is made of one or more Linux terminal commands, which you must provide sepparated only by a white space.
- your API key is the one which you retrieved from the site indicated above

## Example of usage

```bash
docker run -e PROMPT="lsof sudo grep" -e API_KEY="sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx" adrancarnavale/explain:latest
```