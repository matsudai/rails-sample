ARG uid=1000
ARG gid=1000
ARG app_root=/workspaces/ruby

FROM ruby:3.2.2-bookworm

RUN apt update && \
    apt install -y \
        vim jq wget curl && \
    apt clean && rm -rf /var/lib/apt/lists/*

ARG gid
ARG uid
ARG app_root

RUN groupadd -g ${gid} ruby && \
    useradd -u ${uid} -g ${gid} -s /bin/bash -m ruby

USER ruby

WORKDIR ${app_root}

ENV BUNDLE_APP_CONFIG=${app_root}/.bundle
ENV BUNDLE_BIN=${app_root}/vendor/bundle/bin
ENV BUNDLE_PATH=${app_root}/vendor/bundle

ENV PATH="${app_root}/bin:${app_root}/vendor/bundle/bin:${PATH}"
