FROM python:2.7-alpine3.7

RUN set -ex \
    && apk add --no-cache --virtual .builddeps \
        build-base \
    && apk add --no-cache --virtual .rundeps \
        libxml2-dev \
        libxslt-dev \
        libffi-dev \
        openssl-dev \
        unixodbc-dev \
        libstdc++ \
    && pip install --no-cache-dir \
        lxml \
        pyodbc \
        pypyodbc \
        pytest \
        pytz \
        robotframework \
        records \
        requests \
        signxml \
        sqlalchemy \
        suds-jurko \
        tablib \
        tox \
    && apk del .builddeps
