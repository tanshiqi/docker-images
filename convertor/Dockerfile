FROM gotenberg/gotenberg:7

USER root

RUN apt-get update -qq &&\
    DEBIAN_FRONTEND=noninteractive apt-get install -y -qq --no-install-recommends libreoffice-l10n-zh-cn &&\
    sed -i '/zh_CN.UTF-8/s/^# //g' /etc/locale.gen &&\
    locale-gen &&\
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

ENV LANG zh_CN.UTF-8
ENV LANGUAGE zh_CN:zh
ENV LC_ALL zh_CN.UTF-8

USER gotenberg