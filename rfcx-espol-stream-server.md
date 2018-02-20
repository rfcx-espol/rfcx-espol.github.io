# RFCX ESPOL Stream Server
Stream Server used to listen audio captured by [RFCX devices](rfcx-devices.md) 

## Responsibilities
- Setup and mantain a stream service to stream .ogg files stored in [Web Server](rfcx-espol-web-server.md).
- Mantain streaming playlist for stream sources.
- Delete .ogg files based on creation date.

## Development
This server is developed using open source streaming tools and linux shell scripts to mantain the streaming playlists

### Used Technologies 
- [Icecast](https://icecast.org) as an http stream server. 
- [Ices](http://icecast.org/ices/), multiple instances as stream sources, feedeng the stream server through different channels.

## Deployment
Currently, we have just tested deployment to Ubuntu 16.04 and we have developed a set of shell scripts to helps us with the task. The process to deploy server is described below.

### How to deploy RFCX ESPOL Web Server?
The Web and Stream servers are deployed at same time using the following steps:

- Run deps.sh
- Edit config.sh file modifying its declared variables.
- Run deploy.sh

This will install necessary software and set an automatic restart linux service.
