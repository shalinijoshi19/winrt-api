---
-api-id: T:Windows.UI.Xaml.Automation.StylesPatternIdentifiers
-api-type: winrt class
---

<!-- Class syntax.
public class StylesPatternIdentifiers : Windows.UI.Xaml.Automation.IStylesPatternIdentifiers
-->

# Windows.UI.Xaml.Automation.StylesPatternIdentifiers

## -description
Contains values used as identifiers by [IStylesProvider](../windows.ui.xaml.automation.provider/istylesprovider.md).

## -remarks
Classes such as [StylesPatternIdentifiers](stylespatternidentifiers.md) are the identifiers for the Windows Runtime implementation of a common provider pattern for Microsoft UI Automation. You might use these identifiers if you are implementing a Windows Runtime custom automation peer that reports support for [IStylesProvider](../windows.ui.xaml.automation.provider/istylesprovider.md) in its [GetPattern](../windows.ui.xaml.automation.peers/automationpeer_getpattern_2046576749.md) implementation. These identifiers are needed for the [RaisePropertyChangedEvent](../windows.ui.xaml.automation.peers/automationpeer_raisepropertychangedevent_715050195.md) calls that you make from control code that references your own peer, or for [FindItemByProperty](../windows.ui.xaml.automation.peers/itemscontrolautomationpeer_finditembyproperty_1997743353.md) in an items container peer. This same pattern is usually exposed to clients in a different way, depending on which technology they use to implement the client and examine the Microsoft UI Automation tree. [IStylesProvider](http://msdn.microsoft.com/library/9424a6cd-9f4b-4653-9737-4afb9cfb510f) is also presented as a Component Object Model (COM) interface.

## -examples

## -see-also
[IStylesProvider](../windows.ui.xaml.automation.provider/istylesprovider.md), [Custom automation peers](http://msdn.microsoft.com/library/aa8da53b-fe6e-40ac-9f0a-cb09637c87b4), [Control patterns and interfaces](http://msdn.microsoft.com/library/2091883c-5d0c-44ed-936a-709022926a42)