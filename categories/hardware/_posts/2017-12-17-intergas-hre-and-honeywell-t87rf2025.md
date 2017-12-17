---
layout: post
title: Intergas Kombi Kompakt HRE 24/18 and Honeywell T87RF2025
description: Finding a replacement for my Honeywell thermostat. Can I do it myself?
image: assets/img/RPI/thermostat_RT87RF2025.jpg
category: hardware
tags: RPI thermostat
---
The aim of this research is to find out it is possible to replace or enhance my [current wireless thermostat][honeywell-T87RF2025]{:target="_blank"}
. I know it works with RF and the heater has a build-in RF receiver. Probably they speak OpenTherm, however I'm not sure how its encoded over the RF signal. That seems to be the main problem for directly connecting to the heater. 

Another option is through an existing solution. As far as I know there are two options. First the [Incomfort of Intergas itself][incomfort]{:target="_blank"}. This is a `lan2rf` gateway which seems easy to install. Furthermore it is possible [connect it to Domoticz][incomfort-domoticz]{:target="_blank"} and [a plugin for pimatic is also available][incomfort-pimatic]{:target="_blank"}. For Domoticz, it is 'officially' supported [since version 3.8153][domoticz-releasenotes]{:target="_blank"}. This suggests that you can access it locally, there is some http access and thus app is not required. It does require an investment of just under €100. 

The other way to go may be the [Honeywell RFG100 gateway][honeywell-rfg100]{:target="_blank"}. I'm unsure how this works. It either connects to the thermostat or connects directly to the heater. There is description available for [connecting the RFG100 to Domoticz][ffg100-domoticz]{:target="_blank"}, however there are apparently some issues with setting values. Reading does seem work.

I'll probably buy the Incomfort unit and create my own interface. Although it may be time to check out Domoticz.


[incomfort]: http://www.intergas-verwarming.nl/consument/product/incomfort-2/
[incomfort-domoticz]: https://www.domoticz.com/forum/viewtopic.php?t=7745
[incomfort-pimatic]: https://pimatic.org/plugins/pimatic-intergasincomfort/
[honeywell-rfg100]: www.honeywelluk.com/Documents/Full-Specification/pdf/RFG100.pdf
[ffg100-domoticz]: https://www.domoticz.com/wiki/Evohome
[honeywell-T87RF2025]: https://products.ecc.emea.honeywell.com/europe/pdf/t87-y87-en0h8598-uk07r0516.pdf
[domoticz-releasenotes]: https://www.domoticz.com/forum/viewtopic.php?f=3&t=18597#p143437

