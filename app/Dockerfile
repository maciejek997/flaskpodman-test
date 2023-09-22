FROM --platform=amd64 python:alpine

WORKDIR /app

COPY . /app

RUN --mount=type=cache,target=/root/.cache/pip \
    pip install flask

CMD [ "python", "app.py" ]

EXPOSE 5000