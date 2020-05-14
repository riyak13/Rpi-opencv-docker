# Rpi-opencv-docker
Build image: 
Docker build -t cardetect .

Run container (in terminal):
comment out #cv2.imshow('video2', frames) from carDetection.py
Docker run cardetect:latest

Run container with video display:
cv2.imshow('video2', frames)
docker run -ti --net=host --env="DISPLAY" --volume="$HOME/.Xauthority:/root/.Xauthority:rw" --privileged cardetect
