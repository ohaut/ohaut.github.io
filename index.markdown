---
layout: post
---

## Introduction

The Opensource Home Automation project puts together the building blocks
for home automation based on the very affordable ESP8266 system on chip,
providing WiFi and MQTT/IP connectivity with optional integration to
[OpenHAB][openhab_url].

Every single project is released in source format, including CAD files
which are developed in the [KiCad][kicad] format and the software in
C++ based on the [ESP8266 Arduino][esp8266_arduino] environment. Updates
over the Air (wireless updates) just one click away in the Arduino IDE.

[kicad]:           http://www.kicad-pcb.org
[esp8266_arduino]: https://github.com/esp8266/Arduino
[openhab_url]:     http://www.openhab.org

## Ray project
The [ray project][ray_url] is the first project to be released.
It's a 3 Channel LED dimmer, capable of sustaining up to 5 to 48V
with 2A to 5A per channel. (Real specs still to be determined)

### Release 1.00B
* [schematics][ray_schematics]
* [gerbers][ray_gerbers]
* [bill of materials][ray_bom]

[ray_url]: http://github.com/ohaut/ray
[ray_schematics]: https://github.com/ohaut/ray/blob/master/hardware/microdimmer/pcb/releases/1.00B/schematics.pdf
[ray_gerbers]: https://raw.githubusercontent.com/ohaut/ray/master/hardware/microdimmer/pcb/releases/1.00B/gerbers.zip
[ray_bom]: https://raw.githubusercontent.com/ohaut/ray/master/hardware/microdimmer/pcb/releases/1.00B/bill-of-materials.csv

### Photon video
<iframe src="//player.vimeo.com/video/146833981" width="800" height="469"
frameborder="0" webkitallowfullscreen mozallowfullscreen
allowfullscreen></iframe>

## About Opensource Hardware

Trying to close the gap in opensource hardware, we will work with manufaturers
to build the boards and make them available in online shops.
If you are a manufacturer or a reseller, please feel free to ping us, we will
provide a link to your shop.

If you want to build the hardware yourself, you will have all the necessary
information available for every project.


## Getting started

### Get a preassembled board
Ok, this is the easy way :), from there you can use it, or modify the software
and upload via WiFi.

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
* Programming Cable: [banggood ft232rl][banggood_pgcable]

[banggood_pgcable]: http://www.banggood.com/FT232RL-FTDI-USB-To-TTL-Serial-Converter-Adapter-Module-For-Arduino-p-917226.html?p=6503002515035201509S

<div class="home">
  <br/>
  <h1>Posts</h1>

  <ul class="posts">
    {% for post in site.posts %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}
        </a>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
</div>
