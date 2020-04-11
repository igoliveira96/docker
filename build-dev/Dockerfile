FROM python:3.6
LABEL maintener="Igor Goulart de Oliveira"

RUN useradd www && \
  mkdir /app && \
  mkdir /log && \
  chown www /log

USER www
VOLUME /log
# Diretório de trabalho
WORKDIR /app
# Expondo a porta 8000
EXPOSE 8000

ENTRYPOINT [ "/usr/local/bin/python" ]
CMD [ "run.py" ]