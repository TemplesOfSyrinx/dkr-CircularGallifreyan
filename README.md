# dkr-CircularGallifreyan

Dockerfile containing Gallifreyan java app
 - Run Gallifreyan in docker. 
 - Use x11docker to run image to be able to run GUI application from within docker image. 
 - Get [x11docker and x11docker-gui from github](https://github.com/mviereck/x11docker)

# Example commands: 
 - `x11docker templesofsyrinx/dkr-circulargallifreyan`

# Without container isolation:
 - `docker run --rm \
       --env DISPLAY=unix$DISPLAY \
       --volume /tmp/.X11-unix:/tmp/.X11-unix \
       templesofsyrinx/dkr-circulargallifreyan`

