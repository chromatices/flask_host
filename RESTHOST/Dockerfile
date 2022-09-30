FROM python:3.8.8

LABEL email='bomebug15@keti.re.kr'

ARG DEBIAN_FRONTEND=noninteractive
ENV TZ=Asia/Seoul
RUN ["apt-get", "install", "-y", "tzdata"]

ENV HOME=/home/

RUN ["mkdir", "-p", "${HOME}/"]

RUN ["pip","install","flask"]

WORKDIR ${HOME}

COPY ["./src", "."]

CMD ["python3", "rest-host.py"]