---
title: Quality Of Life
icon: sparkle-fill
order: 3
---

### Disable Notifications
```json
{
    "FFlagToastNotificationsProtocolEnabled2": "False"
}
```
### Disable VC
> [!NOTE]
> Setting this to `True` will not do anything
```json
{
    "DFFlagVoiceChat4": "False"
}
```
### Disable Telemetry
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
### Disable fulscreen title bar
```json
{
    "FIntFullscreenTitleBarTriggerDelayMillis": "3600000"
}
```
### Automatically unmute mic (VC)
```json
{
    "FFlagDebugDefaultChannelStartMuted": "False"
}
```
### Party to Roblox Chat
```json
{
    "FFlagAppChatRebrandStringUpdates": "False"
}
```
### Remove translated supported message
> [!NOTE]
> `"Roblox automatically translates supported languages in chat."`
```json
{
    "FFlagChatTranslationEnableSystemMessage": false
}
```