---
-api-id: P:Windows.Devices.Lights.Effects.LampArrayCustomEffect.ZIndex
-api-type: winrt property
---

<!-- Property syntax.
public int ZIndex { get;  set; }
-->

# Windows.Devices.Lights.Effects.LampArrayCustomEffect.ZIndex

## -description
The global precedence for two effects that modify the same lamp.

## -property-value
Value of the global precedence. Default value is 0.

## -remarks
Higher zIndex implies higher precedence.

If two effects with the same zIndex operate on the same lamp (via two separate [LampArrayEffectPlaylists](lamparrayeffectplaylist.md)), the behavior is undefined.

## -see-also

## -examples

