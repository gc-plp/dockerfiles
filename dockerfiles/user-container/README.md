Ubuntu based container that creates the default user with the creator's UID, GID and username.

###### Build:
docker build --build-arg UID=$(id -u) --build-arg GID=$(id -g) --build-arg UNAME=$(echo $USER) -t <name> .

###### Run:
docker run -it --rm <container> /bin/bash
