# jenkins-docker

To allow Docker based builds through a Docker running Jenkins Server.

`docker run -p 8080:8080 -p 50000:50000 -v /var/run/docker.sock:/var/run/docker.sock -v /Users/stefan/Docker/jenkins_home:/var/jenkins_home jenkins-docker`

## Manual docker image build

`docker build -t "jenkins-docker" .`

`docker login`

`docker tag 35075fe8dd73 sogis/jenkins-docker` 

`docker push sogis/jenkins-docker`