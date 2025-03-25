---
title: Audio Related
icon: mute
order: -6
---
### Allows you to change voice chat distance
added by @pixelyloaf
> [!NOTE]
> **Default: [Min 7 Max 80]**
```json
{
    "DFIntVoiceChatRollOffMinDistance": "7",
    "DFIntVoiceChatRollOffMaxDistance": "80"
}
```
### Sounds use physical velocity and become distorted
added by @pixelyloaf
> [!NOTE]
> **<2017 Audio**
```json
{
    "FFlagSoundsUsePhysicalVelocity": "True"
}
```
### Audio Occlusion
added by @pixelyloaf
```json
{
    "FFlagDebugEnableDirectAudioOcclusion2": "True"
}
```
### Limit audios that are being played
added by @pixelyloaf
```json
{
    "DFIntMaxLoadableAudioChannelCount": "1"
}
```
### Mess with voice chat volume
added by @pixelyloaf
[!NOTE]
> **Default: 1000**
```json
{
    "DFIntVoiceChatVolumeThousandths" "100000"
}
```
### No sounds
added by @pixelyloaf
```json
{
    "FFlagDebugRomarkMockingAudioDevices": "True"
}
```