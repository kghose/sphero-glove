# Sphero Glove
Control the sphero with the ESP32's hall effect sensor

# Background

I was a little disappointed to gradually discover that "programming" the Sphero SPRK+ 
meant running a program on an App (or the browser) that took in sensor data from
the Sphero and sent back motor and LED commands to the Sphero. I was hoping that the
Sphero could run autonomously, like a microcontroller you could download code into.

As a next best thing, I wanted to learn how to directly interface with the Sphero SPRK+ 
instead of via the App. From [this post][1] it seems that Sphero control is via bluetooth.
Interesting: I have an ESP32 lying around that has bluetooth.

[1]: http://richardhayler.blogspot.com/2015/06/controlling-sphero-with-astro-pi.html

In that article the author controls the Sphero from a device that has an accelerometer
and uses tilting to control the Sphero.

I began searching for whether the ESP32 has an onboard sensor when I ran into [this post][2]
that taught me the ESP32 dev boards have a hall effect sensor and capacitive rouch sensors
and in a flash the idea came to me:

A control glove throw back that will control the Sphero SPRK+ movement.

[2]: https://www.etechnophiles.com/controlling-esp32-touch-sensor-and-hall-effect-sensor/

Let's see where this goes.
