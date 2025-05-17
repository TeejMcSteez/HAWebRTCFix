Used to patch the issue in firefox where Ring WebRTC streams fail due to incorrect offer/answer signals sent by Ring API.

Uses SDP transform to morph Ring API signals to what they are suppoed to be.

This **HAS NOT** been tested more of a fix for my core setup as I use firefox and seem to be one of the only ones to enjoy it.

[sdp-transform](https://github.com/skymaze/sdp-transform) GitHub, Forked from skymaze/sdp-transform.

[HA_Core](https://github.com/home-assistant/core) GitHub, Forked from home-assistant/core. Used ring components, specifically camera.py, to flip bad Ring WebRTC offers

### Credits

- Original Home Assistant WebRTC Ring integration by the Home Assistant core team  
- SDP parsing library by the sdp-transform authors  
- Firefox SDP direction patch by TeejMcSteez ([github.com/TeejMcSteez/HAWebRTCFix](https://github.com/TeejMcSteez/HAWebRTCFix))
