FROM debian:stable-slim

WORKDIR /app

COPY pocketbase /app/pocketbase

RUN chmod +x /app/pocketbase

EXPOSE 8080

CMD ["./pocketbase", "serve", "--http=0.0.0.0:$PORT"]
