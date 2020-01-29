## run docker container with bash
docker exec -it <mycontainer> bash

## copy file to container
docker cp wine.data 7f668770f536:/home/jovyan/wine.data

## run container
docker run -v /Users/pvlhead/code/docker:/home/jovyan/ -p 8888:8888 jupyter/scipy-notebook:17aba6048f44

## build/run with volume and name
docker build -t my_notebook
docker run -v /Users/pvlhead/code/docker:/home/jovyan/ -p 8888:8888 my_notebook


docker-compose up
