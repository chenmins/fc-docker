FROM aliyunfc/runtime-python2.7:base

RUN apt-get install -y vim \ 
    cmake \
    zip \
    clang \
    build-essential \
    libgmp3-dev \
    python2.7-dev 

RUN curl -s https://gosspublic.alicdn.com/fcli/fcli-v1.0.1-linux-amd64.zip > fcli.zip \
    && unzip -o fcli.zip -d /usr/local/bin/ \
    && rm fcli.zip

RUN curl -s https://gosspublic.alicdn.com/fun/fun-v2.9.3-linux-x64.zip > fun.zip \
    && unzip -o fun.zip -d /usr/local/bin/ \
    && rm fun.zip \
    && mv /usr/local/bin/fun-v* /usr/local/bin/fun

WORKDIR /code
