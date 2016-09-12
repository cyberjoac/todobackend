FROM jhagege/todobackend-base:latest
MAINTAINER Joachim Hagege <cyberjoac@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse