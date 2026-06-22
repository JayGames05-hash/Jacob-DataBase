FROM alpine:latest

WORKDIR /app

COPY pocketbase /app/pocketbase
COPY pb_data /app/pb_data
COPY pb_migrations /app/pb_migrations
COPY pb_public /app/pb_public
COPY reset_admin.sh /app/reset_admin.sh

RUN chmod +x /app/pocketbase
RUN chmod +x /app/reset_admin.sh

EXPOSE 8080


