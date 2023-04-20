# Reference Algorithm Container for LDCTIQAC2023

This docker image contains a reference implementation that serve as a template for you to implementat your own algorithm for submission at LDCTIQAC2023

## Content:
1.Prerequisites

2.An overview of the structure of this example

3.Packing algorithm into a docker container image

4.Buliding container

5.Testing container and gernerating the bundle for uploading your algorithm

6.Creating an algorithm on Grand Challenge and submitting the solution to LDCTIQAC2023 Challenge

## 1.Prerequisites
- Install Docker, [Docker Installation](https://www.docker.com/get-started/)
- Clone this repository:
```bash
git clone https://github.com/JoyceWLee/LDCTIQAG_reference_docker.git
```
-  Install evalutils (provided by grand-challenge):
```bash
pip install evalutils
```
## 2.An overview of the structure of this example
## 3.Packing algorithm into a docker container image
## 4.Buliding container
- To test if all dependencies are met, you should run the `build.sh` to build the docker container. 
## 5.Testing container and gernerating the bundle for uploading your algorithm
- To test your container, you can run `test.sh`. This will run the test image provided in the test folder though your model. It will check them against what you provide in `test/expexted_output.json`. Noted: this will initially not be equal to the demo detections in this reference.
- To gerneate the bundle, you need to run the `export.sh` to generate the package of your docker with the extension **tar.gz**, which you can then upload to grand challenge to submit your algorithm.
## 6.Creating an algorithm on Grand Challenge and submitting the solution to LDCTIQAC2023 Challenge
- In order to submit the docker container, you have to add an algorithm for you docker container, [add algorithm](https://ldctiqac2023.grand-challenge.org/evaluation/challenge/algorithms/create/).
- Enter the name and description of the algorithm, and save the algorithm.
- After saving, you can add the docker container by uploading the container and waiting until the container becomes **active**.
- You can submit your docker container to LDCTIQAC2023 Challenge: [here](https://ldctiqac2023.grand-challenge.org/evaluation/challenge/submissions/create/).

