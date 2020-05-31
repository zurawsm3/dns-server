FROM arm32v7/debian:buster-slim

RUN apt-get update && apt-get install -y bind9

COPY ./named.conf /etc/bind/

ENTRYPOINT ["named"]
CMD ["-f"]

