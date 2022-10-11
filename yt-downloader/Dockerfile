# choose base image
FROM ubuntu:18.04 
WORKDIR /home #change working directory
# install needed tools
RUN apt update && apt install -y curl python
# download script 
RUN curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
# add permissions to downloaded script
RUN chmod a+x /usr/local/bin/youtube-dl 
# set environment variable
ENV LC_ALL=C.UTF-8
# set entrypoint script
ENTRYPOINT ["/usr/local/bin/youtube-dl"]
