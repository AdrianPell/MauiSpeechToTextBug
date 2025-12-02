# Maui Community Toolkit - Speech to Text inconsistency

This repo contains a Maui Blazor Hybrid project to demonstrate inconsistency in the way that events from OfflineSpeechToTest are presented:
* On Android, each event includes the entire text which has been recognized
* On iOS, each event only includes new text recognized since the previous event

The difference in this behavior is unexpected since the basic expectation from the toolkit is that behavior is the same on all platforms.

## How to use

* Open the repo in Visual Studio 2026 with the MAUI workload installed, and connected to appropriate test devices for Android and iOS
* Build and deploy to an Android device
* Run by pressing the "Start Listening" button and speak into the microphone
* The display shows the various stages of recognition, with the whole text to date being displayed
* Repeat for iOS, showing only the incrementatal recognition text
