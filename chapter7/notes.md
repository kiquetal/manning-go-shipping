#### Containerized deployment

- Building a standarized way of deploying applications across multiple machines
- Using Buildpacks to build optimized containers for hosted infraestructure.
- Customizing a deployment using a Dockerfile
- Deploying containers to hosted environments
- Organizing containers for local development.

### Buildpack

It uses two phaes: detection and build phase.
For the detection phase, will recognize the code used, and then will trigger the build phase, to create
a container optimized for the runtime and hardware.


### Writing your own image

Creating image , usage of --target for a specific FROM line

docker build -t hello-api:min --target prod .

