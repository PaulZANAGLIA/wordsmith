FROM postgres
COPY words.sql /docker-entrypoint-initdb.d/words.sql
ENV POSTGRES_HOST_AUTH_METHOD=trust

# Build it with : docker build -t "db:Dockerfile" .