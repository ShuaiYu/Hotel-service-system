# Hotel-service-system
Hotel Internet Service System
Introduction and goals
Structure and Algorithm
code
Introduction and goals
This is a Hotel Internet Service System. It is a Soft Defined Network(SDN) application. POX controller is applied in this application. It is tested on a topology which is built by mininet. The application aims to build a charge system. Only paid hosts can access to the internet and they can also access to some intern resources.

2. Structure and Algorithm
Topology of this system is shown in Figure 1. There is a POX controller and several hosts. Host 1(h1) is regarded as a sever the rest are clients.

Figure 1

The flow diagram is represented as Figure 2. When a custom come to the reception and check in. He or she will get a room number, a password to the internet, which is a random number created by controller and stored in a csv file named by the room number, and how long the customer can access to the internet, if the customer pay for the internet. When the customer try to access to the internet, the customer first type in the password, if it matches with the room csv file, the controller will get the computer`s mac address and store it into a mac address csv file. Only hosts with addresses in this file are able to access to the internet. If the password does not match do nothing.At the same time,timer will record the time, when time out, room number csv will be deleted and the computer`s mac address will be deleted in the mac address csv file.

Figure 2
