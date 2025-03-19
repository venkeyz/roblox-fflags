---
title: Abusive
icon: alert-fill
order: -7
---
### Drunk
```json
{
    "FFlagSimAdaptiveTimesteppingDefault2": "True",
    "DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999",
    "DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```
### Fake lag
```json
{
    "DFIntS2PhysicSenderRate": "1"
}
```
### Noclip 1
> [!NOTE]
> **this currently looks broken to me, might not work for you (good job roblox, honestly)**

> [!TIP]
> adjust the value if you fall through stuff that you shouldn't be falling through
```json
{
    "DFIntAssemblyExtentsExpansionStudHundredth": "-50"
}
```
### Noclip 2/Mesh noclip
```json
{
    "DFIntPhysicsDecompForceUpgradeVersion": "1500"
}
```
### Tool desync
```json
{
    "DFIntSimBlockLargeLocalToolWeldManipulationsThreshold": "-1"
}
```
### No Knockback/Ragdoll
```json
{
    "DFIntGameNetLocalSpaceMaxSendIndex": "100000",
    "DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "0"
}
```
### Weird leg movement
```json
{
    "DFFlagAnimatorPostProcessIK": "True"
}
```
### No animations
> [!NOTE]
> stops the game trying to replicate your animation in the server (animations exist in client)
```json
{
    "DFIntReplicatorAnimationTrackLmiitPerAnimator": "-1"
}
```
### Warp
```json
{
    "DFIntMaxMissedWorldStepsRemembered": "1000"
}
```
### Buggy zplane camera
```json
{
    "FIntCameraFarZPlane": "1"
}
```