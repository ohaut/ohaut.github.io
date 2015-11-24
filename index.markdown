---
layout: post
---


## Introduction

The Opensource Home Automation project puts together the building blocks
for home automation based on the very affordable ESP8266 system on chip,
providing WiFi and MQTT/IP connectivity.

Every single project is released in source format, including CAD files
which are developed in the [KiCad][kicad] format and the software in
C++ based on the [ESP8266 Arduino][esp8266_arduino] environment.

[kicad]:          http://www.kicad-pcb.org
[esp8266_arduino]: https://github.com/esp8266/Arduino

## Photon project
The [photon project][photon_url] is the first project to be released.
It's a 3 Channel LED dimmer, capable of sustaining up to 5 to 48V
with 2A to 5A per channel. (Real specs still to be determined)

[photon_url]: http://github.com/ohaut/photon

<!-- ## Video

<iframe src="//player.vimeo.com/video/....." width="800" height="469"
frameborder="0" webkitallowfullscreen mozallowfullscreen
allowfullscreen></iframe> -->

## Public statement about OSHW

We will also try to put together open hardware in collaboration with
manufacturers, so the devices are readily available for purchase somewhere.
If you are a manufacturer or a reseller, please feel free to ping us, we will
provide a link to your shop.

If you want to manufacture the devices, and you need help, please feel free
to ping us too.

## Getting started

### Get a preassembled board
Ok, this is the easy way :)

### Assemble one yourself
* buy bare PCBs or order a few from gerbers
* buy the components from the bill of materials
* solder the components
* bring up the board, check voltages, etc.
* program initial firmware from the Arduino environment or esptool

## Development

### Tools
* CAD: [KiCad project][kicad]
* Arduino: [ESP8266 Arduino][esp8266_arduino]

<div class="home">
  <br/>
  <h1>Posts</h1>

  <ul class="posts">
    {% for post in site.posts %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{
post.title }}</a>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend:
site.baseurl }}">via RSS</a></p>

</div>
