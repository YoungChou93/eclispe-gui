# eclispe-gui
eclipse gui docker image

## VNC

### docker pull alanzhou/eclipse-vnc
### docker run -d -p 5905:5900 alanzhou/eclipse-vnc


volume workspace
### docker run -d -p 5905:5900 -v "your path":/usr/local/workspace alanzhou/eclipse-vnc


## LOCAL

### docker pull alanzhou/eclipse-local
### docker run -it --rm  -e DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix eclipse-local


volume workspace
### docker run -it --rm  -e DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix -v "your path":/home/developer/workspace eclipse-local
