---
-api-id: T:Windows.UI.Input.Preview.Injection.InjectedInputTouchParameters
-api-type: winrt enum
---

<!-- Enumeration syntax
public enum Windows.UI.Input.Preview.Injection.InjectedInputTouchParameters : uint
-->

# InjectedInputTouchParameters

## -description
Specifies the touch states used to simulate touch input through [InjectedInputTouchInfo](injectedinputtouchinfo.md).

## -enum-fields
### -field None:0
No touch state reported. Default.

### -field Contact:1
The screen coordinates of the bounding box that represents the touch contact area.

### -field Orientation:2
The counter-clockwise angle of rotation around the major axis of the pointer device (the z-axis, perpendicular to the surface of the digitizer).

### -field Pressure:4
The force exerted by the pointer device on the surface of the digitizer.


## -remarks

> [!Important]
> The APIs in this namespace require the inputInjectionBrokered [restricted capability](https://docs.microsoft.com/windows/uwp/packaging/app-capability-declarations#special-and-restricted-capabilities).

Using input injection requires the following be added to the Package.appxmanifest:

- To `<Package>`
    - `xmlns:rescap="http://schemas.microsoft.com/appx/manifest/foundation/windows10/restrictedcapabilities"`
    - `IgnorableNamespaces="rescap"`
- To `<Capabilities>`
    - `<rescap:Capability Name="inputInjectionBrokered" />`


## -examples

## -see-also

### Conceptual

[Gaze interactions and eye tracking in UWP apps](https://docs.microsoft.com/windows/uwp/design/input/gaze-interactions)

### Samples

- [Simulate user input through input injection](https://review.docs.microsoft.com/windows/uwp/design/input/input-injection?branch=kbridge-inputinjection)
- [Input injection sample (mouse to touch)](https://github.com/MicrosoftDocs/windows-topic-specific-samples/archive/uwp-input-injection-mouse-to-touch.zip)
- [Touch injection sample](http://go.microsoft.com/fwlink/p/?LinkID=267906)
- [Input: XAML user input events sample](http://go.microsoft.com/fwlink/p/?linkid=226855)
