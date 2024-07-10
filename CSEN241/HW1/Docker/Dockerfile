FROM ubuntu:20.04

# Update the package list
RUN apt-get update

# Install sysbench
RUN apt-get install -y sysbench

# Copy multiple scripts
COPY cpu1000.sh cpu2000.sh fileiorrw.sh fileioseq.sh mem1M.sh mem512K.sh tests.sh /

# Set the entry point to tests.sh
ENTRYPOINT ["/tests.sh"]
