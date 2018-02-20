# rfcx-guardian-android

## Guide for instalation

1. Install the four aplications: guardian, updater, setup and admin using gradle (gradle 2.2) or building them with android studio
2. Ensure to have fb2png executable in android device in the route /data/data/org.rfcx.guardian.admin/files/screenshot/bin/ , if not download from https://github.com/cybertk/android-fb2png and follow the instructions
3. Even C and C++ executables are in the repository, if you have some issue, build them with ndk, for that install ndk , and run ndk-build in the folder rfcx-guardian-lib-audio\jni 

If you have some issue , let us know it.


# Bosque protector servicios

These proyect have the objective to contain all the new functionalities added by ESPOL's people.

## Module SendingAudio

These module is to send the audios that are in the phone to the server located in ESPOL. For these we used a service named SendingAudioService that used 
OkHTTP library to communicate with the server. Also there is a broadcast receiver that initialize the service at boot.

Also there is an app which function is to modify some feautures of the service


* NumberOfIntents

number of intents in which each audio is try to upload to the server

* SendingAudioTime

Time between the service is "restarted"

* IsOnService

Switch to desactivate or activate the service

* OnDestroyAudio

Switch to delete the audios , if they are send correctly to the server
