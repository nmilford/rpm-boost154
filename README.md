rpm-boost
=========

An RPM spec file to build and install the Boost C++ libraries.

To Build:

`sudo yum -y install rpmdevtools && rpmdev-setuptree`

`sudo yum -y install bzip2-devel gcc44-c++ python-devel python-libs libicu-devel openmpi-libs`

`wget http://downloads.sourceforge.net/project/boost/boost/1.54.0/boost_1_54_0.tar.gz -O ~/rpmbuild/SOURCES/boost_1_54_0.tar.gz`

`wget https://raw.github.com/nmilford/rpm-boost154/master/boost154.spec -O ~/rpmbuild/SPECS/boost154.spec`

`rpmbuild -bb ~/rpmbuild/SPECS/boost154.spec`
