[GitHub]: https://github.com/TemplesOfSyrinx/dkr-CircularGallifreyan
[GitHub_Tags]: https://github.com/TemplesOfSyrinx/dkr-CircularGallifreyan/tags
[GitHub_Issues]: https://github.com/TemplesOfSyrinx/dkr-CircularGallifreyan/issues
[GitHub_Forks]: https://github.com/TemplesOfSyrinx/dkr-CircularGallifreyan/network
[DockerHub]: https://hub.docker.com/r/templesofsyrinx/dkr-circulargallifreyan
[DockerHub_Builds]: https://hub.docker.com/r/templesofsyrinx/dkr-circulargallifreyan/builds
# dkr-CircularGallifreyan

| [GitHub] | [DockerHub] |
| -------- | ----------- |
| [![GitHub tags](https://img.shields.io/github/tag/TemplesOfSyrinx/dkr-CircularGallifreyan.svg "GitHub tag")][GitHub_Tags]| [![Docker build](https://img.shields.io/docker/automated/templesofsyrinx/dkr-circulargallifreyan.svg "Docker build")][DockerHub_Builds]
| [![GitHub issues](https://img.shields.io/github/issues/TemplesOfSyrinx/dkr-CircularGallifreyan.svg "GitHub issues")][GitHub_Issues]| [![Docker stars](https://img.shields.io/docker/stars/templesofsyrinx/dkr-circulargallifreyan.svg "Docker stars")][DockerHub]
| [![GitHub forks](https://img.shields.io/github/forks/TemplesOfSyrinx/dkr-CircularGallifreyan.svg "GitHub forks")][GitHub_Forks]| [![Docker pulls](https://img.shields.io/docker/pulls/templesofsyrinx/dkr-circulargallifreyan.svg "Docker pulls")][DockerHub]

Dockerfile containing Gallifreyan java app
 - Run Gallifreyan in docker. 
 - Use x11docker to run image to be able to run GUI application from within docker image. 
 - Get [x11docker and x11docker-gui from github](https://github.com/mviereck/x11docker)

# Example command: 
 ```
 x11docker templesofsyrinx/dkr-circulargallifreyan:{Version}
 ```

# Without container isolation:
 ```
 docker run --rm \
    --env DISPLAY=unix$DISPLAY \
    --volume /tmp/.X11-unix:/tmp/.X11-unix \
    templesofsyrinx/dkr-circulargallifreyan:{Version}
 ```
