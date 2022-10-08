# VezerSyncManager

VezerSyncManager is an HDA for combining Houdini and Vezer.
It allows mutual keyframe editing between Vezer and Houdini.
This HDA help you...
-  Hit keyframes on Houdini, where audio playback is terrible.
- Reuse Keyframes typed in Houdini in other software that can receive OSC.

# Intended users
People who type keyframes in Vezer on Mac and create CG in Houdini on Windows.

# Getting Started
1. Clone this repo.
1. Copy otls/VezerSyncManager.hda to your HDA directory
1. Set your Vezer file Path
1. Hit Load Buttoon
1. Vezer obj is created in your /obj
1. This node has a corresponding parameter to Vezer's Track.
1. You can use keyframe value via reference copy and so on...
1. If you edit keyframe value and want to 
# Limitation
- Supported Vezer Track types are "MIDI CC", "OSC Value", and "OSC Flag".
- The functions for keyframe completion that can be used inside each software are limited.
- This is a personal development, so please forgive any bugs.

## Interpolate function Correspondence Tables

### Vezer → Houdini
|  TH  |  TH  |
| ---- | ---- |
|  No Interpolation |  TD  |
|  TD  |  TD  |


### Houdini →  Vezer
|  TH  |  TH  |
| ---- | ---- |
|  No Interpolation |  TD  |
|  TD  |  TD  |