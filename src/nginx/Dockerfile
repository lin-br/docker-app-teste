ARG IMAGE_NGINX

FROM nginx:${IMAGE_NGINX}

ENV TZ=America/Sao_Paulo
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
