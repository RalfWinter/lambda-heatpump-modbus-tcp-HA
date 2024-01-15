Last year I moved from a natural gas heating to a heatpump system from the Austrian company "Lambda" (https://lambda-wp.at). According to my personal market research they produce one of the most efficient air-water-heatpumps on the market (actually I have a COP of 5 for the winter season between November and February, which is great). I have to say that I run all heating circuits (also the radiator circuit) with the same low temperature for under floor heating, which is 40°C at outer temperatures of -10°C).

The heatpump controller talks VNC and MODBUS/tcp. VNC offers a nice graphical view, but Lambda requires a VPN constantly opened into my local network, I do not like this idea. Once you know the local VNC-password the VPN is no longer required, however, in order to have the data in Home Assistant and to be able to control the heatpump as soon as I have solar panels on my roof, convinced me to integrate the MODBUS registers of the heatpunp into HA.

I could not fully test all sensors because I have not all features installed which are described in Lambda's MODBUS specification (this can be downloaded from Lambda's website). The version of MODBUS specification I found at the time of writing the yaml file was dated April 11th, 2023.

Here is a quick view of a simple representation of the data in HA:
<picture>
  <img alt="Shows my dashboard for the Lambda-WP in HA" src="https://up.picr.de/46939285kg.png">
</picture>
