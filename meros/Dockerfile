FROM nimlang/nim:1.0.4 AS builder
RUN apt-get update && apt-get install -y \
    git \
    gcc \
    g++ \
    make \
    cmake \
    autoconf \
    automake \
    libtool \
    curl
RUN git clone https://github.com/MerosCrypto/Meros && \
    cd Meros && \
    nimble build -y -d:nogui

FROM ubuntu:devel
COPY --from=builder ./Meros/build/Meros .
CMD ["./Meros"]