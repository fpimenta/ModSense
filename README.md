# ModSense
### The LEGO power strip. We built it smart, modular and connected.

![Logo](https://github.com/JCacho/ModSense/blob/master/LOGO_ModSense.jpg)

## Inspiration
Have you never tried to plug your computer charger to the power strip but you didn't find any vacant space? Of course you have, because you don't have a ModSense power strip.
Do you at least know how much power you are wasting with your electronics when you are not using them? Well... we can also help you with that.

## What it does
**ModSense is a smart, modular and connected power strip**. You don't have to adjust to the product, the product adjusts to you. Add how many modules you need, to plug how many devices you want. All sockets have power measurement and can be turned on and off remotely, controlled in a web browser or by a mobile application. You can program your power strip to turn on/off the devices at a certain hour or under certain conditions ( e.g. the temperature in the room is above 25ºC, so you want to turn off the socket controlling the heater or if you shutdown your computer it can automatically turn off the peripherals). Because it is modular, each socket can have a different feature, like temperature sensing, air quality sensing, noise sensing or it can even act as a wifi repeater. All this data is sent to a server where it is accessible through a web browser and a mobile application where the communication works both ways. Also, because it's modular, we can have modules with different socket standards, e.g. in a restaurant, our strip could be used for tourists to charge their devices without the need for an adapter.

## How we built it
 - Designed a 3D model of a power socket that can be combined into a power strip by just adding more modules (like LEGO)
 - Assembled and coded an Arduino Nano for each socket with power consumption and temperature sensors
 - Used I2C protocol to connect each Slave Arduino Nano in each socket to the Master ESP8266 so information from the Slaves can be uploaded to the cloud
 - Connected the ESP8266 to a Heroku server to post the information retrieved from each arduino nano on the server so it could be acessed by an android application
 - Built an android application to present all sensors information to the user
 
## Challenges we ran into
 - Couldn't use Mains AC (the organization asked us not to) so we had to re-design all our circuits
 - No one had 3D modelling skills
 - Designing a plug system that was safe to use, even with the 230V AC (we did it, but we couldn't test it)

## Accomplishments that we're proud of
 - Finishing the prototype in time
 - Building something from scratch
 
## What we learned
 - How to use Autodesk Fusion 360 and Cura
 - How to integrate the ESP, the server and the mobile phone

## What's next for ModSense
 - Sleep
 - Actual testing using Mains power
 - Build more modules and add more functionalites
 - Re-make the design more compact

[Visit Us Here!](https://devpost.com/software/modsense-dzi6vx)
