# Docker Open Broadcaster Software (OBS 28)
Repo is forked from bandi13's obs docker [repo](https://github.com/bandi13/docker-obs). Using OBS 28.0.3

This container is based on [nkostic/ubuntu-gui-docker](https://github.com/nkostic/ubuntu-gui-docker). The OBS is incorporated into the container and can be used to stream your desktop.

Here is a screenshot:
![Alt](https://raw.githubusercontent.com/bandi13/docker-obs/master/screenshot.png "Example screenshot")

# To run
You can start the container with:

`docker run --shm-size=256m -it -p 5901:5901 -e VNC_PASSWD=123456 nkostic/ubuntu-docker-obs`

The shm-size argument is to make sure that the webclient does not run out of shared memory and crash. You can change the default VNC password of '123456' on the docker run command to whatever you wish.
