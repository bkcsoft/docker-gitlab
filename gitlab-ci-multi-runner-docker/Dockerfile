FROM sameersbn/gitlab-ci-multi-runner:0.5.5

# Installing Docker
RUN apt-get update && apt-get install -y docker.io && apt-get clean

# Installing Docker-Compse
RUN apt-get install -y python-pip && apt-get clean && pip install docker-compose

RUN groupadd -g 997 docker_derp && usermod -a -G docker_derp gitlab_ci_multi_runner
