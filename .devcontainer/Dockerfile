FROM node:12-slim

# update all
RUN apt-get update && apt-get install -y --no-install-recommends

# install git
RUN apt-get install -y git

# install angular cli
RUN npm install -g @angular/cli

# make work directory
RUN mkdir /workspace
WORKDIR /workspace

# Clean up
RUN apt-get autoremove -y \
    && apt-get clean -y