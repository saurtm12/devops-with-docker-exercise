FROM ubuntu:22.04
RUN apt update && apt upgrade && apt install -y curl
COPY ./script.sh ./script.sh
RUN chmod +x ./script.sh
CMD ./script.sh