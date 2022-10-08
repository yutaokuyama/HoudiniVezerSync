# VezerSyncManager

VezerSyncManager is an HDA for combining Houdini and Vezer.
It allows mutual keyframe editing between Vezer and Houdini.
This HDA help you...
-  Set keyframes on Houdini, where audio playback is terrible.
- Reuse Keyframes added in Houdini in other software that can receive OSC.
[![Image from Gyazo](https://i.gyazo.com/bd83f8f55af97ae3e32579b37f1d49c7.gif)](https://gyazo.com/bd83f8f55af97ae3e32579b37f1d49c7)
# Intended users
People who set keyframes in Vezer on Mac and create CG in Houdini on Windows.

# Getting Started
1. Clone this repo.
1. Copy `otls/VezerSyncManager.hda` to your HDA directory
1. Put VezerSyncManager to `/obj` and set your Vezer file Path in parameter
1. Hit Load Button
1. Vezer obj is created in your `/obj`
1. This node has a corresponding parameter to Vezer's Track.
1. You can use keyframe value via reference copy and so on...
1. If you edit keyframe value and want to reflect Vezer file, hit save button.

# Transfer Vezer file via SSH
The HDA additionally supports the exchange of vezer files via SSH. To use this feature, you must be able to log in remotely from Windows to your Mac with public key authentication.
[![Image from Gyazo](https://i.gyazo.com/a7f1ec0cdf5d2be157794cf37e245391.png)](https://gyazo.com/a7f1ec0cdf5d2be157794cf37e245391)

# Limitation
- Supported Vezer Track types are `MIDI CC`, `OSC Value`, and `OSC Flag`
- The functions for keyframe completion that can be used inside each software are limited.
- This is a personal development, so please forgive any bugs.
