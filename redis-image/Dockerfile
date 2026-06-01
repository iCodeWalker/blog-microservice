# Use an existing image as a base
# FROM Instruction : It is to specify the docker image that we want to use as a base
# The purpose to specify a base image is to give us an initial starting point or initial set of programs that we can use to further customize our image. 
FROM alpine

# Download and install a dependency
# RUN Instruction : Is used to execute some command while we are preparing our custom image 
RUN apk add --update redis

RUN apk add --update gcc

# Tell the image what to do when it starts as a container 
# CMD Instruction : What should be executed when our image is used to start up a brand new container 
CMD ["redis-server"]



## We take the image that was generated during the previous step, We create a new container from it, we execute the command in the container or make changes to the file it's system, We than look at that container, We take a snapshot of it's file system and save it as an output for the next instruction along the chain, and when there is no more instructions to execute, the image that was generated during the last step is the output from the entire process as the final image.  