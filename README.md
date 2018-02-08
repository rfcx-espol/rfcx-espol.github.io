# RFCX ESPOL

## Introduction
RFCX Espol is based on the work of [Rainforest Connection](https://rfcx.org/) which purpose is to provide acoustic monitoring systems for those who wish to end illegal deforestation in real-time. Our main contibution is to enhance the experience of accessing this real-time acoustic data, and looking forward to expand the range of metrics that can be transmitted through the monitoring system.

Behind our efforts are:
 - [ESPOL University](www.espol.edu.ec): Provides the student-developers the environment and tools to implement the system, while applying and reinforcing the knowledge acquired in the classrooms.
 - [Bosque Protector La Prosperina](http://www.bosqueprotector.espol.edu.ec/): Is a non-profit organization that manages the forest in which the system will be deployed
 - [Telefonica](http://fundaciontelefonica.com.ec/): Given its interest in environmental preservation projects, it will provide telecommunication resources through an association with ESPOL. eg: recicled cellphones, free mobile data transmition, etc.
 
## Description
The system is composed by the following modules
 - RFCX devices
 - Web server
 - Stream server
 - Unity WebGL application

## Architecture
The following image describes the relations and communication paths between the system's modules and users.

![architecture](/img/RFCX-ESPOL%20Architecture.jpg "Architecture")


## Modules

[RFCX ESPOL Module](rfcx-espol-block.md)

[Bosque Protector Module](bosque-protector-block.md)
