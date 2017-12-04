FROM kirill/todobackend-base:latest
MAINTAINER kirill

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse