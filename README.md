Used to patch the issue in Firefox where Ring WebRTC streams fail due to incorrect offer/answer signals sent by the Ring API.

Uses SDP transform to morph Ring API signals to what they are supposed to be.

This **HAS NOT** been tested more of a fix for my core setup as I use Firefox and seem to be one of the only ones to enjoy it.

[sdp-transform](https://github.com/skymaze/sdp-transform) GitHub, Forked from skymaze/sdp-transform.

[HA_Core](https://github.com/home-assistant/core) GitHub, Forked from home-assistant/core. Used ring components, specifically camera.py, to flip bad Ring WebRTC offers

### Credits

- Original Home Assistant WebRTC Ring integration by the Home Assistant core team  
- SDP parsing library by the sdp-transform authors  
- Firefox SDP direction patch by TeejMcSteez ([github.com/TeejMcSteez/HAWebRTCFix](https://github.com/TeejMcSteez/HAWebRTCFix))

### Usage

1. Import these files into your config into a new directory ./custom_components/ring
  - This will override the normal ring component with your custom one if you already have the integration

2. Restart the HA server and it should install all dependencies as well as override the ring component if already installed

3. Now you can stream Ring Cams on your Firefox dashboard!
