From python:3.8.2-buster

RUN apt-get update && apt-get install -y \
    python-zeroc-ice \
    python-pil \
    python-simplejson \
    mercurial \
    python-pil \
    build-essential \
    python-dev \
    libjpeg-dev
RUN apt-get install -y \
    libpng16-16 \
    libfreetype6-dev \
    libbz2-dev \
 && rm -rf /var/lib/apt/lists/*

RUN pip install --upgrade pip
RUN pip install Pillow 
RUN pip install zeroc-ice
RUN cd /usr/src && hg clone http://bitbucket.org/Svedrin/mumble-django && mv mumble-django app
RUN cd /usr/src/app && hg update stable
