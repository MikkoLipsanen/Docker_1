FROM ubuntu:latest

WORKDIR /mydir
RUN apt-get update && apt-get install -y curl wget

COPY script.sh .
CMD ["/mydir/script.sh"]

