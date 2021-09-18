FROM python:alpine

RUN apk add build-base libxml2-dev libxslt-dev \
    && pip install parsedmarc

RUN mkdir /app
WORKDIR /app

COPY parsedmarc.ini ./

ENTRYPOINT ["parsedmarc", "-c", "parsedmarc.ini"]
