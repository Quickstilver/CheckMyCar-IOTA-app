# CheckMyCar-IOTA-app
Copyright Stefano Balla, Federica La Piana

A IOTA APPLICATION

A System (sender-receiver, scalable) for monitoring the car by the sensors. It is based on MAM messages and IPFS. The simulated Car ( HIGH MOBILITY) sends the file with sensed data to IPFS, then retrieve the CID from IPFS. So the Car sends the CID and the sha256 of the file to the USER/ RECEIVER using MAM trough the Iota TANGLE. 
The Receiver receives the CID and the sha256, with the first it can download the file from IPFS and then control the integrity using the sha256.
In addition, with the Web app you can monitor all the sensed data AND send MIOTA to the MECHANICAL in case of maintainance.


-Create a simulated car on HIGH MOBILITY.

-Activate all the sensors.

-Copy And Paste the API keys in infoServices.js.

-Execute SenderSingleRoot.js to retrieve an hash and then copy and paste the hash into appSingleRoot.js line 36 -> nextRoot= "paste here"

-Run Localhost 3000 to launch the app.

Car (SENDER) files:
- senderSingleRoot.js
- infoServices.js

web app (Receiver) files:
- appSingleRoot.js
- maintenanceServices.js
- pay.js
- errorhandling.js



