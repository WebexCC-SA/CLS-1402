## Scenario 4 - Start a call for the end user

## Problem

In this scenario you will start a call from remote access for the end user but they want continued support during the call. That is not a supported scenario for Remote Access so we will have to find ways to continue supporting the call using other tools from Webex.

## Your task

In this scenario what you will need to do is start a remote access session, and start a call on the device, after that the remote access session will stop since its not supported in call. From here you  have 2 options to continue to give support for the call, one is use the xAPI commands to continue giving support for the call, the other option is to use Local Device Control and log in to the Web Interface and give support for the call in the WebUI interface.

- To start a Remote Access session follow the instructions from [Hello Remote Access](./helloRemoteAccess.md).

### Option 1: Use the xAPI to continue giving support for the call

Use the xAPI to continue giving support for the call. You can do that by using the xAPI commands from https://roomos.cisco.com/xapi. You can execute them on Control Hub, over the Web Interface, or directly on the device. 

#### Using the xAPI commands on Control Hub

- To log in to Control Hub follow the instructions from [Logging into Control Hub](../guides.md). After that find your device and go to the devices page. You will wind an _Action_ button with the option of _Run XCommand_. From there you can run commands that will allow you to control the call. A list of relevant commands are described below.

#### Using the xAPI commands on Local Device Controls webpage

- To use Local Device Controls you need to be on the same network as the device.

- To log in to the Web Interface follow the instructions from [Access Local Device Controls from Control Hub](../guides.md). 

- Go to Developer API tab and run the commands

#### Here are a few xAPI commands you can run to control the call

Here are a few examples:

```
xCommand Call Disconnect
xCommand Presentation Start
xCommand Presentation Stop
xCommand Audio Microphones Mute
xCommand Audio Volume Decrease/Increase

``` 

More at https://roomos.cisco.com/xapi

### Option 2: Use Local Device Control to log in to the Web Interface and give support for the call tab in the Web Interface

- To log in to the Web Interface of the device follow the instructions from [Logging into the WebUI interface](../guides.md).

- Once logged in go to the Call tab. There you will have full control over the call on the interface and can do basic call functions, should look something like this:

![Call Controls Interface on the Device](./../assets/CallControlsInterfaceonWebInterface.png){ width="500" }

