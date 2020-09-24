language: generic
sudo: required

services:
  - docker

before_install:
  - docker build -t stephengrider/docker-react -f Dockerfile.dev .

script:
  - docker run -e CI=true stephengrider/docker-react npm run test
