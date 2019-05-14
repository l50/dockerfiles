FROM kalilinux/kali-linux-docker
LABEL maintainer "Jayson Grace <jayson.e.grace@gmail.com>"

RUN set -x \
&& echo "[INFO] Installing Dependencies..." \
&& apt-get update \
  && apt-get upgrade -y \
&& apt-get install -y \
  --no-install-recommends \
  dirb \
&& echo "[INFO] Removing Build Dependencies..." \
&& apt-get autoremove --purge -y \
&& apt-get clean \
&& rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

ENTRYPOINT ["dirb"]
