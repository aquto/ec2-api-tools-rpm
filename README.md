
# CentOS/RPM Packaging for Amazon EC2 API Command Line Tools 

This repository contains CentOS/RPM packaging for the [Amazon EC2 API
Tools] (http://aws.amazon.com/developertools/351), which are
command-line utilities that interface with Amazon's EC2 service.

If you wish to use `rpm`, or `yum` to install the Amazon
API Tools on a Redhat/CentOS system, then you might
be interested in this packaging.

Current EC2 API CLI Version in this repo is 1.6.7.1. 

## Requirements

Requires the following packages to be installed:
rpm-build

## Usage

### Building the Redhat/CentOS packages 

1. Clone this repository 
2. In the repository home directory, run

rpmbuild --target=noarch --define "_projectdir `pwd`" -v -bb install/SPEC/ec2-api-tools.spec  

RPM will be built and will be located ~/rpmbuild/RPMS/noarch/ec2-api-tools-1.6.7-1.noarch.rpm

## Information
If you are just looking for the rpm, check out the rpm folder in this project 
 
