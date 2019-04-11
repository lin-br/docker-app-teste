ARG IMAGE_MARIADB

FROM mariadb:${IMAGE_MARIADB}

ENV TZ=America/Sao_Paulo
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
