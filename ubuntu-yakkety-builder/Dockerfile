FROM ubuntu:yakkety
RUN apt-get -y update && apt-get -y dist-upgrade
RUN apt-get -y install nano sudo apt-utils dnsutils psmisc pv dialog irssi irssi-scripts mc mc-data screen 
RUN apt-get -y install automake autoconf autopoint autogen autoproject autotools-dev build-essential *-6-multilib bison flex
RUN apt-get -y install doxygen libjson-glib-dev libpurple-dev yasm nasm ccache openjdk-8-jre-headless
RUN apt-get -y install git cvs mercurial subversion curl perl-base python python3 python-pip python3-pip
RUN echo "imnx ALL=NOPASSWD:ALL" > /etc/sudoers.d/myOverrides
RUN read -p "Password to use for new user [iMnX]: " newPassword
RUN useradd -m -p "$newPassword" imnx
CMD bash
