# Setup instruction
This container could be used to parse bagfiles with out interfering with host OS ROS processes. Please, follow REDME.md for usage instruction.

- Setup docker in your machine follow: https://docs.docker.com/get-docker/ .
- In your terminal run `docker --version` should work now.
- clone this github repository.
- cd into the reposoitory:  `cd ROS-Noetic-Container` 
- to build image:  `docker build -t {your_unique_name} .`
- this will mount your present working directory to /src inside docker and take you to contaier command line:  `docker run -it -v "$(pwd)":/src <your_unique_name>  bash` 

- `rosbag --version`
- `python3 --version`
- `rosversion -d`