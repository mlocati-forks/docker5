FROM ghcr.io/concrete5-community/docker5:base

ARG CCM_PHP_VERSION=8.1
ARG CCM_COMPOSER_VERSION=2
ARG CCM_PHPUNIT_VERSION=8
ARG CCM_C5_ARCHIVE=https://github.com/concretecms/concretecms/archive/master.tar.gz
ARG CCM_STARTING_POINT=atomik_full
ARG CCM_PATCH_ENVIRONMENT_ONLY=N
ARG CCM_INSTALL_BLOCKS_CLONER=N

COPY assets/app-patch /tmp/
COPY assets/start-patch /tmp/
COPY build /

RUN /build && rm /build
