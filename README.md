SONiC NAS Common
===============

Common utilities for the network abstraction service 

Description
-----------

This repo contains the Common utilities for the Network abstraction service. This provides utilities for getting interface mapping, switch configurations etc.

Building
---------
Please see the instructions in the sonic-nas-manifest repo for more details on the common build tools.  [Sonic-nas-manifest](https://github.com/Azure/sonic-nas-manifest)

Development Dependencies
 - sonic-base-model
 - sonic-common-utils
 - sonic-object-library
 - sonic-logging

Dependent Packages:
- libsonic-logging-dev libsonic-logging1 libsonic-model1 libsonic-model-dev libsonic-common1 libsonic-common-dev libsonic-object-library1 libsonic-object-library-dev

BUILD CMD: sonic_build --dpkg libsonic-logging-dev libsonic-logging1 libsonic-model1 libsonic-model-dev libsonic-common1 libsonic-common-dev libsonic-object-library1 libsonic-object-library-dev -- clean binary


(c) Dell 2016
