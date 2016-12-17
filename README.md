ShadowsocksR
===========

[![Build Status]][Travis CI]

A fast tunnel proxy that helps you bypass firewalls.

Server
------

### Install

Debian / Ubuntu:

    apt-get install git
    git clone https://github.com/dearzhangyi/shadowsocks.git

CentOS:

    yum install git
    git clone https://github.com/dearzhangyi/shadowsocks.git

Windows:

    git clone https://github.com/dearzhangyi/shadowsocks.git

### Usage for single user on linux platform

If you clone it into "~/shadowsocks"  
move to "~/shadowsocks", then run:

    bash initcfg.sh

move to "~/shadowsocks/shadowsocks", then run:

    python server.py -p 443 -k password -m aes-128-cfb -O auth_aes128_md5_compatible -o tls1.2_ticket_auth_compatible

Check all the options via `-h`.

You can also use a configuration file instead (recommand), move to "~/shadowsocks" and edit the file "user-config.json", then move to "~/shadowsocks/shadowsocks" again, just run:

    python server.py

To run in the background:

    ./logrun.sh

To stop:

    ./stop.sh

To monitor the log:

    ./tail.sh


Client
------

* [Windows] / [OS X]
* [Android] / [iOS]
* [OpenWRT]

Use GUI clients on your local PC/phones. Check the README of your client
for more information.

Documentation
-------------

You can find all the documentation in the [Wiki].

License
-------

Copyright 2015 clowwindy

Licensed under the Apache License, Version 2.0 (the "License"); you may
not use this file except in compliance with the License. You may obtain
a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
License for the specific language governing permissions and limitations
under the License.

Bugs and Issues
----------------

* [Issue Tracker]



[Android]:           https://github.com/shadowsocks/shadowsocks-android
[Build Status]:      https://travis-ci.org/falseen/shadowsocks.svg?branch=manyuser-travis
[Debian sid]:        https://packages.debian.org/unstable/python/shadowsocks
[iOS]:               https://github.com/shadowsocks/shadowsocks-iOS/wiki/Help
[Issue Tracker]:     https://github.com/breakwa11/shadowsocks/issues?state=open
[OpenWRT]:           https://github.com/shadowsocks/openwrt-shadowsocks
[OS X]:              https://github.com/shadowsocks/shadowsocks-iOS/wiki/Shadowsocks-for-OSX-Help
[Travis CI]:         https://travis-ci.org/falseen/shadowsocks
[Windows]:           https://github.com/breakwa11/shadowsocks-csharp
[Wiki]:              https://github.com/breakwa11/shadowsocks-rss/wiki
