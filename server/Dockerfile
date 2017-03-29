# 3.3.4 in production
FROM python:3.3
RUN apt-get update && apt-get install -y \
    binutils libproj-dev gdal-bin
COPY docker-entrypoint.sh /usr/bin/docker-entrypoint
RUN chmod +x /usr/bin/docker-entrypoint
ADD data/server/requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt
RUN mkdir /switchapp
WORKDIR /switchapp
