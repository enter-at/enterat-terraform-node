# terraform-node

A Docker container that includes Terraform and node.js.
Functions identically to the official Terraform container.

Pre-built containers are available on Dockerhub:
https://hub.docker.com/r/enterat/terraform-node

## Versioning
Container versions are as follows:

```
<tf-version>-<revision>
```

So for example, `0.12.9-1` would be the first container revision with Terraform 0.12.9.

## Building for Dockerhub

```
# Build the container
$ docker build . -t enterat/terraform-node:<tf-version>-<revision>

# Push to Dockerhub
$ docker push enterat/terraform-node:<tf-version>-<revision>

# Update 'latest' tag
$ docker tag enterat/terraform-node:<tf-version><revision> enterat/terraform-node:latest
$ docker push enterat/terraform-node:latest
```
