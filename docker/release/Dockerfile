FROM santoshr/todobackend-base:latest
MAINTAINER Santosh Rai <santosh.rai.acquis@gmail.com>

# Copy application artifacts
COPY target /wheelhouse

# Install application
RUN . /appenv/bin/activate && \
    pip install --no-index -f /wheelhouse todobackend && \
    rm -rf /wheelhouse