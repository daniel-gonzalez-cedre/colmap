# ubuntu
'''bash
    sudo apt-get install \
        git \
        cmake \
        build-essential \
        libboost-program-options-dev \
        libboost-filesystem-dev \
        libboost-graph-dev \
        libboost-regex-dev \
        libboost-system-dev \
        libboost-test-dev \
        libeigen3-dev \
        libsuitesparse-dev \
        libfreeimage-dev \
        libgoogle-glog-dev \
        libgflags-dev \
        libglew-dev \
        qtbase5-dev \
        libqt5opengl5-dev \
        libcgal-dev
'''

# ubuntu 16.04 and 18.04
'''bash
    sudo apt-get install libcgal-qt5-dev
'''

# install ceres solver
'''bash
    sudo apt-get install libatlas-base-dev libsuitesparse-dev
    git clone https://ceres-solver.googlesource.com/ceres-solver
    cd ceres-solver
    git checkout $(git describe --tags) # Checkout the latest release
    mkdir build
    cd build
    cmake .. -DBUILD_TESTING=OFF -DBUILD_EXAMPLES=OFF
    make
    sudo make install
'''

# configure and install colmap
'''bash
    git clone https://github.com/colmap/colmap.git
    cd colmap
    git checkout dev
    mkdir build
    cd build
    cmake ..
    make
    sudo make install
'''
