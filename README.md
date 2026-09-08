This project is intended to be run in docker. A Dockerfile is available in the deeplearning demonstrations folder. it was used to build a docker image called tensorflow-learn by running 

sudo docker build -t tensorflow-learn .

in the directory containing the Dockerfile.

The plan is to bind mount the Deep-Learning-Demonstrations into the container with the environment and use jupyter lab from there.

Given this folder is completely local nothing happens to it if we rebuild the image or container in docker. Git can be used from the host directly, so the container needs no Github token.


sudo docker run --rm -it \
    --gpus all \
    -p 8888:8888 \
    --mount type=bind,source=/home/sylvia/_Learn/TensorFlow_Learn/Deep-Learning-Demonstrations,target=/workspace \
    tensorflow-learn