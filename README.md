## Introduction
RFCX Espol is based on the work of [Rainforest Connection](https://rfcx.org/) which purpose is to provide acoustic monitoring systems for those who wish to end illegal deforestation in real-time. Our main contibution is to enhance the experience of accessing this real-time acoustic data, and looking forward to expand the range of metrics that can be transmitted through the monitoring system.

Behind our efforts are:
 - [ESPOL University](www.espol.edu.ec): Provides the student-developers the environment and tools to implement the system, while applying and reinforcing the knowledge acquired in the classrooms.
 - [Bosque Protector La Prosperina](http://www.bosqueprotector.espol.edu.ec/): Is a non-profit organization that manages the forest in which the system will be deployed
 - [Telefonica](http://fundaciontelefonica.com.ec/): Given its interest in environmental preservation projects, it will provide telecommunication resources through an association with ESPOL. eg: recycled cellphones, free mobile data transmition, etc.
 
## Description
The system is composed by the following modules:
 - [RFCX devices](rfcx-devices.md), the same used by [Rainforest Connection](https://rfcx.org/)
 - [Web server](rfcx-espol-web-server.md), is responsible to receive, pre-process and serve data of available devices.
 - [Stream server](rfcx-espol-stream-server.md), streams audio data from Web Server to Unity WebGL Visualizer.
 - [Unity WebGL Visualizer](rfcx-espol-visualizer.md), a 3D interactive representation of the forest.
 
 And it is developed with the following users in mind:
 - Children who can navigate the forest and feel the real-time status of it.
 - Biologists and scientists who want to download raw data for further analysis.
 - Everybody who wants to monitor the forest.

## Architecture
The following image describes the relations and communication paths between the system's modules and users.

![architecture](/img/RFCX-ESPOL%20Architecture.jpg "Architecture")
