# rpmbuild-ec2-swapfile

Create a ec2-swapfile RPM for RHEL/CentOS.

## Requirements

To download package sources and install build dependencies

    yum -y install rpmdevtools yum-utils

## Build process

To build the package follow the steps outlined below

    git clone https://github.com/linuxhq/rpmbuild-ec2-swapfile.git rpmbuild
    spectool -g -R rpmbuild/SPECS/ec2-swapfile.spec
    yum-builddep rpmbuild/SPECS/ec2-swapfile.spec
    rpmbuild -ba rpmbuild/SPECS/ec2-swapfile.spec

## License

BSD

## Author Information

This package was created by [Taylor Kimball](http://www.linuxhq.org).
