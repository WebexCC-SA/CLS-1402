# Overview

## Learning Objectives

This lab will give you an introduction to Remote Access and other related features that will help you leverage RoomOS troubleshooting and support capabilities for a seamless experience when managing devices in distributed and scaled deployments.

Our goals are:

- Learn how to leverage Remote Access
- Configure and support RoomOS and MTR devices
- Reduce in-room presence for support
- Learn how to visually verify issues virtually
- Fix issues remotely
- Verify customizations remotely
- What other tools can be leveraged in your troubleshooting journey
- Learn the limitations of Remote Access and how to bridge the gap


## Disclaimer

Although the lab design and configuration examples could be used as a reference, for design related questions please contact your representative at Cisco, or a Cisco partner.
The guidelines and documentation for the feature can be found here: [Remote access to Board, Desk, and Room Series devices](https://help.webex.com/en-us/article/gge81eb/Remote-access-to-Board,-Desk,-and-Room-Series-devices).


## Control Hub Access (TODO)

TODO: Find a way to give the users access to Control Hub individually.

First you need to know your session id and DNS name of your session.
From that you will get your login and password after the for Control Hub at https://admin.webex.com.

## Guides

Here is a list of guides you can follow throughout the lab:

- ### [Enable Remote Access for your company via Control Hub](./guides.md)
- ### [Access Local Device Controls from Control Hub](./guides.md)


## Limitations

Before starting lets go over the scenarios where Remote Access is not supported currently:

- If the device is in a call or a meeting or if the device joins one. If a call starts, the remote access session closes with a notification on the device with a reason why it was closed. Administrators controlling the device are also notified.

- Devices set up in personal mode

- The companion device in companion mode. The main device in a companion mode setup is supported.

- Room Navigators in standalone mode

- Room Bar BYOD devices

- A hot-desking device is in an active session, as the device is considered to be in personal mode.

- Running the first time wizard. The device needs to be registered to the Webex cloud first before a remote access session can be started.

- A wireless share is started from the Webex App to the device. If a wireless share is started on the device, the remote access session closes with a notification on the device with a reason why it was closed. Administrators controlling the device are also notified.

- Other types of wireless share work with remote access, such as AirPlay and Miracast.


## Lets get started

If you are ready lets start at [Hello Remote Access](./scenarios/helloRemoteAccess.md).