# 9.3.9 in production
FROM postgres:9.3.9

# 2.1.4 in production
ENV POSTGIS_MAJOR 2.3

RUN apt-get update \
      && apt-get install -y \
           postgresql-$PG_MAJOR-postgis-$POSTGIS_MAJOR \
           postgresql-$PG_MAJOR-postgis-$POSTGIS_MAJOR-scripts \
      && rm -rf /var/lib/apt/lists/*
