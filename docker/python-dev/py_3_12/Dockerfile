# Python3.12 oficial image
FROM python:3.12
WORKDIR /workdir

# Install git & makefile
RUN apt-get update && apt-get install -y git make nano

# Install pdm
RUN pip install --no-cache-dir pdm
ENV PATH="/root/.local/bin:${PATH}"

# Init a bash interactive shell
CMD ["/bin/bash"]