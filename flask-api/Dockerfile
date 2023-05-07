## It pulls the python image from the Docker Hub.
FROM python:alpine3.7
## Copy everything from the current directory to /app
## Whenever a container is created, that will have directory called /app
COPY . /app
## After copying the content from current directory to /app, that /app directory becomes working directory
WORKDIR /app
## Then the required packages need to be installed by running pip install 
RUN pip install -r requirements.txt
## An Environment variable can be given here
ENV PORT 5000
## Conatainer will expose port 5000 for this application
EXPOSE 5000
## Whenever a container is created, if you want to pass a command you can use ENTRY POINT
## ENTRYPOINT can't be overwritten
ENTRYPOINT ["python"]
## CMD can be used to pass the commands to the cotainer terminal.
CMD ["app.py"]

