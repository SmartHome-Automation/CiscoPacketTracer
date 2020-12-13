# CiscoPacketTracer - Smart Home Automation
Data Communication and Computer Networks Project on smart home automation with Cisco Packet Tracer
<img src="https://github.com/SmartHome-Automation/CiscoPacketTracer/blob/main/Logo%20%26%20pics/Automating%20engines%20pic.gif" width="50%"></img>
## Automating the smart home via network wifi.
- One can control & protect his home from intruder & sudden happenings such as fire etc.
- Control IoT devices remotely and smoothly
- the .pka file gives you immense options to explore Cisco Packet Tracer software's specifications and features.
- using the Simulator, we could identify every small detail about the network.

Designing Smart Home using IoT Devices. With the automation and collaboration the devices in our home becomes smarter. It makes our life become comfortable and convinent.

### Steps of connecting Devices and parts of home/office:
- **HOME GATEWAY** : Control point of other IoT Devices.
- **Living Room** : Ceiling Fan & Window
Wireless connection is established between Living room devices and Home Gateway.
In the I/O config tab, Network Adapter is set to Wireless Card.
- **SMART PHONE** : Smart phone is connected to Home Gateway by Wireless0 Connection keeping the same SSID = `HomeGateway`. Using `IOE Monitor App`, to access the Home Gateway with our mobile by keeping the same IP address.
Register all devices to Home Gateway by choosing the `config` tab and `IoT Server` as Home Gateway.

##### The devices are registered in Home Gateway and controlled via the Desktop IoE monitor. Fan Speed speed can be controlled. Window can be opened and closed.


## Packet Tracer – Home IoT Implementation
Scenario

In this Packet Tracer scenario, Bob has begun to implement an IoT solution in his home. You will explore the variety of devices and manipulate environmental factors to see the impact on sensors and actuators. You will also configure some basic settings, including IP addressing for a sensor, and security settings for the gateway router. Finally, you will verify that all the devices in the home have IP connectivity.

### Part 1: Connecting Devices to the Home Gateway
#### Step 1: Configure Home Gateway.

a.     Click Home to expand the cluster.

b.    Click Home Gateway. Click Config tab.

c.     Click Internet. Select DHCP for IP Configuration.

d.    Click Wireless. Enter MyHomeGateway as the SSID. Select WPA2-PSK as the authentication. Enter CiscoIoT as the PSK Pass Phrase.

e.     Click Home PC. Click Desktop. Click IP Configuration. Select DHCP for IP Configuration.

#### Step 2: Verify Home Gateway connectivity to registration server.

a.     From Home PC, enter www.register.pka in the Web Browser. Enter admin as the Username and admin as the Password to log in to the remote registration server.

Note: It may take a few minutes for all the IoT devices to be listed.

List some of the IoT devices:

What are some available actions for these IoT devices?

b.    From Home PC, enter 192.168.25.1 in the Web Browser. Enter admin as the Username and admin as the Password to log into the local IoT server hosted on Home Gateway.

List some of the IoT devices:

What are some available actions for these IoT devices?

### Part 2: Interacting with IoT Devices

#### Step 1: Automate temperature control.

Currently the Thermostat is off. Set the Thermostat to automatically adjust to the desired setting.

a.     Expand the Thermostat status bar. Click Auto. Enter the desired auto heating and auto cooling temperatures and click Set.

b.    Observe the Heating Element and Cooling Element as they adjust the temperature.

#### Step 2: Automate the Ceiling Fan.

The Ceiling Fan is configured to turn on only when motion is detected and no wind detected. The SBC0 with the use of motion and wind sensors controls the status of the ceiling fan.

Alt + Click the Motion Sensor near the Ceiling Fan. This will activate the Motion Sensor.

Did the Ceiling Fan turn on?

#### Step 3: Automate Lawn Sprinklers.

Watering the lawn could be an activity controlled through conditional statements configured in the local IoT server on Home Gateway.

a.     Expand the status for Lawn Sprinkler, Lawn Sprinkler0, and Water Level Monitor. Observe the relationship between the water level and the status of the lawn sprinklers.

What condition triggers the lawn sprinklers to turn on?

What condition triggers the lawn sprinklers to turn off?

b.    Click Conditions at the top of the webpage. Locate the conditional statements.

How many conditional statements control the lawn sprinklers?

#### Step 4: Automate Web Camera.

The Web Camera is currently configured to only turn on when the Motion Detector is triggered.

a.     Expand the status for Motion Detector and Web Camera. Observe the relationship between the Motion Detector and the status of the Web Camera.

b.    Alt + Click Motion Detector in the topology. Make sure to click the one near the Webcam.

What did you see on Webcam in the webpage?

#### Step 5: Open Windows and Garage Door.

An old car is being repaired in the garage. A CO detector, garage door, and windows have been installed and configured to prevent CO poisoning.

a.     Expand the status for all the windows, Garage Door, and the Garage CO Detector. Are any devices missing from the list?

b.    For the unconnected device, verify that it is configured to connect to the Home Gateway for the IoE Server, and that DHCP is enabled for the IP Configuration settings.

c.     Start the old car by Alt + Click the Car in the garage and watch the CO level rise in the garage.

d.    Alt + Click the Car to turn off the old car.

e.     Observe how the windows and garage door interact with the CO level in the garage.

#### Step 6: Fire suppression

An IoT fire suppression system has been installed in each of the bedrooms and the kitchen. In this IoT demonstration, there will be a simulated fire while you are away from home, and you can observe how the fire suppression operates using the status of the smoke detectors.

a.     Exit the Home cluster by clicking Back. Click the ISP-Internet cluster to enter it.

b.    From Smartphone, enter www.register.pka in the Web Browser. Enter admin as the Username and admin as the Password to log in to the local IoT server hosted on Registration Server.

Note: It may take a few tries before the web page displays.

c.     Expand all the statuses for the smoke detectors. Are any devices missing from the list?

d.    Simulate a fire in the kitchen. What happens to the smoke detectors?

Describe what happens next.

e.     Start a simulated fire in other locations to observe what happens.

#### Step 7: Further investigation

a.     In the previous step, you observed that Home Gateway and Registration Server can be used to control the IoT devices remotely. You can change how these devices are accessed remotely.

1)     Click the device.

2)     In the Device tab, select None, Home Gateway, or Remote Server. For the activity, the server address is www.register.pka (209.165.201.10) and admin as username and password.

3)     Within the server, you can add conditional statements for devices capable of actionable configurations.

b.    If you are interested in programming the IoT end devices, click the device and click Advanced. Select Programming. Select the desired files and review the codes.
