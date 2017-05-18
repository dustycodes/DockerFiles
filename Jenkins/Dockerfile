FROM jenkins:latest
USER root
#
ENV DEBIAN_FRONTEND noninteractive
#RUN cat /etc/apt/sources.list 
#RUN echo "deb http://us.archive.ubuntu.com/ubuntu/ xenial-backports main restricted universe multiverse" >> /etc/apt/sources.list
#ADD sources.list /etc/apt/sources.list
#RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 3B4FE6ACC0B21F32
#RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 40976EAF437D05B5 
RUN echo "deb http://www.deb-multimedia.org jessie main non-free" >> /etc/apt/sources.list
RUN echo "deb-src http://www.deb-multimedia.org jessie main non-free" >> /etc/apt/sources.list
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 5C808C2B65558117
RUN apt-get update && apt-get install deb-multimedia-keyring
RUN apt-get update && apt-get upgrade -y && apt-get install -y --no-install-recommends apt-utils

#RUN apt-get -y install libavdevice-ffmpeg56 # doesnt work for some reason
RUN apt-get -y install libavdevice-dev

RUN apt-get -y install android-tools-adb
RUN apt-get -y install audacious
RUN apt-get -y install clang
RUN apt-get -y install clang-3.8
RUN apt-get -y install clang-3.8-doc
RUN apt-get -y install clang-3.8-examples
RUN apt-get -y install cmake
RUN apt-get -y install cmake-curses-gui
RUN apt-get -y install debhelper
RUN apt-get -y install doxygen
RUN apt-get -y install emacs
RUN apt-get -y install ffmpeg
RUN apt-get -y install git
RUN apt-get -y install gksu
RUN apt-get -y install global
RUN apt-get -y install groff
RUN apt-get -y install lib32z1
RUN apt-get -y install libasound2-dev
RUN apt-get -y install libboost-chrono-dev
RUN apt-get -y install libboost-dev
RUN apt-get -y install libc6-dev
RUN apt-get -y install libclang-3.8-dev
RUN apt-get -y install libcurl4-gnutls-dev
RUN apt-get -y install libcurlpp-dev
RUN apt-get -y install libjpeg-dev
RUN apt-get -y install libpng12-dev
RUN apt-get -y install libqt4-dev
RUN apt-get -y install build-essential
RUN apt-get -y install aptitude
RUN apt-get -y install libstdc++6
RUN apt-get -y install libudev-dev
RUN apt-get -y install libusb-1.0-0-dbg
RUN apt-get -y install libusb-1.0-0-dev
RUN apt-get -y install libusb-1.0-doc
RUN apt-get -y install libusb-dev
RUN apt-get -y install libxml2-dev
RUN apt-get -y install libxml2-utils
RUN apt-get -y install libxslt1-dev
RUN apt-get -y install minicom
RUN apt-get -y install nasm
RUN apt-get -y install putty
RUN apt-get -y install pypar2
RUN apt-get -y install python-clang-3.8
RUN apt-get -y install python-dev
RUN apt-get -y install python-empy
RUN apt-get -y install python-opencv
RUN apt-get -y install python-pip
RUN apt-get -y install qt-sdk
RUN apt-get -y install remake
RUN apt-get -y install vim
USER jenkins
