# TTQM

I haven't updated the alpha 4 read me yet so this is sparse I will update this shortly with at least a new feature list.

This is a pre release 5 of alpha 5.   The code and the app user interface is still unfinished in parts but I would like your feedback on any issues you find. Especially red log 'ERROR' messages, java/groovy errors and 'null' errors. Orange log 'warn' are usually not 'problems' as such.  I will send you all an invite to a new Alpha 5 Pre topic on the HE community shortly.

Inparticular I would like you to test discovery from HA (using statestream) or from homie if you have that option.  Also setting up adhoc devices to import from MQTT.  I will post some notes about the latter here shortly.

NB Although HA and OH interoperability is included my main priority for alpha5 is to get HE<>MQTT complete and working well I will then spend some time on expanding HA connectivity (and also OH but I don't use that platform)

My virtual MQTT Dimmer and Switch drivers are now deprecated. Discovery should create devices using one of the built in virtual drivers and you can link any 'adhoc' MQTT device back to any HE Virtual Device Driver via the new Virtual MQTT Data config page (which is a bit finicky and slow at the moment).  Do not delete your existing devices using my drivers if you wish to keep them around to copy the MQTT data over. They will no longer work though.

There will not be an alpha 6 - - just any needed hotfixes to alpha 5 and then it will be released as public beta 1.

PLEASE DO NOT clone this repository until alpha 5 becomes a release version

This is still currently under the previous highly restrictive licence

NB :   Setup issues

1) I haven't verified that all atomicState and state variables are initialised correctly for new/update installs - you might see some error messages on lauch - please report

2) Under Configuration there is a new dropdown temporarily labeled "Please enable the first option Toggle All on/off - to select all devices*".  You need to do this now so the MQTT app can lookup device names using inbuilt drivers (as I no longer use my own drivers)

3) If HA Discovery doesn't run you might have to enable homie discovery with a random homie device name to allow HA to start (it's currently waiting for homie discovery to finish)

4) The devices discovered numbers are inconsistent and  'Startup Complete' summary shows up in the log well before HA and homie discovery have completed.

Getting there .. 
Kevin
