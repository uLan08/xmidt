# xmidt

Xmidt (pronounced "transmit") is a combination of a server cluster and client that provide a highly available data path to devices deployed all over the world.

# tl;dr summary

A device connects to the xmidt cloud via the xmidt client.  Cloud based services can use the xmidt cloud api to send and receive messages from the devices without needing to worry about where the device is in the world or in the network.  Push and pull data from the device with ease.

# the xmidt servers

### [caduceus](https://github.com/xmidt-org/caduceus)

Caduceus provides the pub-sub message delivery mechanism for xmidt.

[![Build Status](https://travis-ci.com/xmidt-org/caduceus.svg?branch=master)](https://travis-ci.com/xmidt-org/caduceus) 
[![codecov.io](http://codecov.io/github/xmidt-org/caduceus/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/caduceus?branch=master)
[![Go Report Card](https://goreportcard.com/badge/github.com/xmidt-org/caduceus)](https://goreportcard.com/report/github.com/xmidt-org/caduceus)
[![Code Climate](https://codeclimate.com/github/xmidt-org/caduceus/badges/gpa.svg)](https://codeclimate.com/github/xmidt-org/caduceus)
[![Issue Count](https://codeclimate.com/github/xmidt-org/caduceus/badges/issue_count.svg)](https://codeclimate.com/github/xmidt-org/caduceus)
[![Apache V2 License](http://img.shields.io/badge/license-Apache%20V2-blue.svg)](https://github.com/xmidt-org/caduceus/blob/master/LICENSE)


### [scytale](https://github.com/xmidt-org/scytale)

Scytale accepts the inbound requests, fans out across data centers and delivers the messages to the Talaria machines that could be hosting the device connection.

[![Build Status](https://travis-ci.com/xmidt-org/scytale.svg?branch=master)](https://travis-ci.com/xmidt-org/scytale) 
[![codecov.io](http://codecov.io/github/xmidt-org/scytale/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/scytale?branch=master)
[![Go Report Card](https://goreportcard.com/badge/github.com/xmidt-org/scytale)](https://goreportcard.com/report/github.com/xmidt-org/scytale)
[![Code Climate](https://codeclimate.com/github/xmidt-org/scytale/badges/gpa.svg)](https://codeclimate.com/github/xmidt-org/scytale)
[![Issue Count](https://codeclimate.com/github/xmidt-org/scytale/badges/issue_count.svg)](https://codeclimate.com/github/xmidt-org/scytale)
[![Apache V2 License](http://img.shields.io/badge/license-Apache%20V2-blue.svg)](https://github.com/xmidt-org/scytale/blob/master/LICENSE)


### [talaria](https://github.com/xmidt-org/talaria)

Talaria maintains the secure websocket connections from the device and passes the messages from or to the device.

[![Build Status](https://travis-ci.com/xmidt-org/talaria.svg?branch=master)](https://travis-ci.com/xmidt-org/talaria) 
[![codecov.io](http://codecov.io/github/xmidt-org/talaria/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/talaria?branch=master)
[![Go Report Card](https://goreportcard.com/badge/github.com/xmidt-org/talaria)](https://goreportcard.com/report/github.com/xmidt-org/talaria)
[![Code Climate](https://codeclimate.com/github/xmidt-org/talaria/badges/gpa.svg)](https://codeclimate.com/github/xmidt-org/talaria)
[![Issue Count](https://codeclimate.com/github/xmidt-org/talaria/badges/issue_count.svg)](https://codeclimate.com/github/xmidt-org/talaria)
[![Apache V2 License](http://img.shields.io/badge/license-Apache%20V2-blue.svg)](https://github.com/xmidt-org/talaria/blob/master/LICENSE)


### [petasos](https://github.com/xmidt-org/petasos)

Petasos helps reduce the load on the Talaria machines during mass reboot cases by calculating which specific Talaria a device should connect to & redirecting the incoming request.

[![Build Status](https://travis-ci.com/xmidt-org/petasos.svg?branch=master)](https://travis-ci.com/xmidt-org/petasos) 
[![codecov.io](http://codecov.io/github/xmidt-org/petasos/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/petasos?branch=master)
[![Go Report Card](https://goreportcard.com/badge/github.com/xmidt-org/petasos)](https://goreportcard.com/report/github.com/xmidt-org/petasos)
[![Code Climate](https://codeclimate.com/github/xmidt-org/petasos/badges/gpa.svg)](https://codeclimate.com/github/xmidt-org/petasos)
[![Issue Count](https://codeclimate.com/github/xmidt-org/petasos/badges/issue_count.svg)](https://codeclimate.com/github/xmidt-org/petasos)
[![Apache V2 License](http://img.shields.io/badge/license-Apache%20V2-blue.svg)](https://github.com/xmidt-org/petasos/blob/master/LICENSE)

### [mnemosyne](https://github.com/xmidt-org/mnemosyne)

Mnemosyne provides a mapping between names of devices.

# the xmidt client

### [parodus](https://github.com/xmidt-org/parodus)

Parodus is the light weight client that reaches out to the xmidt cloud to establish the connection.

[![Build Status](https://travis-ci.com/xmidt-org/parodus.svg?branch=master)](https://travis-ci.com/xmidt-org/parodus)
[![codecov.io](http://codecov.io/github/xmidt-org/parodus/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/parodus?branch=master)
[![Coverity](https://img.shields.io/coverity/scan/11192.svg)](https://scan.coverity.com/projects/comcast-parodus)
[![Apache V2 License](http://img.shields.io/badge/license-Apache%20V2-blue.svg)](https://github.com/xmidt-org/parodus/blob/master/LICENSE)

# server support libraries

### [webpa-common](https://github.com/xmidt-org/webpa-common)

[![Build Status](https://travis-ci.com/xmidt-org/webpa-common.svg?branch=master)](https://travis-ci.com/xmidt-org/webpa-common) 
[![codecov.io](http://codecov.io/github/xmidt-org/webpa-common/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/webpa-common?branch=master)
[![Go Report Card](https://goreportcard.com/badge/github.com/xmidt-org/webpa-common)](https://goreportcard.com/report/github.com/xmidt-org/webpa-common)

### [kratos](https://github.com/xmidt-org/kratos)

[![Build Status](https://travis-ci.com/xmidt-org/kratos.svg?branch=master)](https://travis-ci.com/xmidt-org/kratos)
[![codecov.io](http://codecov.io/github/xmidt-org/kratos/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/kratos?branch=master)
[![Go Report Card](https://goreportcard.com/badge/github.com/xmidt-org/kratos)](https://goreportcard.com/report/github.com/xmidt-org/kratos)

### [golang-money](https://github.com/xmidt-org/golang-money)

[![Build Status](https://travis-ci.com/xmidt-org/golang-money.svg?branch=master)](https://travis-ci.com/xmidt-org/golang-money) 
[![codecov.io](http://codecov.io/github/xmidt-org/golang-money/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/golang-money?branch=master) 
[![Go Report Card](https://goreportcard.com/badge/github.com/xmidt-org/golang-money)](https://goreportcard.com/report/github.com/xmidt-org/golang-money) 

### [tr18b1e](https://github.com/xmidt-org/tr18b1e)

[![Build Status](https://travis-ci.com/xmidt-org/tr18b1e.svg?branch=master)](https://travis-ci.com/xmidt-org/tr18b1e)
[![codecov.io](http://codecov.io/github/xmidt-org/tr18b1e/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/tr18b1e?branch=master)
[![Go Report Card](https://goreportcard.com/badge/github.com/xmidt-org/tr18b1e)](https://goreportcard.com/report/github.com/xmidt-org/tr18b1e)

### [golang-discovery-client](https://github.com/xmidt-org/golang-discovery-client)

[![Build Status](https://travis-ci.com/xmidt-org/golang-discovery-client.svg?branch=master)](https://travis-ci.com/xmidt-org/golang-discovery-client) 
[![codecov.io](http://codecov.io/github/xmidt-org/golang-discovery-client/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/golang-discovery-client?branch=master) 
[![Go Report Card](https://goreportcard.com/badge/github.com/xmidt-org/golang-discovery-client)](https://goreportcard.com/report/github.com/xmidt-org/golang-discovery-client) 

# client support libraries

### [nopoll fork](https://github.com/xmidt-org/nopoll)

### [cimplog](https://github.com/xmidt-org/cimplog)

[![Build Status](https://travis-ci.com/xmidt-org/cimplog.svg?branch=master)](https://travis-ci.com/xmidt-org/cimplog)
[![codecov.io](http://codecov.io/github/xmidt-org/cimplog/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/cimplog?branch=master)
[![Coverity](https://img.shields.io/coverity/scan/11572.svg)]("https://scan.coverity.com/projects/comcast-cimplog)
[![Apache V2 License](http://img.shields.io/badge/license-Apache%20V2-blue.svg)](https://github.com/xmidt-org/cimplog/blob/master/LICENSE.txt)

### [seshat](https://github.com/xmidt-org/seshat)

[![Build Status](https://travis-ci.com/xmidt-org/seshat.svg?branch=master)](https://travis-ci.com/xmidt-org/seshat)
[![codecov.io](http://codecov.io/github/xmidt-org/seshat/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/seshat?branch=master)
[![Coverity](https://img.shields.io/coverity/scan/11941.svg)]("https://scan.coverity.com/projects/comcast-seshat)
[![Apache V2 License](http://img.shields.io/badge/license-Apache%20V2-blue.svg)](https://github.com/xmidt-org/seshat/blob/master/LICENSE.txt)

### [cjwt](https://github.com/xmidt-org/cjwt)

[![Build Status](https://travis-ci.com/xmidt-org/cjwt.svg?branch=master)](https://travis-ci.com/xmidt-org/cjwt)
[![codecov.io](http://codecov.io/github/xmidt-org/cjwt/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/cjwt?branch=master)
[![Coverity](https://img.shields.io/coverity/scan/11926.svg)]("https://scan.coverity.com/projects/comcast-cjwt)
[![Apache V2 License](http://img.shields.io/badge/license-Apache%20V2-blue.svg)](https://github.com/xmidt-org/cjwt/blob/master/LICENSE.txt)

### [cjson-extras](https://github.com/xmidt-org/cjson-extras)

### [libucresolv](https://github.com/xmidt-org/libucresolv)

### [wrp-c](https://github.com/xmidt-org/wrp-c)

[![Build Status](https://travis-ci.com/xmidt-org/wrp-c.svg?branch=master)](https://travis-ci.com/xmidt-org/wrp-c)
[![codecov.io](http://codecov.io/github/xmidt-org/wrp-c/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/wrp-c?branch=master)
[![Coverity](https://img.shields.io/coverity/scan/9155.svg)]("https://scan.coverity.com/projects/comcast-wrp-c)
[![Apache V2 License](http://img.shields.io/badge/license-Apache%20V2-blue.svg)](https://github.com/xmidt-org/wrp-c/blob/master/LICENSE.txt)

### [trower-base64](https://github.com/xmidt-org/trower-base64)

[![Build Status](https://travis-ci.com/xmidt-org/trower-base64.svg?branch=master)](https://travis-ci.com/xmidt-org/trower-base64) [![codecov.io](http://codecov.io/github/xmidt-org/trower-base64/coverage.svg?branch=master)](http://codecov.io/github/xmidt-org/trower-base64?branch=master)
[![coverity](https://img.shields.io/coverity/scan/9029.svg)](https://scan.coverity.com/projects/trower-base64)
