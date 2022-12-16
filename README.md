# IoT-Project
Documentation/README for my IoT-Project (no code involved)

## About The Project:
This Project demonstrates how to use Microsoft Azure IoT-Hub to create a IoT-system.
It collects data from a sensor simulator, stores data in a blob-container and visualizes the data in PowerBi.


## Resources used:
- Raspberry Pi Azure IoT Online Simulator
- Azure IoT-Hub
- Azure Storage Container
- Azure Stream Analytics Job
- Power Bi


## Step by step setup:

1. First i created and configured up my own Azure IoT-Hub, in Azure Portal. This Hub would later controll my Device, endpoints and routes for incoming Data.

2. Then i created an Azure device in my IoT-Hub, wich would be used to recieve data-messages in the future.
   I choose to use "Raspberry Pi Azure IoT Online Simulator" from Azure as Datasource/Sensor.
   I configured the code for the Raspberry Pi so it would send data-messages to my IoT-Hub Device.

3. Then I created a Storage Account in Azure Portal, in the account I created a blob-container to store data.
   After some configurations I tried to send data-messages in JSON format to my device, wich would store incoming data inside the blob-container.
   It worked!

4. After this I configured up a "Stream Analytics Job" in the Azure Portal. 
   This would then stream Data from my blob-container, to a Dataset wich I created in my Power Bi Account.

5. In the end I created a Power Bi report wich "subscribes" to the Dataset I created before, and visualizes the Data in a Power Bi graph.


## Overview of Project setup:

<br>
<img src="https://github.com/Danken1337/IoT-Project/blob/main/projectOverview.png"/>
<br>


## Results:
<br>
<img src="https://github.com/Danken1337/IoT-Project/blob/main/visualize.png" width="800"/>
<br>


