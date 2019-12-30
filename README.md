# TTQM

I haven't updated the alpha 4 read me yet so this is sparse I will update this shortly with at least a new feature list.

This is a pre release 5 of alpha 5.   The code and the app user interface is still unfinished in parts but I would like your feedback on any issues you find. Especially red log 'ERROR' messages and inparticular any code breaks - or null warnings. Warnings are usually not 'problems'.  I have sent you an invite to a new Alpha 5 Pre topic on the HE community.

NB Although HA and OH interoperability is included my main priority for alpha5 is to get HE<>MQTT complete and working well I will then spend some time on expanding HA connectivity (and also OH but I don't use that platform)

My virtual MQTT Dimmer and Switch drivers are now deprecated. Discovery should create devices using one of Hubitats built in drivers and you can link any 'adhoc' MQTT device back to any HE Virtual Device Driver via the new Virtual MQTT Data config page (which is a bit finicky and slow at the moment).  Do not delete your existing devices using my drivers if you wish to keep them around to copy the MQTT data over.

There will not be an alpha 6 - - just any needed hotfixes to alpha 5 and then it will be released as public beta 1.

PLEASE DO NOT clone this repository until alpha 5 becomes a release version

This is still currently under the previous highly restrictive licence

