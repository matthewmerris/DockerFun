# DockerFun

## Synaposis
A simple demonstration of the power of docker, a container
system that allows for the creation of specified development 
environments (amongst other great powers!).  This demo builds
an Ubuntu 18.04 environment for developing c applications that
need the LAPACKE library, a c wrapper for the world famous
LAPACK library(Fortran workhorse).

## Running the experiment
a brief exploration of docker:

	1st: clone repo
	2nd: from source directory, issue the following commands
		docker build docker -t test:LAPACKE
		docker run -ti test:LAPACKE
As a result of the previous commands, you should be in
an interactive terminal for the freshly built container
run the application demonstrating the DGELS routine from LAPACKE,
 which solves a least squares minimization
problem, by issuing the command:

	./callingDGELS

stdout should display a 3x2 matrix with columns 
(2,1,1) and (1,1,2)
