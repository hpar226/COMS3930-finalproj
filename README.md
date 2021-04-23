# COMS3930-finalproj

<h3>Background:</h3>
Introducing The Bird Box! This is a bird feeder cam, it has an ESP32-CAM that takes pictures of birds looking for grub. It is powered via a 5v power supply and 1 li-po battery, and utilizes a motion sensor detector to trigger the camera.

This was a fun project because it brought forth a set of unexpected challenges that were satisfying to solve, such as:
<ul>
 	<li>figuring out where and how to mount the components to the birdhouse</li>
 	<li>setting up the wiring so that things can be easily taken apart for things such as accessing the memory card storing the photos and changing the li-po battery when needed. Also used thumbtacks to mount containers for easy removal.</li>
 	<li>learn new way to load data on an ESP32-CAM that does not use a direct USB-port input. I had to purchase an FTDI programmer to interface with the ESP32-CAM via GPIO pins and a mini-USB port. The mini-USB port, eg. not a micro-USB, made me turn my house upside down looking for a 15 year old cable (PS3 controller charger ftw!)</li>
 	<li>since the ESP32-CAM would be enclosed in a box, I needed a way to know whether the camera was being activated. I setup an external LED light to turn on when the camera takes a photo.</li>
 	<li>the enclosure being outdoors creates a set of challenges for waterproofing and bird-poop proofing (probably, I am guessing).</li>
</ul>
Disclaimer: I am a complete bird noobie, I do not know anything about birds and this is the first time I've dabbled with anything "bird" related.

Disclaimer 2: I had the bird feeder up for 2 days, but unfortunately, I was not able to capture an image of a bird on the bird-feeder. I am not sure if this is due to bad placement of the feeder, perhaps the components did not make the feeder attractive, or just needed more time to be out in the wild.
<h3>Materials:</h3>
<ul>
 	<li>birdhouse / birdseed - purchased from Home Depot</li>
 	<li>1 ESP32-CAM</li>
 	<li>4 plastic container boxes</li>
 	<li>jumper wires</li>
 	<li>FTDI programmer</li>
 	<li>infrared motion sensor</li>
 	<li>1 red LED</li>
 	<li>1 220 ohm resistor</li>
 	<li>1 li-po battery</li>
 	<li>1 5V power supply</li>
 	<li>8 thumbtacks</li
  
  <h3>Troubleshooting / Issues:</h3>
My initial plan was to create a Twitter page and have photos of birds posted to it automatically. I was not able to get that far because I realized I would actually need pictures of birds to post and I did not have the time to get reliable photos of birds to even attempt this.

The 5v power supply to the motion detector could've been substituted with a battery, but I did not have enough pins on the ESP32-CAM to power another device through it. The ESP32-CAM itself was rather cumbersome to work with, not having a dedicated USB interface for uploading code like the dev board made life harder dealing with wires all the time. I liked working with the Freenove dev board much better than the ESP32-CAM.

Again, placement of the feeder is probably important and being a bird noob does not help. Was a fun project to do nonetheless!
