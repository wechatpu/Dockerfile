#+++++++++++++++++++++++++++++++++++++++
# Dockerfile for webdevops/nginx-dev:alpine
#    -- automatically generated  --
#+++++++++++++++++++++++++++++++++++++++

FROM webdevops/nginx:alpine

ENV WEB_DOCUMENT_ROOT=/app \
    WEB_DOCUMENT_INDEX=index.php \
    WEB_ALIAS_DOMAIN=*.vm

COPY conf/ /opt/docker/

# Install apache
RUN true \
    && /opt/docker/bin/bootstrap.sh \
    && docker-image-cleanup

EXPOSE 80 443
