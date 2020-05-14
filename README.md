# Rpi-opencv-docker
Build image: 
Docker build -t cardetect .

Run container with video display:
docker run -ti --net=host --env="DISPLAY" --volume="$HOME/.Xauthority:/root/.Xauthority:rw" --privileged cardetect
