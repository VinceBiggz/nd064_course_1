# set the base image. Since we're running 
# a Go application a Go base image is used
FROM golang:alpine

# set a key-value label for the Docker image
LABEL maintainer="Vincent Wachira"

#  defines the working directory within the container
WORKDIR /go/src/app

# add files to the working directory
ADD . .

# run commands within the container. 
# to build the application
RUN go build -o helloworld

# open the port for the applcaition
EXPOSE 6111

# command to run on container start.
CMD [ "./helloworld" ]

