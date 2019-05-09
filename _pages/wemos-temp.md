---
permalink: /projects/wemos-temp
layout: single
---

This project was started by my desire to find out what the actual temperatures were for my baseboard heaters at the "Low - Med - High" settings.

Initially I was measuring at a location with a power outlet so I was able to just use a USB adapter for power. The second location I wanted to monitor was a utility closet in my garage that didn't have an outlet so I needed to come up with another option. I knew that the WeMos module had sleep modes but it wasn't something that I had ever implemented before.

In my case I was going to be running on batteries so I wanted an absolute minimum of power consumption while the WeMos was idle. The deep sleep mode was perfect as I didn't need any sort of wifi or CPU function other than a wake up trigger from the real time clock (RTC). This is amazingly simple in code:

`ESP.deepSleep(sleep_delay * 1000000); // microseconds`

On the hardware side all I needed to do was connect pin D0 to RST. The RTC sends a pulse on D0 when the timer expires and triggers a reset of the controller. At that point it starts the normal boot cycle and runs any code as usual. For this project I set it up to connect to wifi, take a temperature reading, send it to the server, and then go back to sleep for another 15 minutes.
