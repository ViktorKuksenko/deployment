FROM python:3.6.7-slim-stretch

WORKDIR /app

RUN apt-get update -y

RUN apt-get -y install gcc git build-essential libtool automake

RUN pip3 install Cython

RUN pip3 install git+https://github.com/MagicStack/uvloop

RUN pip3 install sanic

RUN pip3 install asyncio_redis

RUN pip3 install asyncpg

RUN pip3 install passlib

RUN pip3 install pytest

RUN pip3 install marshmallow

RUN pip3 install aiohttp

VOLUME [ "/app" ]

EXPOSE 8000

CMD ["python3", "run.py"] 
