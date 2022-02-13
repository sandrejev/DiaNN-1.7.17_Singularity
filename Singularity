Bootstrap: docker

From: ubuntu:focal


%help
    Help me. I'm in the container.

%files
    DiaNN-1.7.17.zip

%post
    apt-get update
    apt-get install -y unzip build-essential
    unzip /DiaNN-1.7.17.zip -d /opt
    cd /opt/DiaNN-1.7.17/mstoolkit/
    make

%runscript
    echo "Arguments received: $*"
    /opt/DiaNN-1.7.17/diann-linux "$@"