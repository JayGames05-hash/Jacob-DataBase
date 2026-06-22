FROM alpine:latest

WORKDIR /app

COPY pocketbase /app/pocketbase
COPY reset_admin.sh /app/reset_admin.sh

RUN chmod +x /app/pocketbase
RUN chmod +x /app/reset_admin.sh

EXPOSE 8080

CMD ["./pocketbase", "serve", "--http=0.0.0.0:$PORT"]
