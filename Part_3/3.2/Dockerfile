FROM ubuntu:16.04 

ENV LC_ALL=C.UTF-8 

RUN apt-get update && apt-get install -y \ 
    python python3-pip ffmpeg wget php7.0-cli php-bcmath curl php-xml && \ 
    pip3 install -U yle-dl && \  
    apt-get purge -y --auto-remove curl && \ 
    rm -rf /var/lib/apt/lists/* 

WORKDIR /app

ENTRYPOINT ["yle-dl"]
