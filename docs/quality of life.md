---
title: Quality Of Life
order: -4
---

### DO NOT DISTURB/Disable Notifications
added by @pixelyloaf
```json
{
    "FFlagToastNotificationsProtocolEnabled2": "False"
}
```
### Disable VC
added by @pixelyloaf
> [!NOTE]
> Setting this to `True` will not do anything
```json
{
    "DFFlagVoiceChat4": "False"
}
```
### Remove translated supported message on join
added by @pixelyloaf
> [!NOTE]
> `"Roblox automatically translates supported languages in chat."`
```json
{
    "FFlagChatTranslationEnableSystemMessage": "False"
}
```

### Allows you to customize which languages are available for the chat translation feature
added by @pixelyloaf
> [!IMPORTANT]
> English cannot be removed.


```json
{
    "FStringChatTranslationEnabledLocales": "es_es,fr_fr,pt_br,de_de,it_it,ja_jp,ko_kr,id_id,tr_tr,zh_cn,zh_tw,th_th,pl_pl,vi_vn,ru_ru,"
}
```
### Remove long recommended section in homepage
added by @pixelyloaf
```json
{
    "FIntGameGridFlexFeedItemTileNumPerFeed": "0"
}
```
### Disable Captures Keybind
added by @pixelyloaf
```json
{
    "FFlagEnableCapturesHotkeyExperiment_v4": "False"
}
```
### Reduced Avatar Item Particle in FP
added by @pixelyloaf
```json
{
    "FFlagUserHideCharacterParticlesInFirstPerson": "True"
}
```
### FPS Unlocker in Roblox Menu Settings
added by @pixelyloaf
```json
{
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
    "DFIntTaskSchedulerTargetFps": "9999"
}
```
### Disable 240 FPS cap
added by @pixelyloaf
```json
{
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False"
}
```
### Unlimited FPS Unlocker
added by @pixelyloaf
```json
{
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
    "DFIntTaskSchedulerTargetFps": "9999"
}
```
### GUI Hiding Toggles
added by @pixelyloaf
```json
{
    "FFlagUserShowGuiHideToggles": "True",
    "GuiHidingApiSupport2": "True"
}
```
### Hide GUIs
added by @pixelyloaf
> [!IMPORTANT]
> Replace "ID" with any group ID that you are in.

| Key combination   | Action                                                                    |
| ----------------- | ------------------------------------------------------------------------- |
| Ctrl + Shift + B  | Toggles GUIs in 3D space (BillboardGuis, SurfaceGuis, etc)                |
| Ctrl + Shift + C  | Toggles game-defined ScreenGuis                                           |
| Ctrl + Shift + G  | Toggles Roblox CoreGuis                                                   |
| Ctrl + Shift + N  | Toggles player names, and other BillboardGuis that show up above a player |
```json
{
    "DFIntCanHideGuiGroupId": "ID"
}
```
### Remove layered clothing related for searching in lua app catalog
added by @pixelyloaf
```json
{
    "FStringAXCategories": "ClassicShirts.ClassicTShirts.ClassicPants"
}
```
### Disable Fullscreen Title Bar
added by @pixelyloaf
```json
{
    "FIntFullscreenTitleBarTriggerDelayMillis": "3600000"
}
```
### Stuttery Animation Fix
added by @pixelyloaf

might of messed up the spelling mb
```json
{
    "DFIntTimestepArbiterThresholdCFLThou": "300"
}
```
### Disable In-game Advertisements
added by @pixelyloaf
```json
{
    "FFlagAdServiceEnabled": "False"
}
```
### Disable Telemetry
added by @pixelyloaf
```json
{
    "FFlagDebugDisableTelemetryEphemeralCounter": "True",
    "FFlagDebugDisableTelemetryEphemeralStat": "True",
    "FFlagDebugDisableTelemetryEventIngest": "True",
    "FFlagDebugDisableTelemetryPoint": "True",
    "FFlagDebugDisableTelemetryV2Counter": "True",
    "FFlagDebugDisableTelemetryV2Event": "True",
    "FFlagDebugDisableTelemetryV2Stat": "True"
}
```
### Surf the web inside of Roblox
added by @pixelyloaf
> [!IMPORTANT]
> **Click the Beta Badge of the 13+ badge to open the webview browser.**
```json
{
    "FFlagTopBarUseNewBadge": "True",
    "FStringTopBarBadgeLearnMoreLink": "https://udm14.com/",
    "FStringVoiceBetaBadgeLearnMoreLink": "https://udm14.com/"
}
```
### MTU
added by @pixelyloaf
==- :icon-question: View Full Documentation
> [!TIP]
> **Identify the Current MTU**
> - **Windows**: Open Command Prompt and type 'netsh interface ipv4 show subinterfaces`.
> - **Linux**: Use 'ifconfig' or 'ip link show' to find the current MTU of your network interface.

> [!TIP]
> **Determine the Optimal MTU**
> - **Ping Test**: Use the `ping` command with the `-f` flaf (to avoid fragmentation) and the `l` (or `s` on Linux) flag to set the global packet size.
> - **Example for Windows**:
> ```bash
> ping roblox.com -f -l 1472
> ```
> - **Example for Linux**:
> ```bash
> ping -s 1472 -M do roblox.com
> ```
> - Start with a packet size of 1472 bytes, then reduce by 10-12 bytes if needed until you find the largest size that doesn't fragment. Add 28 bytes to this number to get the optimal MTU.
===
```json
{
    "DFIntConnectionMTUSize": "MTU_HERE"
}
```
### No Internet Disconnect
added by @pixelyloaf
> [!NOTE]
> **You will still be kicked but the message will not show.**
```json
{
    "DFFlagDebugDisableTimeoutDisconnect": "True"
}
```
### Adjust Default Timeout Time
added by @pixelyloaf
> [!TIP]
> **1 second = 1000**


```json
{
    "DFIntDefaultTimeoutTimeMs": "10000"
}
```
### Quick Game Launch
added by @pixelyloaf
> [!CAUTION]
> **This can cause some bugs**
```json
{
    "FFlagEnableQuickGameLaunch": "True"
}
```
### Increased Asset Preloading Count
added by @pixelyloaf
==- :icon-question: View Full Documentation
> [!NOTE]
> **Increasing the maximum limit of preloaded assets from 100 to infinite allows games you've already played to load much faster by instantly accessing previously loaded assets.**

> [!IMPORTANT]
> **For this to be effective, the game must have been fully loaded at least once, preferably with the entire map cached.**

> [!TIP]
> **If a game has a "Skip Loading" button, it's recommended to use it. These games typically include a countdown timer that, after reaching zero, merely confirms that all assets are loaded.**
===

```json
{
    "DFIntNumAssestsMaxToPreload": "9999999",
    "DFIntAssetPreloading": "9999999"
}
```
### Disable In-Gmae Purchases
added by @pixelyloaf
```json
{
    "DFlagOrder66": "True"
}
```
### Disable Chat
added by @pixelyloaf
```json
{
    "FFlagDebugForceChatDisabled": "True"
}
```
### Disable Dynamic Heads Animations
added by @pixelyloaf
```json
{
    "DFIntAnimationLodFacsDistanceMin": "0",
    "DFIntAnimationLodFacsDistanceMax": "0",
    "DFIntAnimationLodFacsVisibilityDenominator": "0"
}
```
### Automatically unmuts your mic on join (VC)
added by @pixelyloaf
```json
{
    "FFlagDebugDefaultChannelStartMuted": "False"
}
```
### opt-out Experience Language
added by @pixelyloaf
> [!NOTE]
> **Removes the Experience Language option in settings**
```json
{
    "FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0"
}
```
### Lets you change the zoom out limit
added by @pixelyloaf
> [!IMPORTANT]
> **Only applies to games that has not changed the default zoom limit**
```json
{
    "FIntCameraMaxZoomDistance": "9999"
}
```
### Exclusive Fullscreen
added by @pixelyloaf
> [!TIP]
> Alt + Delete
```json
{
    "FFlagHandleAltEnterFullscreenManually": "False"
}
```
### Change Age Rating Learn More Link
added by @pixelyloaf
```json
{
    "FStringExperienceGuidelinesExplainedPageUrl": "https://udm14.com/"
}
```
### Rename Party 2 Roblox Chat
added by @pixelyloaf
```json
{
    "FFlagAppChatRebrandStringUpdates": "False"
}
```
### 5 decimal digits limit for camera sensitivity
added by @pixelyloaf
> [!NOTE]
> only added because people i know use them
```json
{
    "FFlagFixSensitivityTextPrecision": "False"
}
```