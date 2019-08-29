swiperproxy
===========

[![Build Status](https://travis-ci.org/swiperproxy/swiperproxy.svg?branch=develop)](https://travis-ci.org/swiperproxy/swiperproxy)

SwiperProxy is a very easy to use HTTP and HTTPS web proxy.

![SwiperProxy Screenshot](doc/screenshot.png)

Docker image for swiperproxy
----------------------------

### Building

Run `build.sh`

### Usage

You need to specify some environment settings in order for the container to work properly, namely:

* SP_HOSTNAME - `hostname` in `proxy.conf`
* SP_HTTP_PORT - `http_port` in `proxy.conf`
* SP_HTTPS_PORT= `https_port` in `proxy.conf`

Example:

```
docker run -e SP_HOSTNAME=proxy.example.org -e SP_HTTP_PORT=80 -e SP_HTTPS_PORT=443 -p80:8080 -p443:40443 swiperproxy/swiperproxy
```
License
-------

SwiperProxy is licensed under the MIT license. See the `COPYING.md`
file in `/doc/`.

Download
--------

See <https://swiperproxy.github.io/download.html> for releases and git
checkout instructions.

Create a clone of this repository
---------------------------------

Clone the repo by running:
`$ git clone https://github.com/SwiperProxy/swiperproxy.git`

Support
-------

Commercial installation and support is not available. For general
community support, see <https://swiperproxy.github.io/contact.html>.
