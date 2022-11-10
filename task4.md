# **SAIC SysAdmin Test**
## Task 1. Docker Deployments

Run multiple website on different docker conatiners

1. CP DASHBOARD(ReactJS)
- Clone the github repo.
- Change the directory to CP-DASHBOARD
- Make a Dockerfile.
Contents of the docker file are below.
~~~
FROM node:alpine
WORKDIR '/app'
COPY package.json .
RUN npm install --force
COPY . .
CMD ["npm", "start"]
~~~



2. STAC IIT Mandi
- Clone the github repo.
- Change the directory to xray-burst-detection
- Make a Dockerfile.
Contents of the docker file are below.
~~~
FROM ubuntu
RUN apt update
RUN apt install python3-pip -y
WORKDIR /app
COPY . .
RUN pip3 install -r /app/requirements.txt
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]
~~~


3. SAIC IIT Mandi
- Clone the github repo.
- Change the directory to CP-DASHBOARD
- Make a Dockerfile.
~~~

~~~
