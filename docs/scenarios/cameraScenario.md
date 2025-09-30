# Scenario 2 - Camera

## Problem

In this scenario the end user is reporting the camera is misaligned.

Heading to the location of the endpoint could be costly so to solve this scenario we will use Remote Access to help the end user configure the camera and also set up meeting zones.

### User report:

> The camera on my device is always aiming at the ceiling, it always worked as expected until last week when it was used for a different presentation when the camera angle was changed. Can you come fix this?
Here is a screenshot of the device:
![Preset Camera FullScreen](./../assets/PresetCameraFullScreen.png){ width="500" }

## Your task

In this scenario you’ll need to start a Remote Access session, open the device settings, and adjust the camera view so the end user is supported:

- To start a Remote Access session follow the instructions from [Hello Remote Access](./helloRemoteAccess.md).

- After the session is established you will have access to the devices as if you are in the room, first thing to do is check the current state of the self view. To do so go to settings by clicking the top right settings icon ![Control Panel Icon](./../assets/Controlpanel_normal.png){ width="30" }. Click on the camera icon and set camera to a position where it frames the user in the room. Here you can also have a visual confirmation that the camera is pointing at a reasonable place. 

Another option (not using Remote Access) is to to activate speaker tracker config _(xconfiguration Cameras SpeakerTrack Mode: Auto)_ so the end user can choose between Dynamic and Manual camera mode. We can skip that.

There are additional things you could do here such as apply different backgrounds or blur the background, or set up Meeting Zone to prevent from possible issues in the future.

### Setting up meeting zones

- An additional way to improve the end user experience is to configure the meeting zone. On the device navigate to Device Settings ![Settings Icon](./../assets/Cogwheel_Black.png){ width="30" } at the bottom of the sidebar, then Camera -> Meeting Zones. Select either Rectangular zone or Round zone. As seen in the image here you can outline the area the device should focus when having a meeting. Meeting Zones allows you to limit the area of interest for the speaker tracker and video framing logic allowing the device to reach better results when deciding what to include in the video frames.

![Meeting Zones](./../assets/MeetingZones.png){ width="500" }

You have now solved an issue for the user with minimal effort, no presence in the room was needed, and you improved the meeting experience.


We are ready for the next scenario where we will take the role of an integrator and be sure our deployment is working as expected: [Scenario 3 - Customizations](./customizationsScenario.md).
