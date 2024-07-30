FROM ubuntu:20.04
ARG user=raj
ARG group=raj
ARG uid=1000
ARG gid=1000
ENV USER_HOME_DIR=/home/raj
RUN groupadd -g ${gid} ${group} \ 
&& useradd -d "$USER_HOME_DIR" -u ${uid} -g ${gid} -m -s /bin/bash ${user}
USER ${user} # sets the user in container 
WORKDIR ${USER_HOME_DIR} # sets the directory 
CMD ["echo", "helloworld"]