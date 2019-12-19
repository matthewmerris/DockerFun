# DockerFun

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
