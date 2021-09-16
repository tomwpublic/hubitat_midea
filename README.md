# hubitat_midea

This provides Thermostat driver capabilities for Hubitat with Midea branded and Midea-supplied air conditioning units.  Many common brands are supplied by Midea and are compatible with this integration.

This component is substantially based on and is mostly a direct port of this excellent work: https://github.com/mac-zhou/midea-msmart

Special thanks to ghgeiger and etienne from the Hubitat forums for their testing and troubleshooting help.

# Manual Installation instructions:
* In the *Drivers Code* section of Hubitat, add the mideaAC_localController driver.

# Configuration instructions:
* Follow the instructions on this page to install and execute the `midea-discover` utility: https://github.com/mac-zhou/midea-msmart/blob/master/README.md
    * Note that this requires a separate computer running Python3 and can not be run directly from Hubitat.  This is a one-time configuration step.
    * Sample Output:
    * ![Alt text](docs/sampleOutput.png?raw=true "midea-discover output")

* In the *Devices* section of Hubitat, add a *New Virtual Device* of type Midea AC local controller.
* On the configuration page for the newly created *Device*, enter the token, key, and device id from `midea-discover`, along with the IP address and port of your Midea AC unit.
* Indicate whether you plan to use Celsius or Fahrenheit for your temperature setpoints and temperature reporting.  


# Usage instructions:

* Utilize the various commands to control your AC unit.

# Disclaimer

I have no affiliation with any of the companies mentioned in this readme or in the code.
