FROM gotenberg/gotenberg:8

USER root

# COPY fonts/* /usr/local/share/fonts/

RUN apt-get update -qq &&\
    DEBIAN_FRONTEND=noninteractive apt-get install -y -qq --no-install-recommends -t bookworm-backports libreoffice-l10n-zh-cn &&\
    sed -i '/zh_CN.UTF-8/s/^# //g' /etc/locale.gen &&\
    locale-gen &&\
    # Cleanup.
    # Note: the Debian image does automatically a clean after each install thanks to a hook.
    # Therefore, there is no need for apt-get clean.
    # See https://stackoverflow.com/a/24417119/3248473.
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

ENV LANG zh_CN.UTF-8
ENV LANGUAGE zh_CN.UTF-8
ENV LC_ALL zh_CN.UTF-8

USER gotenberg
