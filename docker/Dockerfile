FROM gcc

LABEL maintainer="@joshuacook"

RUN sed -i 's|http://deb.debian.org/debian|http://ftp.debian.org/debian|g' /etc/apt/sources.list && \
    apt-get update && \
    apt-get update --fix-missing && \
    apt-get install -y \
    gsl-bin \
    libgsl0-dbg \
    libgsl0-dev \
    libgsl27 \
    libgslcblas0 && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
