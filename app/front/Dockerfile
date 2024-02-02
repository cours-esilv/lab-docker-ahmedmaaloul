FROM nginx:latest

WORKDIR /usr/share/nginx/html

COPY . .

RUN chmod +x entrypoint.sh
RUN apt update && apt install dos2unix && dos2unix entrypoint.sh

ENTRYPOINT ["./entrypoint.sh"]