# ECE444-F2020-Lab3 (LAB-4&5 Experiment)

This repo is a clone of
https://github.com/miguelgrinberg/flasky

**Deliverable 1: (1 mark)**
All development has been performed in branch "lab4_Microservice_Experiment" in my Lab3 task GitHub repository 

**Deliverable 2: (6 mark)**
- README.md file (Done)
- To build the system: 
    - `docker build -t lab4:latest .`
- To start the system use either of the following commands (both work): 
    - `docker run -d -p 5000:5000 lab4`
    - `docker run -it --name lab4 --rm -p 5000:5000 lab4`
- Location of Docker files:
    - ./Dockerfile
    - ./requirements.txt
- SCREENSHOTS:

    - ![Screenshot1-4&5](Screenshot1-4&5.jpeg)

    - ![Screenshot2-4&5](Screenshot2-4&5.jpeg)

    - ![Screenshot3-4&5](Screenshot3-4&5.jpeg)

    - ![Screenshot4-4&5](Screenshot4-4&5.jpeg)


**Deliverable 3: (3 mark)**

- Briefly summarize the differences between Docker and Virtual Machine:

Virtual machines (VMs) emulate computer systems. They make it possible to run multiple OS on the same hardware making it seem like separate computers.

Unlike VMs Docker is a type of containers that sit on top of the host OS and the hardware making it possible to have better potability of projects and their dependencies. 

Following are some of the key differences:

VM <—> Docker:
1. Each VM has own OS <—> All the docker containers share single OS
2. Hardware is virtualized <—> OS virtualized
3. 100% isolated <—> Only process level isolation
4. Heavyweight operation <—> Very lightweight operation
5. Large startup time, minutes <—> Small startup time, less than seconds
6. Lots of memory needed <—> Minimal memory needed
7. Better for apps that require all of OS resources <—> Better for when we want to maximize number of apps rather than giving apps full OS resources
8. Detailed well defined security <—> simple reduced security

VM examples:
- Hyper-V, VirtualBox

Docker like container examples:
- Windows Server containers, and Linux containers like LXD

