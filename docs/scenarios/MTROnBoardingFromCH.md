# Scenario 5 - MTR onboarding

!!! important "Not a hands-on scenario"
    We will not go over this scenario on the devices in our lab. The devices here are Cisco Desks and do not support MTR. We will go over this scenario together.

In this scenario, you will be an admin that needs to get the Microsoft Teams Room (MTR) code that shows on the device to be able to finish the MTR onboarding process. The device still needs to be registered to control hub so we can start a Remote Access session. Your goal is to view the MTR code on Remote Access session. We will not go further with the MTR registration. Once you reach this screen you are done with this scenario:

![MTR Code](./../assets/MTRCode.png){ width="800" }


But we will need some setup to get to this scenario.

## Setup Steps

### 1 - Factory reset the device. 

Make use of one of the guides on how to run an xCommand: 

- [Using xAPI commands on Control Hub](../guides.md#xapi-commands-on-CH)  

- [Using xAPI commands on Local Device Controls webpage](../guides.md#xapi-commands-on-LocalDeviceControls)

Then run the following xCommand to factory reset the device:

```
xCommand SystemUnit FactoryReset Confirm: yes
```

This process might take a few minutes.

### 2 - Get an activation code from Control Hub 

In Control Hub, got to the Devices page click Add Device -> Shared Usage -> Next -> New Workspace. Here, you can set a name for the workspace that you will use to find the device later. Click Next -> Cisco Room and Desk Devices -> Next (there is no need to change anything). Click on Add Device to get the activation code. That is the code you will enter on the device.

??? Note "Show me how to get the activation code in CH"
    ![alt text](./../assets/GetActivationCodeInCH.gif)

We will enter the activation code soon on the device, so make sure to save it or have it available to you during step 3.

### 3 - Add the activation code to the device during the MTR onboarding process.

Now that you have the activation code, enter it manually on the device manually. After the factory reset the device will be on the welcome screen. From here, choose all the default options until you see a screen with "Cisco RoomOS Experience" and "Microsoft Teams Experience". Select Microsoft, then enter the activation code, press "Continue" and then begin installation. This process will take several minutes.

??? Note "Show me how to register device and start MTR onboarding process"
    ![alt text](./../assets/MTROnboardingViaControlHub.gif)

### 4 - Start a Remote Access Session
- Go to Control Hub and find the device you just registered with the workspace you created in step 2.
- Now you are ready to start a Remote Access session.

### 5 - Verify what is the MTR Code on screen
- If step 3 is still not over, the MTR installation is still in progress. You might need to wait a few more minutes.
- You should be able to see the MTR code on screen. From this point on as an admin you should be able to finish the registration process on the microsoft login webpage but we will not cover that on this course. 


For a full guide on how to register MTR devices check the documentation on [MTR OnBoarding](https://roomos.cisco.com/doc/MTR/MTROnBoarding#control-hub-registration-after-the-initial-setup). The documentation also describes the scenario of devices already registered to Control Hub being registered to MTR. 


Our last scenario is [Scenario 6 - RoomOS onboarding](./roomOSOnBoardingFromCH.md).
