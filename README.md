
## IP Camera RTSP stream string
https://github.com/grigory-lobkov/rtsp-camera-view/wiki/IP-Camera-RTSP-stream-string

Grigory Lobkov edited this page on Jun 28, 2018 · 2 revisions
Fix your camera IP address
To determine the IP address of your IP camera, connect to your router and watch for DHCP client list.

You should create an address reservation on router or config a static IP on your camera.

ONVIF parameters
Download an "Onvif Device Manager" https://sourceforge.net/projects/onvifdm/

Install it and run. It will show you the list of your Onvif sources. Choose desirable camera. If you will see an error about authentication, enter your Login and Password at the top of window and press "Log In".

Click "Live Video" in the middle. On the right you will see your camera video, below the video there is a string to connect your camera over RTSP.

For example: rtsp://192.168.0.4:554/live/main

If this string won't work, add some creditionals to URL:

rtsp://admin:mypass@192.168.0.4:554/live/main

RTSP streaming
You can use VLC to show this stream.

You can play URL in VLC: Open "Media" - "Open network stream" - "Network", put your URL here, "Play".
You can add URL to VLC shortcut:
"C:\Program Files (x86)\VideoLAN\VLC\vlc.exe" rtsp://admin:mypass@192.168.0.4/live/main

You can also add command line parameter "--aspect-ratio 16:9"
RTSP multi streaming
Add all your cameras to rtsp-camera-view and manage it manually.

# RTSP Camera view &nbsp; [![Share](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Watch%20your%20cameras%20in%20one%20place%20for%20free&url=https://github.com/grigory-lobkov/rtsp-camera-view&hashtags=rtsp,ip-camera,windows,c#)

[![FREE](https://img.shields.io/badge/price-FREE-0098f7.svg?style=flat-square)](https://github.com/grigory-lobkov/rtsp-camera-view/blob/master/LICENSE) 
[![Open Source](https://img.shields.io/github/last-commit/grigory-lobkov/rtsp-camera-view.svg?style=flat-square)](https://github.com/grigory-lobkov/rtsp-camera-view) 
[![Pro](https://img.shields.io/github/license/grigory-lobkov/rtsp-camera-view.svg?style=flat-square)](https://github.com/grigory-lobkov/rtsp-camera-view/blob/master/LICENSE)

Monitoring of IP-cameras, view any streaming video sources in the grid mode

Release &nbsp; &nbsp; &nbsp; [![GitHub release](https://img.shields.io/github/release/grigory-lobkov/rtsp-camera-view.svg?style=flat-square)](https://github.com/grigory-lobkov/rtsp-camera-view/releases) 
[![Github Releases](https://img.shields.io/github/downloads-pre/grigory-lobkov/rtsp-camera-view/latest/total.svg?style=flat-square)](https://github.com/grigory-lobkov/rtsp-camera-view/releases)

Beta &nbsp; &nbsp; &nbsp; &nbsp; [![GitHub (pre-)release](https://img.shields.io/github/release/grigory-lobkov/rtsp-camera-view/all.svg?style=flat-square)](https://github.com/grigory-lobkov/rtsp-camera-view/releases) 
[![Github Releases](https://img.shields.io/github/downloads/grigory-lobkov/rtsp-camera-view/latest/total.svg?style=flat-square)](https://github.com/grigory-lobkov/rtsp-camera-view/releases)

If you using it, please, put your [Issue here](https://github.com/grigory-lobkov/rtsp-camera-view/issues)

![](https://user-images.githubusercontent.com/36440722/39676355-b801a8b2-5182-11e8-9d37-1002c36ac873.jpg)



## Table of contents

- [Installation](#installation)
- [Contributing](#contributing)
- [Supported formats](#supported-formats)
- [Supported languages](#supported-languages)
- [Features](#features)
- [Overview](#overview)
- [Contributors](#contributors)
- [Copyright and license](#copyright-and-license)



## Installation
Dependencies
- Windows XP or higher
- .NET Framework 4.0 or higher
- VLC 2.1.3 / 2.1.5

Download executable from [Releases](https://github.com/grigory-lobkov/rtsp-camera-view/releases) and unpack

You have to know url of RTSP stream to your cameras, to add them to camera list


## Contributing
All contributions are more than welcomed. Contributions may close an issue, fix a bug (reported or not reported), improve the existing code, localize, add new feature, and so on.



## Supported formats
- UDP/RTP Unicast, UDP/RTP Multicast, HTTP / FTP, TCP/RTP Unicast, DCCP/RTP Unicast
- any video for fun: file:////Movies/Shrek.mkv



## Supported languages
- English
- Russian



## Features
- expanding the entire window by double-clicking on the stream
- automatic switching to high / low resolution stream
- support for command line parameters
- launching on the screen with the specified number, full-screen'ed
- customizable source name
- alert on video lost


## Overview
[Screenshots, examples](https://github.com/grigory-lobkov/rtsp-camera-view/wiki/Overview)



## Contributors

Special thanks to everyone who contributed to getting the RTSP Camera View to the current state.

- [Gregory Lobkov](https://github.com/grigory-lobkov) - idea, programming, testing, design, etc



## Copyright and license

Code and documentation copyright 2018 [Gregory Lobkov](https://github.com/grigory-lobkov). Code released under the [Apache License 2.0](https://github.com/grigory-lobkov/rtsp-camera-view/blob/master/LICENSE).
