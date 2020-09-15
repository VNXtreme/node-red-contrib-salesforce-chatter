node-red-contrib-force
========================

A processing node of <a href="http://nodered.org" target="_new">Node-RED</a> nodes for <a href="http://www.salesforce.com/" target="_new">Salesforce Chatter</a>.

[![NPM](https://nodei.co/npm/node-red-contrib-force.png?downloads=true)](https://nodei.co/npm/node-red-contrib-force/)

Pre-requisites
-------

The node-red-contrib-force requires <a href="http://nodered.org" target="_new">Node-RED</a> to be installed.


Install
-------

Run the following command in the root directory of your Node-RED install

    npm install node-red-contrib-salesforce-chatter

Restart your Node-RED instance, the force node appears in the palette and ready for use.


Overview
-------

node-red-contrib-force contains the following modules.

#### force chatter content node

Post a message to Chatter. The message to be posted is set in `msg.payload` using the following structure:
`msg.payload = [
      {
            text: "This is the message 1",
            mention: "chatty.00d2w000009yf8ueaw.9wfk1pviifmg@chatter.salesforce.com"
      },
      {
            text: "Message 2 without mentioning"
      }
];`

You can also post image which is set in `msg.binaryBuffer` and `msg.filename`.


**Tip**： For more information on connected apps, see [Create a Connected App](https://help.salesforce.com/articleView?id=connected_app_create.htm) in the Salesforce Help.


Acknowledgements
----------------

The node-red-contrib-salesforce-chatter uses the following open source software:

- [JSforce] (https://github.com/jsforce/jsforce): Salesforce API Library for JavaScript applications.
- [Requet] (https://github.com/request/request): Simplified HTTP request client.
- [force-node] (https://github.com/joeartsea/node-red-contrib-force): A collection of Node-RED nodes for Salesforce/force.com.
