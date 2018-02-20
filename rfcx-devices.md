# RFCX devices

Rfcx devices have two repositories: rfcx-guardian-android and Bosque protector servicios. 


## rfcx-guardian-android

This uses [Rain Forest technologies](https://rfcx.org/) to record the audio files from the device. It consists of four apks, that have to be installed simultaneously. Each have to be opened once , and then restart the phone, so each app can work correctly . The phone has to be rooted to make all work fine. A guide of instalation is provided below.

### Guide for instalation

1. Clone the [forked repository](https://github.com/rfcx-espol/rfcx-guardian-android)
2. Install the four aplications: guardian, updater, setup and admin using gradle (gradle 2.2) or building them with android studio
3. Ensure to have fb2png executable in android device in the route /data/data/org.rfcx.guardian.admin/files/screenshot/bin/ , if not download from [android fb2png repository](https://github.com/cybertk/android-fb2png) and follow the instructions
4. Even C and C++ executables are in the repository, if you have some issue, build them with ndk, for that install ndk , and run ndk-build in the folder rfcx-guardian-lib-audio\jni 


## Bosque protector servicios

These part of the devices proyect have the objective to contain all the new functionalities added by ESPOL's people.

### Module SendingAudio

These module is to send the audios that are in the phone to the server located in ESPOL. For this we used a service named SendingAudioService that use OkHTTP library to communicate with the server. Also there is a broadcast receiver that initialize the service at boot.

Also there is an app which function is to modify some feautures of the service


* NumberOfIntents

number of intents in which each audio is try to upload to the server

* SendingAudioTime

Time between the service is "restarted"

* IsOnService

Switch to desactivate or activate the service

* OnDestroyAudio

Switch to delete the audios , if they are send correctly to the server


If you have some issue , let us know it.
