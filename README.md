sonic-nas-common
===============

This repo contains the common utilities for the network abstraction service (NAS). This provides utilities to obtain interface mapping, switch configurations, and so on.

Build
---------
Please see the instructions in the sonic-nas-manifest repo for more details on the common build tools. See [sonic-nas-manifest](https://github.com/Azure/sonic-nas-manifest) for more information on common build tools.

### Development dependencies
* `sonic-base-model`
* `sonic-common-utils`
* `sonic-object-library`
* `sonic-logging`

### Dependent packages
* `libsonic-logging-dev` 
* `libsonic-logging1`
* `libsonic-model1` 
* `libsonic-model-dev` 
* `libsonic-common1` 
* `libsonic-common-dev` 
* `libsonic-object-library1` 
* `libsonic-object-library-dev`

### Build command
    sonic_build --dpkg libsonic-logging-dev libsonic-logging1 libsonic-model1 libsonic-model-dev libsonic-common1 libsonic-common-dev libsonic-object-library1 libsonic-object-library-dev -- clean binary

(c) Dell 2016
