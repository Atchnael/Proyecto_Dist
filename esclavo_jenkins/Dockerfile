FROM evarga/jenkins-slave
USER root
RUN apt-get update
RUN apt-get install -y git 
run apt-get install -y python-dev
run apt-get install -y python-distribute 
run apt-get install -y wget
Run wget https://bootstrap.pypa.io/get-pip.py
run python get-pip.py
run pip install virtualenv
workdir /home/jenkins
RUN mkdir /home/jenkins/.virtualenvs
workdir /home/jenkins/.virtualenvs
run virtualenv testproject
run . testproject/bin/activate
run pip install flask
run pip install pytest
run pip install pytest-cov
run pip install xmlrunner
run pip install unittest2

