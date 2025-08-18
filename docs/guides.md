# Guides

## Log in to Control Hub

To log into Control Hub navigate to [admin.webex.com](https://admin.webex.com) and log in with the email and password designated for you.

## Enable Remote Access for your company via Control Hub

To enable Remote Access feature in Control Hub for your company. Navigate to Device -> Settings in control hub, read the description of Remote Acces and toggle on Enable Remote Access.

![Remote Access](./assets/enableRemoteAccess.png){ width="500" }

You also have to option to enable/disable Remote Access per device, refer to the [documentation](https://help.webex.com/en-us/article/gge81eb/Remote-access-to-Board,-Desk,-and-Room-Series-devices) for that.

In case you want to activate it directly on a device using the xAPI the public xConfiguration that activated Remote Access is:

> xConfiguration RemoteAccess Mode: On/Off

## Access Local Device Controls from Control Hub

You should know that the local device controls, also known as the device's Web Interface can only be accessed from the same network as the device. 

To access the local device controls first you have to navigate to the device page after searching and finding it on the devices tab. Once you are in the devices page you can click on Launch on the Local Device Controls within the Support card as seen in the image below:

![Local Device Controls](./assets/SupportLocalDeviceControlsBlurred.png){ width="500" }

Press connect with hostname and you will have access to the Web Inteface of the device

![Cross Launch Device Controlls](./assets/CrossLaunch.png){ width="500" }

??? Note "Accept risks in case you are prompted"
    You are accessing a page hosted on the device, its safe to ignore the warnings from the browser and continue.

You will land on the home page of the Web Interface of the device ass seen in the image bellow:

Having access to this page opens up a series of options that will be usefull for us in this lab. Such as:

- Remote Access from the Web Interface. You can give it a try!
??? Note "Configuration NetworkServices Websocket: FollowHTTPService"
    Using remote access from the device's web interface requires that the configuration NetworkServices Websocket is set to FollowHTTPService.
- Developer API where you can execute xCommand and xConfiguration directly on the device. This can be useful in case you want to control a call with xcommands for instance.
- Macro Editor, where you can create your own macros in combination with UI Extensions. This will be useful for us in the integrator scenario where we will have to visit this page to fix our customizations.
- Call tab. This will be useful in the call scenario where we will have started a call from Remote Access. Remote Access is not supported in call the the remote access session will end and you will be able to control the call from this tab on the Web Interface.
