FROM amirzaidi2002/todobackend-base:latest
MAINTAINER Amir Zaidi <amir.zaidi@dell.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse