# jenkins2

taken from the original (official) jenkins build.

#### build image:
    docker build --build-arg http_proxy=http://myproxy.com:8080 --build-arg https_proxy=http://myproxy.com:8080 --build-arg no_proxy=.mydomain.com,.myseconddomain.com -t "jenkins2" jenkins/
#### run container:
    docker run --name "jenkins2" -p 8050:8080 -p 50000:50000 -v /opt/jenkins2/:/var/jenkins_home jenkins2

the user jenkins must have access rights to the directory "/opt/jenkins2/"
