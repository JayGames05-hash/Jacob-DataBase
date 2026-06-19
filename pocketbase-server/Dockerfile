FROM alpine:latest

WORKDIR /app

COPY pocketbase /app/pocketbase
COPY pb_data /app/pb_data
COPY pb_migrations /app/pb_migrations
COPY pb_public /app/pb_public

RUN chmod +x /app/pocketbase

EXPOSE 8080

CMD ["sh", "-c", "./pocketbase serve --http=0.0.0.0:${PORT}"]
