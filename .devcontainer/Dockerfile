FROM buildpack-deps:bullseye

RUN apt-get update \
  && apt-get install -y python pip

RUN groupadd dev
RUN useradd -rm --home /home/dev --shell /bin/bash -g dev -G sudo -u 1001 dev
USER dev
WORKDIR /home/dev
