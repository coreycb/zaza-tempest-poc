# Overview

This repository contains zaza yaml config and Juju bundles for
deploying/configuring various OpenStack bundles and running tempest
against the OpenStack deployment.

# How to use

git clone https://github.com/gnuoy/zaza-tempest-poc
cd zaza-tempest-poc
export OS_TEST_HTTP_PROXY=http://squid.internal:3128
export OS_TEST_FIP_RANGE=10.5.150.0:10.5.200.254
export OS_TEST_CIDR_EXT=10.5.0.0/16
export OS_TEST_GATEWAY=10.5.0.1
export OS_TEST_NAMESERVER=10.245.168.6
export OS_TEST_CIDR_PRIV=192.168.21.0/24
export OS_TEST_SWIFT_IP=10.245.161.162
tox -e func-smoke
