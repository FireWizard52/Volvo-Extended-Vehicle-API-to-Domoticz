# Volvo-Extended-Vehicle-API-to-Domoticz

1. Introduction.

This document describes the use of the Volvo Extended Vehicle API for use in Node Red and push the data to Domoticz.
However, you can omit the Domoticz part and implement an interface to any Home Automation System.

2. Create an account.

Before you are able to request the valid key and other needed credentials you have to create an account at:
https://developer.volvocars.com/account/

3. Obtain a valid VCC API Key and an User Access Token.

If you own a Volvo Car and have a valid subscription to Volvo on Call, you may get a User Access Token for your own car.

4. The Node Red flow contains two "Configuration" nodes.
In the first node (most left) you should insert the obtained VCC API Key and the User Access Token.
The second "Configuration" node is only for Domoticz users and may left untouched by others.
Domoticz user have to insert the Domoticz IDX number of their corresponding virtual sensor or switch.

5. Start the flow.
You can inject the timestamp in the "Inject" to start the flow.
Feel free to configure the "Inject"node to your desired values.

Note.

Currently the obtained User Access Token for both the Demo car, as well as your own car will expire after 1 hour.
In order to get a new token, you will have to log out and afterwards to log in again.

Non Domoticz users may safely delete the last "Function" node and the most right "Configuration" node.

Disclaimer.

This is work in progress and the Volvo Extended Vehicle API is still in beta, so may change in the future.
