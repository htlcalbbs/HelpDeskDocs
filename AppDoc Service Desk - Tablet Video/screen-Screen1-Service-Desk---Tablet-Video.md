# Power App Documentation \- Service Desk \- Tablet Video

| Property                   | Value                                   |
| -------------------------- | --------------------------------------- |
| App Name                   | Service Desk \- Tablet Video            |
| App Logo                   | ![App Logo](resources/applogoSmall.png) |
| Documentation generated at | Friday, May 3, 2024 4:30 PM             |

- [Overview](index-Service-Desk---Tablet-Video.md)
- [App Details](appdetails-Service-Desk---Tablet-Video.md)
- [Variables](variables-Service-Desk---Tablet-Video.md)
- [DataSources](datasources-Service-Desk---Tablet-Video.md)
- [Resources](resources-Service-Desk---Tablet-Video.md)
- [Controls](controls-Service-Desk---Tablet-Video.md)

## Screen1

| Property                        | Value        |
| ------------------------------- | ------------ |
| ![screen](resources/screen.png) | Type: screen |

### Design

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Height              | Max(App.Height, App.MinScreenHeight)                                                                                                                                                                                                                                                                                                                                                                           |
| ImagePosition       | ImagePosition.Fit                                                                                                                                                                                                                                                                                                                                                                                              |
| LoadingSpinner      | LoadingSpinner.None                                                                                                                                                                                                                                                                                                                                                                                            |
| LoadingSpinnerColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 51, 102, 1)</td></tr><tr><td style="background-color:#003366"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table> |
| Orientation         | If(Self.Width \< Self.Height, Layout.Vertical, Layout.Horizontal)                                                                                                                                                                                                                                                                                                                                              |
| Size                | 1 + CountRows(App.SizeBreakpoints) \- CountIf(App.SizeBreakpoints, Value \>\= Self.Width)                                                                                                                                                                                                                                                                                                                      |
| Width               | Max(App.Width, App.MinScreenWidth)                                                                                                                                                                                                                                                                                                                                                                             |

### Color Properties

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fill     | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>White</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property      | Value    |
| ------------- | -------- |
| Child Control | Gallery1 |
| Child Control | Button4  |

## Button4

| Property                        | Value        |
| ------------------------------- | ------------ |
| ![button](resources/button.png) | Type: button |

### Behavior

| Property | Value                                                                                                                                                                                                                                                             |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ForAll( Gallery1.AllItems As My, Patch( TicketTypes, LookUp(TicketTypes, ID = My.ID), { TicketTypes: My.field_0 } ) ); <td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property | Value    |
| -------- | -------- |
| Text     | "Button" |

### Design

| Property      | Value                |
| ------------- | -------------------- |
| Align         | Align.Center         |
| BorderStyle   | BorderStyle.Solid    |
| DisplayMode   | DisplayMode.Edit     |
| Font          | Font.'Open Sans'     |
| FontWeight    | FontWeight.Semibold  |
| Height        | 40                   |
| Size          | 15                   |
| VerticalAlign | VerticalAlign.Middle |
| Width         | 160                  |
| X             | 306                  |
| Y             | 725                  |
| ZIndex        | 2                    |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | ColorFade(Self.Fill, \-15%)                                                                                                                                                                                                                                                                                                                                                                                      |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |
| DisabledBorderColor | ColorFade(Self.BorderColor, 70%)                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                              |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                           |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(62,96,170,1)</td></tr><tr><td style="background-color:#3E60AA"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table>     |
| FocusedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverBorderColor    | ColorFade(Self.BorderColor, 20%)                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverColor          | Self.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverFill           | ColorFade(Self.Fill, 20%)                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedBorderColor  | Self.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedColor        | Self.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | Self.Color                                                                                                                                                                                                                                                                                                                                                                                                       |

### Child & Parent Controls

| Property       | Value   |
| -------------- | ------- |
| Parent Control | Screen1 |

## Gallery1

| Property                          | Value         |
| --------------------------------- | ------------- |
| ![gallery](resources/gallery.png) | Type: gallery |

### Data

| Property  | Value                                                                                                                                                                    |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Items     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">TicketTypes<td style="background-color:#ffcccc; width:50%;">CustomGallerySample</td></tr></table> |
| WrapCount | 1                                                                                                                                                                        |

### Design

| Property            | Value                                                                                                                                                                  |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle         | BorderStyle.Solid                                                                                                                                                      |
| DisplayMode         | DisplayMode.Edit                                                                                                                                                       |
| Height              | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">362<td style="background-color:#ffcccc; width:50%;">575</td></tr></table>                       |
| Layout              | Layout.Vertical                                                                                                                                                        |
| LoadingSpinner      | LoadingSpinner.None                                                                                                                                                    |
| LoadingSpinnerColor | Self.BorderColor                                                                                                                                                       |
| TemplatePadding     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;">0</td></tr></table>                           |
| TemplateSize        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">48<td style="background-color:#ffcccc; width:50%;">Min(160, Self.Height - 60)</td></tr></table> |
| Transition          | Transition.None                                                                                                                                                        |
| Width               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">421<td style="background-color:#ffcccc; width:50%;">640</td></tr></table>                       |
| X                   | 299                                                                                                                                                                    |
| Y                   | 405                                                                                                                                                                    |
| ZIndex              | 1                                                                                                                                                                      |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| DisabledBorderColor | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                              |
| DisabledFill        | Self.Fill                                                                                                                                                                                                                                                                                                                                                                                                     |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 231, 246, 1)</td></tr><tr><td style="background-color:#CCE7F6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| FocusedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                              |
| HoverBorderColor    | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                              |
| HoverFill           | Self.Fill                                                                                                                                                                                                                                                                                                                                                                                                     |
| PressedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedFill         | Self.Fill                                                                                                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value            |
| -------------- | ---------------- |
| Child Control  | galleryTemplate2 |
| Child Control  | Label1           |
| Child Control  | Label1\_1        |
| Parent Control | Screen1          |

## galleryTemplate2

| Property                                          | Value                 |
| ------------------------------------------------- | --------------------- |
| ![galleryTemplate](resources/galleryTemplate.png) | Type: galleryTemplate |

### Design

| Property     | Value                                                                                                                                                                                                                                                                                                                                |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| TemplateFill | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Color Properties

### Child & Parent Controls

| Property       | Value    |
| -------------- | -------- |
| Parent Control | Gallery1 |

## Label1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                    |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Select(Parent)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property | Value                                                                                                                                                            |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Live     | Live.Off                                                                                                                                                         |
| Role     | TextRole.Default                                                                                                                                                 |
| Text     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.field_0<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property      | Value                |
| ------------- | -------------------- |
| Align         | Align.Left           |
| BorderStyle   | BorderStyle.Solid    |
| DisplayMode   | DisplayMode.Edit     |
| Font          | Font.'Open Sans'     |
| FontWeight    | FontWeight.Normal    |
| Height        | 40                   |
| Overflow      | Overflow.Hidden      |
| Size          | 13                   |
| VerticalAlign | VerticalAlign.Middle |
| Width         | 150                  |
| X             | 0                    |
| Y             | 0                    |
| ZIndex        | 1                    |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101, 128, 187, 1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47,41,43,1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                              |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                                  |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                                  |
| FocusedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverBorderColor    | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverColor          | Self.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverFill           | Self.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedColor        | Self.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedFill         | Self.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value    |
| -------------- | -------- |
| Parent Control | Gallery1 |

## Label1\_1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                    |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Select(Parent)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property | Value                                                                                                                                                                |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Live     | Live.Off                                                                                                                                                             |
| Role     | TextRole.Default                                                                                                                                                     |
| Text     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.TicketTypes<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Align           | Align.Left                                                                                                                                   |
| BorderStyle     | BorderStyle.Solid                                                                                                                            |
| BorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;">0</td></tr></table> |
| DisplayMode     | DisplayMode.Edit                                                                                                                             |
| Font            | Font.'Open Sans'                                                                                                                             |
| FontWeight      | FontWeight.Normal                                                                                                                            |
| Height          | 40                                                                                                                                           |
| Overflow        | Overflow.Hidden                                                                                                                              |
| Size            | 13                                                                                                                                           |
| VerticalAlign   | VerticalAlign.Middle                                                                                                                         |
| Width           | 150                                                                                                                                          |
| X               | 231                                                                                                                                          |
| Y               | 0                                                                                                                                            |
| ZIndex          | 2                                                                                                                                            |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101, 128, 187, 1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47,41,43,1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                              |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                                  |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                                  |
| FocusedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverBorderColor    | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverColor          | Self.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverFill           | Self.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedColor        | Self.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedFill         | Self.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value    |
| -------------- | -------- |
| Parent Control | Gallery1 |
