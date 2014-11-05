# Nest Device Type
http://build.smartthings.com/projects/smartnest/

Now SmartThings can talk to your Nest thermostat.

Note: this is technically against the Nest TOS. So use at your own risk.

## Installation

1. Create a new device type (https://graph.api.smartthings.com/ide/devices)
    * Name: Nest
    * Author: dianoga7@3dgo.net
    * Namespace: smartthings-users
    * Capabilities:
        * Polling
        * Relative Humidity Measurement
        * Thermostat
        * Temperature Measurement
		* Presence Sensor
		* Sensor
    * Custom Attributes:
        * temperatureUnit
    * Custom Commands:
        * away
        * present
        * setPresence
        * heatingSetpointUp
        * heatingSetpointDown
        * coolingSetpointUp
        * coolingSetpointDown
        * setFahrenheit
        * setCelsius

1. Publish the device type (next to Save button) > For Me

1. If you want to switch from slider controls to buttons, comment out the slider details line and uncomment the button details line.

1. Create a new device (https://graph.api.smartthings.com/device/list)
    * Name: Your Choice
    * Device Network Id: Your Choice
    * Type: Nest (should be the last option)
    * Location: Choose the correct location
    * Hub/Group: Leave blank

1. Update device preferences
    * Click on the new device to see the details.
    * Click the edit button next to Preferences
    * Fill in your information.
    * To find your serial number, login to http://home.nest.com. Click on the thermostat you want to control. Under settings, go to Technical Info. Your serial number is the second item.

1. That's it, you're done.
