To create a Docker container:

1. Create a new folder `CONTAINER-NAME`

1. Inside, create the `environment.yml` with all requirements and the `Dockerfile`

1. Authenticate to the container registry using Personal access Token: `docker login registry.git.embl.org`

1. Add an image to the registry: `docker build -t registry.git.embl.org/grp-mif/mif_resources/containers/CONTAINER-NAME .`

1. Push the image to the registry: `docker push registry.git.embl.org/grp-mif/mif_resources/containers/CONTAINER-NAME`

You should then be able to see the available containers at `Deploy/Container registry`.
