ARG TIMEZONE
ARG IMAGE_NGINX

FROM nginx:${IMAGE_NGINX}

ENV TZ=${TIMEZONE}
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
