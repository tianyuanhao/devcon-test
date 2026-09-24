FROM ubuntu:26.04

RUN apt-get update \
    && apt-get install --no-install-recommends -y --allow-remove-essential \
        sudo \
    && rm -r /var/lib/apt/lists

RUN echo "ubuntu ALL=(root) NOPASSWD:ALL" > /etc/sudoers.d/ubuntu \
    && chmod 440 /etc/sudoers.d/ubuntu
