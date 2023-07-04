** Real-Time Rain Monitoring using Communication Satellites **

In communication satellite systems, satellite operators monitor the connection to each of their satellite dishes (internet users everywhere on Earth) in real-time. 
This parameter is the carrier-tonoise (C/N) ratio which can be understood as the signal-to-noise ratio and is measured in dB. 
In case of rain above the terminal, the signal drops and there is a clear correlation between the amount of signal drops and the rain intensity. 
As the signal is almost only impacted by rain it can be used as a virtual rain sensor. 
More precisely, it can be seen as a point measurement of rain at the location of the satellite dish. 
Combining many of these rain point measurement allows for creating rain maps for a full region with e.g. 1km x 1km spatial resolution.

Tasks

Attached you can find 2 C/N data samples from one satellite dish. For several months and for every 5 minutes you can find the time stamp, the C/N value (“FWD C/N”) and the actual rain intensity in mm/h (“rain_intensity_rg”) as measured by a rain gauge located in close proximity to the satellite dish. If the rain is very strong, the satellite dish sometimes experiences an outage in which case there is no C/N reported.

The task is to develop an algorithm that extracts rain intensity information from the C/N signal. In order to estimate the rain at any time stamp, the 2 hour history of C/N values can be used. But as it is a real-time product no future C/N values can be used.

