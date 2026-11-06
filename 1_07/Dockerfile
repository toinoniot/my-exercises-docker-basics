FROM ubuntu:24.04

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the hello.sh file from this location to /usr/src/app/ creating /usr/src/app/hello.sh.
COPY script.sh .

# Execute a command with `/bin/sh -c` prefix.
RUN apt-get update
RUN apt-get install -y curl

# When running Docker run
CMD ["/usr/src/app/script.sh"]
