FROM bitnami/odoo:12-debian-10
MAINTAINER Fábrica de Software Libre S.A. <soporte@fslibre.com>

#USER root

RUN set -x; \
        apt-get update \
        && apt-get install -y --no-install-recommends \
            git \
            vim \
            mc \
            libsasl2-dev \
            libssl-dev \
            build-essential \
            libldap2-dev \
            python3-dev \
            python3-pandas \
            default-jdk \
            default-jre \
            libreoffice-writer \
            libreoffice-calc

RUN pip3 install \
        pyotp \
        unidecode \
        wand \
        checksumdir \
        cachetools \
        validate_email \
        simplejson \
        oauthlib \
        pyqrcode \ 
        pyldap \
        zeep \
        xmltodict \
        odoorpc \
        openpyxl \
        pyzk \
        viivakoodi \
        raven \
        xlrd \
        xlwt \
        email_validator \
        py3o.template \
        py3o.formats \
        PyPDF2 \
        netifaces \
        wdb

RUN python3 -m pip install redis
RUN python3 -m pip install paramiko
RUN pip3 install openupgradelib

#RUN usermod -u 1500 odoo
#RUN groupmod -g 1500 odoo

#USER odoo
