# RFCX ESPOL Web Server
Web Server for saving audio files from [RFCX devices](rfcx-devices.md) and make them ready for streaming and offline analysis. It has a MVC design.

## Responsibilities
- Receive compressed audio files as gzip files from [RFCX devices](rfcx-devices.md).
- Decompress received gzip files.
- Convert decompressed audio files to ogg format for [streaming](rfcx-espol-stream-server.md).
- Let users download saved audio files between desired dates.

## Repository Organization
* rfcx-espol-server
** RfcxServer
*** Icecast
*** WebApplication
*** config.sh
*** deploy.sh
*** deps.sh

## Development
This server is developed using multiplatform tools, which allow development and deployment for Windows, Linux and Mac OS. 

### Used Technologies
- [.Net Core 2.0.0](https://dotnet.github.io/), multiplatform core for .Net development.
- [ASP.Net core](https://docs.microsoft.com/en-us/aspnet/core/), for its reduced API compared with ASP.Net and better open source technologies integration. We use the MVC web application development facilities.
- [Visual Studio Code](https://code.visualstudio.com/), modern editor with valuable multiplatform debugging capabilities.
- [Microsoft.Orleans](https://dotnet.github.io/orleans/), is a Virtual Actor Model Framework for distributed systems. We have not used this yet, but we look at it for future due to the increasing popularity of Actor Model to develop IoT and distributed systems.
- [FFmpeg](https://www.ffmpeg.org/), used to convert saved audio files to desired format.

## Deployment
Currently, we have just tested deployment to Ubuntu 16.04 and we have developed a set of shell scripts to helps us with the task. The process to deploy server is described below.

### How to deploy RFCX ESPOL Web Server?
The Web and Stream servers are deployed at same time using the following steps:

- Run deps.sh
- Edit config.sh file modifying its declared variables.
- Run deploy.sh

This will install necessary software and set an automatic restart linux service.

### Deployed Folder Organization
