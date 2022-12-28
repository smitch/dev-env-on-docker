FROM python:3.11-bullseye

RUN apt-get update && apt-get install -y \
    tzdata \
&&  ln -sf /usr/share/zoneinfo/Asia/Tokyo /etc/localtime \
&&  apt-get clean \
&&  rm -rf /var/lib/apt/lists/*

ENV TZ=Asia/Tokyo

RUN python3 -m pip install --upgrade pip \
&&  pip install --no-cache-dir \
    jupyterlab
