FROM r0mdau/trinitycore-base-build

LABEL name=r0mdau/trinitycore-src

RUN set -x && \
    git clone -b 3.3.5 git://github.com/TrinityCore/TrinityCore.git && \
    cd TrinityCore/ && \
    mkdir build && \
    cd build/ && \
    cmake ../ -DCMAKE_INSTALL_PREFIX=/root && \
    time make -j 6 && \
    make -j 6 install
