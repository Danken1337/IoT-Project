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

## Overview of Project setup:


<img src="https://github.com/Danken1337/IoT-Project/blob/main/projectOverview.png"/>

```
+------------------------------+           +----------------+          +---------------------------+        +-----------------------+
| Datasource                   |           | Azure Deivce   |          | Azure IoT-Hub             |        | Azure Blob-Container  |
| RaspberryPi Sensor Simulator | --------> | Gets data from | <------> | Controlls Device, storage | -----> | Stores collected data |
| Sends data to device         |           | datasource     |          | and data stream           |        |                       |
+------------------------------+           +----------------+          +---------------------------+        +-----------------------+
                                                                                                                         |
                                                                                                                         |
                                                                                                                         |
                                                                                                            +----------------------------+
                                                                                                            | Azure Stream Analytics Job |     |
                                                                                                            | Strams Data to PowerBi     |       
                                                                                                            +----------------------------+
                                                                                                                         |
                                                                                                                         |
                                                                                                                         |
                                                                                                            +-----------------------+
                                                                                                            | Power Bi              |
                                                                                                            | Gets data from dataset|
                                                                                                            | Visualizes Data       |
                                                                                                            +-----------------------+

```
## Step by step setup:



## Results:

<img src="https://github.com/Danken1337/IoT-Project/blob/main/visualiseringIoTproject.png" width="800"/>



