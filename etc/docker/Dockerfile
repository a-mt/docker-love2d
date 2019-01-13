FROM ubuntu

RUN apt-get update && apt-get install -y software-properties-common

# Install love
RUN add-apt-repository -y ppa:bartbes/love-stable && apt-get install -y love

# Install Zerobrane Studio
RUN apt-get install -y libgtk2.0-0 xdg-utils
RUN apt-get install -y curl unzip

RUN curl --output /tmp/ZeroBraneStudio.zip --location https://github.com/pkulchenko/ZeroBraneStudio/archive/master.zip; \
    unzip -d /tmp /tmp/ZeroBraneStudio.zip; \
    mv /tmp/ZeroBraneStudio-master /usr/sbin/ZeroBraneStudio;

# Settings
RUN useradd -ms /bin/bash project
USER 1000:1000
WORKDIR /usr/sbin/ZeroBraneStudio

# Run CLI
CMD ["/bin/bash"]
