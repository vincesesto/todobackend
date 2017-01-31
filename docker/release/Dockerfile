FROM vsesto/todobackend-base:latest
MAINTAINER Vince Sesto <vincent.sesto@airnz.co.nz>

COPY target /wheelhouse

RUN chmod u+x ./appenv/bin/activate

RUN ./appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse
