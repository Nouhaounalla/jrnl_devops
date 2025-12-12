# Docker Execution Guide for jrnl

## Build the image
docker build -t jrnl-app .

## Run jrnl commands
docker run jrnl-app --version
docker run -it jrnl-app

## With persistent storage
docker run -v jrnl-data:/root/.local/share/jrnl jrnl-app