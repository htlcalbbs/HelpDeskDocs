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

## TicketdetailsPage

| Property                        | Value        |
| ------------------------------- | ------------ |
| ![screen](resources/screen.png) | Type: screen |

### Behavior

| Property  | Value |
| --------- | ----- |
| OnVisible |       |

### Design

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Height              | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Max(App.Height, App.DesignHeight)<td style="background-color:#ffcccc; width:50%;">Max(App.Height, App.MinScreenHeight)</td></tr></table>                                                                                                                                                                                                |
| ImagePosition       | ImagePosition.Fit                                                                                                                                                                                                                                                                                                                                                                                              |
| LoadingSpinner      | LoadingSpinner.None                                                                                                                                                                                                                                                                                                                                                                                            |
| LoadingSpinnerColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 51, 102, 1)</td></tr><tr><td style="background-color:#003366"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table> |
| Orientation         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(TicketdetailsPage.Width < TicketdetailsPage.Height, Layout.Vertical, Layout.Horizontal)<td style="background-color:#ffcccc; width:50%;">If(Self.Width < Self.Height, Layout.Vertical, Layout.Horizontal)</td></tr></table>                                                                                                           |
| Size                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1 + CountRows(App.SizeBreakpoints) - CountIf(App.SizeBreakpoints, Value >= TicketdetailsPage.Width)<td style="background-color:#ffcccc; width:50%;">1 + CountRows(App.SizeBreakpoints) - CountIf(App.SizeBreakpoints, Value >= Self.Width)</td></tr></table>                                                                            |
| Width               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Max(App.Width, App.DesignWidth)<td style="background-color:#ffcccc; width:50%;">Max(App.Width, App.MinScreenWidth)</td></tr></table>                                                                                                                                                                                                    |

### Color Properties

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fill     | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>White</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property      | Value             |
| ------------- | ----------------- |
| Child Control | Rectangle1\_1     |
| Child Control | TextBox4\_1       |
| Child Control | Rectangle1\_3     |
| Child Control | icon4             |
| Child Control | TextBox3          |
| Child Control | Rectangle5\_7     |
| Child Control | TicketDetailsForm |
| Child Control | TextBox5\_50      |
| Child Control | TextBox5\_56      |
| Child Control | TextBox5\_51      |
| Child Control | TextBox5\_57      |
| Child Control | TextBox5\_52      |
| Child Control | TextBox5\_61      |
| Child Control | TextBox5\_55      |
| Child Control | TextBox5\_58      |
| Child Control | Button1           |
| Child Control | Group3            |
| Child Control | Group4            |

## Button1

| Property                        | Value        |
| ------------------------------- | ------------ |
| ![button](resources/button.png) | Type: button |

### Behavior

| Property | Value                                                                                                                                                                   |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">SubmitForm(TicketDetailsForm)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                    |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Save"<td style="background-color:#ffcccc; width:50%;">"Button"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                                  |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Center                                                                                                                                                                           |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                        |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                                      |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">2</td></tr></table>                                           |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                       |
| FocusedBorderThickness | 4                                                                                                                                                                                      |
| Font                   | Font.'Open Sans'                                                                                                                                                                       |
| FontWeight             | FontWeight.Semibold                                                                                                                                                                    |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">50<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                         |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">10</td></tr></table>                                          |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">10</td></tr></table>                                          |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">10</td></tr></table>                                          |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">10</td></tr></table>                                          |
| Size                   | 15                                                                                                                                                                                     |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                            |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                                   |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(EditRecord.Status="Completed",false,true)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717.0976129582267<td style="background-color:#ffcccc; width:50%;">160</td></tr></table>                         |
| X                      | 306.90238704177295                                                                                                                                                                     |
| Y                      | 718                                                                                                                                                                                    |
| ZIndex                 | 17                                                                                                                                                                                     |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | ColorFade(Button1.Fill, \-15%)                                                                                                                                                                                                                                                                                                                                                                                   |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |
| DisabledBorderColor | ColorFade(Button1.BorderColor, 70%)                                                                                                                                                                                                                                                                                                                                                                              |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                              |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                           |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(107,0,64,.8)</td></tr><tr><td style="background-color:#6B0040"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table>     |
| FocusedBorderColor  | Button1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                              |
| HoverBorderColor    | Button1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                              |
| HoverColor          | Button1.Color                                                                                                                                                                                                                                                                                                                                                                                                    |
| HoverFill           | Button1.Fill                                                                                                                                                                                                                                                                                                                                                                                                     |
| PressedBorderColor  | Button1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedColor        | Button1.Color                                                                                                                                                                                                                                                                                                                                                                                                    |
| PressedFill         | ColorFade(Button1.Fill, 20%)                                                                                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## DataCard10

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                       |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Priority"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.Priority<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Priority"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value8.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>       |

### Design

| Property    | Value                                                                                                                                                       |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">50<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| X           | 0.5                                                                                                                                                         |
| Y           | 682.742858886718                                                                                                                                            |
| ZIndex      | 7                                                                                                                                                           |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Child Control  | Key10             |
| Child Control  | StarVisible10     |
| Child Control  | ErrorMessage10    |
| Child Control  | Rectangle11       |
| Child Control  | Value8            |
| Child Control  | icon2\_11         |
| Child Control  | Rectangle7\_29    |
| Parent Control | TicketDetailsForm |

## DataCard14

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                         |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"DateClosed"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.DateClosed<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"DateClosed"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value12.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |

### Design

| Property    | Value                                                                                                                                                       |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">80<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Visible     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| X           | 0                                                                                                                                                           |
| Y           | 607.653213166145                                                                                                                                            |
| ZIndex      | 8                                                                                                                                                           |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Child Control  | StarVisible14     |
| Child Control  | Key14             |
| Child Control  | Value12           |
| Child Control  | ErrorMessage14    |
| Parent Control | TicketDetailsForm |

## DataCard4

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                      |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Subject"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.Subject<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Subject"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>            |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value1.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |

### Design

| Property    | Value                                                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">128.65321316614452<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X           | 0.5                                                                                                                                                          |
| Y           | 0.5                                                                                                                                                          |
| ZIndex      | 1                                                                                                                                                            |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Child Control  | Key3              |
| Child Control  | StarVisible3      |
| Child Control  | Rectangle3\_1     |
| Child Control  | Value1            |
| Child Control  | ErrorMessage3     |
| Child Control  | Rectangle7\_11    |
| Parent Control | TicketDetailsForm |

## DataCard5

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                          |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Description"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.Description<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Description"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value2.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>          |

### Design

| Property    | Value                                                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">135.79772552886521<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X           | 0.5                                                                                                                                                          |
| Y           | 149.34286063058                                                                                                                                              |
| ZIndex      | 2                                                                                                                                                            |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Child Control  | Key5              |
| Child Control  | StarVisible5      |
| Child Control  | Rectangle6\_2     |
| Child Control  | Value2            |
| Child Control  | ErrorMessage5     |
| Child Control  | Rectangle7\_24    |
| Parent Control | TicketDetailsForm |

## DataCard6

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                      |
| ----------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Comment"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.Comment<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Comment"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>            |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value3.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |

### Design

| Property    | Value                                                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">128.73823191733618<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X           | 0.5                                                                                                                                                          |
| Y           | 304.742858886718                                                                                                                                             |
| ZIndex      | 3                                                                                                                                                            |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Child Control  | Key6              |
| Child Control  | StarVisible6      |
| Child Control  | Rectangle6\_3     |
| Child Control  | Value3            |
| Child Control  | ErrorMessage6     |
| Child Control  | Rectangle7\_25    |
| Parent Control | TicketDetailsForm |

## DataCard7

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                     |
| ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Status"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.Status<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Status"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>           |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value5.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>     |

### Design

| Property    | Value                                                                                                                                                       |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">50<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| X           | 0.5                                                                                                                                                         |
| Y           | 438.742858886718                                                                                                                                            |
| ZIndex      | 4                                                                                                                                                           |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Child Control  | Key7              |
| Child Control  | StarVisible7      |
| Child Control  | Value5            |
| Child Control  | Rectangle8        |
| Child Control  | icon2\_8          |
| Child Control  | ErrorMessage7     |
| Child Control  | Rectangle7\_26    |
| Parent Control | TicketDetailsForm |

## DataCard8

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                         |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"AssignedTo"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.AssignedTo<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"AssignedTo"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value6.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>         |

### Design

| Property    | Value                                                                                                                                                       |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">50<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| X           | 0.5                                                                                                                                                         |
| Y           | 518.742858886718                                                                                                                                            |
| ZIndex      | 5                                                                                                                                                           |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Child Control  | Key8              |
| Child Control  | StarVisible8      |
| Child Control  | Value6            |
| Child Control  | Rectangle9        |
| Child Control  | icon2\_9          |
| Child Control  | ErrorMessage8     |
| Child Control  | Rectangle7\_27    |
| Parent Control | TicketDetailsForm |

## DataCard9

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                          |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"AccountName"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.AccountName<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"AccountName"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value7.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>          |

### Design

| Property    | Value                                                                                                                                                       |
| ----------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">51.99999999999994<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| X           | 0.5                                                                                                                                                         |
| Y           | 600.742858886718                                                                                                                                            |
| ZIndex      | 6                                                                                                                                                           |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                       |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Child Control  | Key9              |
| Child Control  | StarVisible9      |
| Child Control  | Value7            |
| Child Control  | Rectangle10       |
| Child Control  | icon2\_10         |
| Child Control  | ErrorMessage9     |
| Child Control  | Rectangle7\_28    |
| Parent Control | TicketDetailsForm |

## ErrorMessage10

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                        |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Live            | Live.Off                                                                                                                                                     |
| Role            | TextRole.Default                                                                                                                                             |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Error<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| X                      | 12                                                                                                                                                                              |
| Y                      | 0                                                                                                                                                                               |
| ZIndex                 | 3                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>  |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(237, 28, 36, 1)</td></tr><tr><td style="background-color:#ED1C24"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                          |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                         |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| FocusedBorderColor  | ErrorMessage10.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | ErrorMessage10.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | ErrorMessage10.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | ErrorMessage10.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | ErrorMessage10.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | ErrorMessage10.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | ErrorMessage10.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard10 |

## ErrorMessage14

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                        |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Live            | Live.Off                                                                                                                                                     |
| Role            | TextRole.Default                                                                                                                                             |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Error<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| X                      | 30                                                                                                                                                                              |
| Y                      | Value12.Y + Value12.Height                                                                                                                                                      |
| ZIndex                 | 3                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>  |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(237, 28, 36, 1)</td></tr><tr><td style="background-color:#ED1C24"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                          |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                         |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| FocusedBorderColor  | ErrorMessage14.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | ErrorMessage14.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | ErrorMessage14.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | ErrorMessage14.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | ErrorMessage14.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | ErrorMessage14.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | ErrorMessage14.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard14 |

## ErrorMessage3

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                        |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Live            | Live.Off                                                                                                                                                     |
| Role            | TextRole.Default                                                                                                                                             |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Error<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| X                      | 30                                                                                                                                                                              |
| Y                      | Value1.Y + Value1.Height                                                                                                                                                        |
| ZIndex                 | 3                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>  |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(237, 28, 36, 1)</td></tr><tr><td style="background-color:#ED1C24"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                          |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                         |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| FocusedBorderColor  | ErrorMessage3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | ErrorMessage3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | ErrorMessage3.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | ErrorMessage3.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | ErrorMessage3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | ErrorMessage3.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | ErrorMessage3.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard4 |

## ErrorMessage5

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                        |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Live            | Live.Off                                                                                                                                                     |
| Role            | TextRole.Default                                                                                                                                             |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Error<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| X                      | 30                                                                                                                                                                              |
| Y                      | Value2.Y + Value2.Height                                                                                                                                                        |
| ZIndex                 | 3                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>  |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(237, 28, 36, 1)</td></tr><tr><td style="background-color:#ED1C24"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                          |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                         |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| FocusedBorderColor  | ErrorMessage5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | ErrorMessage5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | ErrorMessage5.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | ErrorMessage5.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | ErrorMessage5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | ErrorMessage5.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | ErrorMessage5.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard5 |

## ErrorMessage6

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                        |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Live            | Live.Off                                                                                                                                                     |
| Role            | TextRole.Default                                                                                                                                             |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Error<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| X                      | 30                                                                                                                                                                              |
| Y                      | Value3.Y + Value3.Height                                                                                                                                                        |
| ZIndex                 | 3                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>  |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(237, 28, 36, 1)</td></tr><tr><td style="background-color:#ED1C24"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                          |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                         |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| FocusedBorderColor  | ErrorMessage6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | ErrorMessage6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | ErrorMessage6.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | ErrorMessage6.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | ErrorMessage6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | ErrorMessage6.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | ErrorMessage6.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard6 |

## ErrorMessage7

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                        |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Live            | Live.Off                                                                                                                                                     |
| Role            | TextRole.Default                                                                                                                                             |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Error<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| X                      | 11                                                                                                                                                                              |
| Y                      | 44                                                                                                                                                                              |
| ZIndex                 | 2                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>  |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(237, 28, 36, 1)</td></tr><tr><td style="background-color:#ED1C24"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                          |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                         |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| FocusedBorderColor  | ErrorMessage7.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | ErrorMessage7.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | ErrorMessage7.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | ErrorMessage7.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | ErrorMessage7.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | ErrorMessage7.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | ErrorMessage7.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard7 |

## ErrorMessage8

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                        |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Live            | Live.Off                                                                                                                                                     |
| Role            | TextRole.Default                                                                                                                                             |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Error<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| X                      | 30                                                                                                                                                                              |
| Y                      | 29                                                                                                                                                                              |
| ZIndex                 | 3                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>  |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(237, 28, 36, 1)</td></tr><tr><td style="background-color:#ED1C24"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                          |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                         |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| FocusedBorderColor  | ErrorMessage8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | ErrorMessage8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | ErrorMessage8.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | ErrorMessage8.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | ErrorMessage8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | ErrorMessage8.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | ErrorMessage8.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard8 |

## ErrorMessage9

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                        |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Live            | Live.Off                                                                                                                                                     |
| Role            | TextRole.Default                                                                                                                                             |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Error<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| X                      | 27                                                                                                                                                                              |
| Y                      | 31                                                                                                                                                                              |
| ZIndex                 | 3                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>  |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(237, 28, 36, 1)</td></tr><tr><td style="background-color:#ED1C24"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                          |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                         |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                             |
| FocusedBorderColor  | ErrorMessage9.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | ErrorMessage9.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | ErrorMessage9.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | ErrorMessage9.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | ErrorMessage9.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | ErrorMessage9.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | ErrorMessage9.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard9 |

## Group3

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![group](resources/group.png) | Type: group |

### Design

| Property | Value                                                                                                                                         |
| -------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Height   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| Width    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| X        | 0                                                                                                                                             |
| Y        | 0                                                                                                                                             |
| ZIndex   | 1                                                                                                                                             |

### Color Properties

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## Group4

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![group](resources/group.png) | Type: group |

### Design

| Property | Value |
| -------- | ----- |
| Height   | 5     |
| Width    | 5     |
| X        | 80    |
| Y        | 80    |
| ZIndex   | 54    |

### Color Properties

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## icon2\_10

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Behavior

| Property | Value                                                                                                                                                                                                                |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(AreaPage,ScreenTransition.Fade,{EditRecord:EditRecord,Area:Area})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.ChevronRight<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 683.3048225659651                                                                                                                                           |
| Y                      | 15.5                                                                                                                                                        |
| ZIndex                 | 10                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon2\_10.Fill                                                                                                                                                                                                                                                                                                                                |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon2\_10.BorderColor                                                                                                                                                                                                                                                                                                                         |
| HoverBorderColor    | ColorFade(icon2\_10.BorderColor, 20%)                                                                                                                                                                                                                                                                                                         |
| HoverColor          | ColorFade(icon2\_10.Color, 20%)                                                                                                                                                                                                                                                                                                               |
| HoverFill           | icon2\_10.Fill                                                                                                                                                                                                                                                                                                                                |
| PressedBorderColor  | ColorFade(icon2\_10.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                       |
| PressedColor        | ColorFade(icon2\_10.Color, \-20%)                                                                                                                                                                                                                                                                                                             |
| PressedFill         | icon2\_10.Fill                                                                                                                                                                                                                                                                                                                                |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard9 |

## icon2\_11

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Behavior

| Property | Value                                                                                                                                                                                                                            |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(PriorityPage,ScreenTransition.Fade,{EditRecord:EditRecord,priority:priority})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.ChevronRight<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 683.0964513193788                                                                                                                                           |
| Y                      | 17.5                                                                                                                                                        |
| ZIndex                 | 12                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon2\_11.Fill                                                                                                                                                                                                                                                                                                                                |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon2\_11.BorderColor                                                                                                                                                                                                                                                                                                                         |
| HoverBorderColor    | ColorFade(icon2\_11.BorderColor, 20%)                                                                                                                                                                                                                                                                                                         |
| HoverColor          | ColorFade(icon2\_11.Color, 20%)                                                                                                                                                                                                                                                                                                               |
| HoverFill           | icon2\_11.Fill                                                                                                                                                                                                                                                                                                                                |
| PressedBorderColor  | ColorFade(icon2\_11.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                       |
| PressedColor        | ColorFade(icon2\_11.Color, \-20%)                                                                                                                                                                                                                                                                                                             |
| PressedFill         | icon2\_11.Fill                                                                                                                                                                                                                                                                                                                                |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard10 |

## icon2\_8

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Behavior

| Property | Value                                                                                                                                                                                                                      |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(CasestatusPage,ScreenTransition.Fade,{EditRecord:EditRecord,type:type})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.ChevronRight<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 682.6934662447568                                                                                                                                           |
| Y                      | 17.5                                                                                                                                                        |
| ZIndex                 | 5                                                                                                                                                           |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon2\_8.Fill                                                                                                                                                                                                                                                                                                                                 |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon2\_8.BorderColor                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | ColorFade(icon2\_8.BorderColor, 20%)                                                                                                                                                                                                                                                                                                          |
| HoverColor          | ColorFade(icon2\_8.Color, 20%)                                                                                                                                                                                                                                                                                                                |
| HoverFill           | icon2\_8.Fill                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | ColorFade(icon2\_8.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                        |
| PressedColor        | ColorFade(icon2\_8.Color, \-20%)                                                                                                                                                                                                                                                                                                              |
| PressedFill         | icon2\_8.Fill                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard7 |

## icon2\_9

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Behavior

| Property | Value                                                                                                                                                                                                                        |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(AssigntoPage,ScreenTransition.Fade,{EditRecord:EditRecord,assign:assign})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.ChevronRight<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 683.0964513193778                                                                                                                                           |
| Y                      | 16                                                                                                                                                          |
| ZIndex                 | 8                                                                                                                                                           |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon2\_9.Fill                                                                                                                                                                                                                                                                                                                                 |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon2\_9.BorderColor                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | ColorFade(icon2\_9.BorderColor, 20%)                                                                                                                                                                                                                                                                                                          |
| HoverColor          | ColorFade(icon2\_9.Color, 20%)                                                                                                                                                                                                                                                                                                                |
| HoverFill           | icon2\_9.Fill                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | ColorFade(icon2\_9.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                        |
| PressedColor        | ColorFade(icon2\_9.Color, \-20%)                                                                                                                                                                                                                                                                                                              |
| PressedFill         | icon2\_9.Fill                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard8 |

## icon4

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Behavior

| Property | Value                                                                                                                                                                                                                              |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ResetForm(TicketDetailsForm);Navigate(DashboardPage, ScreenTransition.Fade,{type:"All"})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">28<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.ChevronLeft<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">28<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 16                                                                                                                                                          |
| Y                      | 16                                                                                                                                                          |
| ZIndex                 | 27                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon4.Fill                                                                                                                                                                                                                                                                                                                                    |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon4.BorderColor                                                                                                                                                                                                                                                                                                                             |
| HoverBorderColor    | ColorFade(icon4.BorderColor, 20%)                                                                                                                                                                                                                                                                                                             |
| HoverColor          | ColorFade(icon4.Color, 20%)                                                                                                                                                                                                                                                                                                                   |
| HoverFill           | icon4.Fill                                                                                                                                                                                                                                                                                                                                    |
| PressedBorderColor  | ColorFade(icon4.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                           |
| PressedColor        | ColorFade(icon4.Color, \-20%)                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | icon4.Fill                                                                                                                                                                                                                                                                                                                                    |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## Key10

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                              |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                       |
| Live            | Live.Off                                                                                                                                                           |
| Role            | TextRole.Default                                                                                                                                                   |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.DisplayName<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">53<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                 |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| PaddingBottom          | 5                                                                                                                                                                              |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| PaddingTop             | 5                                                                                                                                                                              |
| Size                   | 13                                                                                                                                                                             |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">180<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                               |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 0                                                                                                                                                                              |
| Y                      | 0                                                                                                                                                                              |
| ZIndex                 | 1                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key10.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | Key10.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverColor          | Key10.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| HoverFill           | Key10.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | Key10.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | Key10.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| PressedFill         | Key10.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard10 |

## Key14

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                              |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                       |
| Live            | Live.Off                                                                                                                                                           |
| Role            | TextRole.Default                                                                                                                                                   |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.DisplayName<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">72<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">18<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 30                                                                                                                                                                              |
| Y                      | 0                                                                                                                                                                               |
| ZIndex                 | 1                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key14.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | Key14.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverColor          | Key14.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| HoverFill           | Key14.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | Key14.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | Key14.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| PressedFill         | Key14.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard14 |

## Key3

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                              |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                       |
| Live            | Live.Off                                                                                                                                                           |
| Role            | TextRole.Default                                                                                                                                                   |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.DisplayName<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">57<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">18<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">19<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | 0.8620689655172414                                                                                                                                                              |
| ZIndex                 | 1                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverBorderColor    | Key3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverColor          | Key3.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverFill           | Key3.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedBorderColor  | Key3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| PressedColor        | Key3.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | Key3.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard4 |

## Key5

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                              |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                       |
| Live            | Live.Off                                                                                                                                                           |
| Role            | TextRole.Default                                                                                                                                                   |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.DisplayName<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | 40                                                                                                                                                                             |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">18<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">19<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 0                                                                                                                                                                              |
| Y                      | 0                                                                                                                                                                              |
| ZIndex                 | 1                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverBorderColor    | Key5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverColor          | Key5.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverFill           | Key5.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedBorderColor  | Key5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| PressedColor        | Key5.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | Key5.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard5 |

## Key6

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                        |
| Live            | Live.Off                                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Internal comments"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | 40                                                                                                                                                                             |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">18<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">19<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">24<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 0                                                                                                                                                                              |
| Y                      | 11.079545454545448                                                                                                                                                             |
| ZIndex                 | 1                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverBorderColor    | Key6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverColor          | Key6.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverFill           | Key6.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedBorderColor  | Key6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| PressedColor        | Key6.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | Key6.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard6 |

## Key7

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                           |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| Live            | Live.Off                                                                                                                                                        |
| Role            | TextRole.Default                                                                                                                                                |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Ticket status"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">54<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                 |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| PaddingBottom          | 5                                                                                                                                                                              |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| PaddingRight           | 5                                                                                                                                                                              |
| PaddingTop             | 5                                                                                                                                                                              |
| Size                   | 13                                                                                                                                                                             |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">200<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                               |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 0                                                                                                                                                                              |
| Y                      | 0                                                                                                                                                                              |
| ZIndex                 | 1                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key7.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverBorderColor    | Key7.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverColor          | Key7.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverFill           | Key7.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedBorderColor  | Key7.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| PressedColor        | Key7.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | Key7.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard7 |

## Key8

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| Live            | Live.Off                                                                                                                                                      |
| Role            | TextRole.Default                                                                                                                                              |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Assigned to"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">51<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                 |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| PaddingBottom          | 5                                                                                                                                                                              |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| PaddingRight           | 5                                                                                                                                                                              |
| PaddingTop             | 5                                                                                                                                                                              |
| Size                   | 13                                                                                                                                                                             |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">216<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                               |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 0                                                                                                                                                                              |
| Y                      | 0                                                                                                                                                                              |
| ZIndex                 | 1                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverBorderColor    | Key8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverColor          | Key8.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverFill           | Key8.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedBorderColor  | Key8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| PressedColor        | Key8.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | Key8.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard8 |

## Key9

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                  |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>           |
| Live            | Live.Off                                                                                                                                               |
| Role            | TextRole.Default                                                                                                                                       |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Area"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">51<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                 |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| PaddingBottom          | 5                                                                                                                                                                              |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| PaddingRight           | 5                                                                                                                                                                              |
| PaddingTop             | 5                                                                                                                                                                              |
| Size                   | 13                                                                                                                                                                             |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">159<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                               |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 0                                                                                                                                                                              |
| Y                      | 0                                                                                                                                                                              |
| ZIndex                 | 1                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key9.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverBorderColor    | Key9.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverColor          | Key9.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverFill           | Key9.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedBorderColor  | Key9.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| PressedColor        | Key9.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | Key9.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard9 |

## Rectangle1\_1

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X                      | 0                                                                                                                                                           |
| Y                      | 0                                                                                                                                                           |
| ZIndex                 | 5                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle1\_1.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_1.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle1\_1.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle1\_1.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## Rectangle1\_3

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                              |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ResetForm(TicketDetailsForm);Navigate(DashboardPage, ScreenTransition.Fade,{type:"All"})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 0                                                                                                                                                           |
| Y                      | 0                                                                                                                                                           |
| ZIndex                 | 26                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle1\_3.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_3.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle1\_3.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle1\_3.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## Rectangle10

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(AreaPage,ScreenTransition.Fade,{EditRecord:EditRecord,Area:Area})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">52<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">529<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 188                                                                                                                                                         |
| Y                      | 0                                                                                                                                                           |
| ZIndex                 | 11                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle10.Fill                                                                                                                                                                                                                                                                                                                       |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>   |
| FocusedBorderColor | Rectangle10.BorderColor                                                                                                                                                                                                                                                                                                                |
| HoverFill          | Rectangle10.Fill                                                                                                                                                                                                                                                                                                                       |
| PressedFill        | Rectangle10.Fill                                                                                                                                                                                                                                                                                                                       |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard9 |

## Rectangle11

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                            |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(PriorityPage,ScreenTransition.Fade,{EditRecord:EditRecord,priority:priority})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">53<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">530<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 187                                                                                                                                                         |
| Y                      | 1                                                                                                                                                           |
| ZIndex                 | 13                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle11.Fill                                                                                                                                                                                                                                                                                                                       |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>   |
| FocusedBorderColor | Rectangle11.BorderColor                                                                                                                                                                                                                                                                                                                |
| HoverFill          | Rectangle11.Fill                                                                                                                                                                                                                                                                                                                       |
| PressedFill        | Rectangle11.Fill                                                                                                                                                                                                                                                                                                                       |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard10 |

## Rectangle3\_1

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                         |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">UpdateContext({subjectdisabled:false,subjectbordercolor:RGBA(230,230,230,1),subjectfill:RGBA(255,255,255,1),subject_visible:false})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">47<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">subject_visible<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">676<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 21                                                                                                                                                          |
| Y                      | 54                                                                                                                                                          |
| ZIndex                 | 5                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle3\_1.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>   |
| FocusedBorderColor | Rectangle3\_1.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle3\_1.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle3\_1.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard4 |

## Rectangle5\_7

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">709.2048192771084<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">307<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 59                                                                                                                                                          |
| ZIndex                 | 4                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle5\_7.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(212, 193, 221,.3)</td></tr><tr><td style="background-color:#D4C1DD"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle5\_7.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle5\_7.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle5\_7.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## Rectangle6\_2

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                            |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">UpdateContext({description_disabled:false,description_bordercolor:RGBA(230,230,230,1),description_fill:RGBA(255,255,255,1),description_visible:false})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                         |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>    |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">63<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">description_visible<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">676.9137931034481<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| X                      | 20.086206896551758                                                                                                                                            |
| Y                      | 40.92610837438432                                                                                                                                             |
| ZIndex                 | 6                                                                                                                                                             |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle6\_2.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>   |
| FocusedBorderColor | Rectangle6\_2.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle6\_2.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle6\_2.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard5 |

## Rectangle6\_3

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                        |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">UpdateContext({commentdisabled:false,commentbordercolor:RGBA(230,230,230,1),commentfill:RGBA(255,255,255,1),commentvisible:false})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">45.8235294117647<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">commentvisible<td style="background-color:#ffcccc; width:50%;"></td></tr></table>    |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">675<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 21                                                                                                                                                          |
| Y                      | 52.1764705882353                                                                                                                                            |
| ZIndex                 | 7                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle6\_3.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>   |
| FocusedBorderColor | Rectangle6\_3.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle6\_3.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle6\_3.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard6 |

## Rectangle7\_11

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">716<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 1                                                                                                                                                           |
| Y                      | 126.44827586206895                                                                                                                                          |
| ZIndex                 | 14                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_11.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_11.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_11.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_11.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard4 |

## Rectangle7\_24

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 134.51363461977453                                                                                                                                          |
| ZIndex                 | 15                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_24.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_24.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_24.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_24.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard5 |

## Rectangle7\_25

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 128.92307692307693                                                                                                                                          |
| ZIndex                 | 16                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_25.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_25.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_25.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_25.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard6 |

## Rectangle7\_26

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 54                                                                                                                                                          |
| ZIndex                 | 17                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_26.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_26.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_26.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_26.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard7 |

## Rectangle7\_27

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 51                                                                                                                                                          |
| ZIndex                 | 18                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_27.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_27.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_27.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_27.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard8 |

## Rectangle7\_28

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 51                                                                                                                                                          |
| ZIndex                 | 19                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_28.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_28.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_28.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_28.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard9 |

## Rectangle7\_29

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 53                                                                                                                                                          |
| ZIndex                 | 20                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_29.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_29.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_29.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_29.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard10 |

## Rectangle8

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                               |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate( CasestatusPage, ScreenTransition.Fade, { EditRecord: EditRecord, type: type } )<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">55<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">523<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 194                                                                                                                                                         |
| Y                      | 0                                                                                                                                                           |
| ZIndex                 | 6                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle8.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>   |
| FocusedBorderColor | Rectangle8.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle8.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle8.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard7 |

## Rectangle9

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                        |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(AssigntoPage,ScreenTransition.Fade,{EditRecord:EditRecord,assign:assign})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                       |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">52<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">529<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 188                                                                                                                                                         |
| Y                      | 0                                                                                                                                                           |
| ZIndex                 | 9                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle9.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>   |
| FocusedBorderColor | Rectangle9.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle9.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle9.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard8 |

## StarVisible10

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                               |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Live            | Live.Off                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"*"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Align.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>                |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key10.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                        |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key10.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                  |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key10.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key10.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key10.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key10.Y                                                                                                                                                                         |
| ZIndex                 | 4                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | StarVisible10.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | StarVisible10.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | StarVisible10.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | StarVisible10.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | StarVisible10.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | StarVisible10.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | StarVisible10.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard10 |

## StarVisible14

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                               |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Live            | Live.Off                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"*"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Align.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>                |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key14.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                        |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key14.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                  |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key14.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key14.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key14.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key14.Y                                                                                                                                                                         |
| ZIndex                 | 4                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | StarVisible14.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | StarVisible14.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | StarVisible14.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | StarVisible14.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | StarVisible14.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | StarVisible14.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | StarVisible14.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard14 |

## StarVisible3

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                               |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Live            | Live.Off                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"*"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Align.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>                |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key3.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                         |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key3.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key3.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key3.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key3.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                      |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key3.Y                                                                                                                                                                          |
| ZIndex                 | 4                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | StarVisible3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | StarVisible3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | StarVisible3.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | StarVisible3.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | StarVisible3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | StarVisible3.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | StarVisible3.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard4 |

## StarVisible5

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                               |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Live            | Live.Off                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"*"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Align.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>                |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key5.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                         |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key5.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key5.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key5.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key5.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                      |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key5.Y                                                                                                                                                                          |
| ZIndex                 | 4                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | StarVisible5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | StarVisible5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | StarVisible5.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | StarVisible5.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | StarVisible5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | StarVisible5.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | StarVisible5.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard5 |

## StarVisible6

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                               |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Live            | Live.Off                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"*"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Align.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>                |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key6.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                         |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key6.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key6.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key6.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key6.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                      |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key6.Y                                                                                                                                                                          |
| ZIndex                 | 4                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | StarVisible6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | StarVisible6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | StarVisible6.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | StarVisible6.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | StarVisible6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | StarVisible6.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | StarVisible6.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard6 |

## StarVisible7

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                               |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Live            | Live.Off                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"*"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Align.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>                |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key7.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                         |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key7.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key7.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key7.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key7.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                      |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key7.Y                                                                                                                                                                          |
| ZIndex                 | 3                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | StarVisible7.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | StarVisible7.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | StarVisible7.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | StarVisible7.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | StarVisible7.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | StarVisible7.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | StarVisible7.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard7 |

## StarVisible8

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                               |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Live            | Live.Off                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"*"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Align.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>                |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key8.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                         |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key8.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key8.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key8.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key8.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                      |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key8.Y                                                                                                                                                                          |
| ZIndex                 | 4                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | StarVisible8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | StarVisible8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | StarVisible8.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | StarVisible8.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | StarVisible8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | StarVisible8.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | StarVisible8.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard8 |

## StarVisible9

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                               |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Live            | Live.Off                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"*"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Align.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>                |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key9.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                         |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key9.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key9.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key9.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key9.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                      |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key9.Y                                                                                                                                                                          |
| ZIndex                 | 4                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | StarVisible9.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | StarVisible9.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | StarVisible9.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | StarVisible9.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | StarVisible9.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | StarVisible9.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | StarVisible9.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard9 |

## TextBox3

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                   |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>            |
| Live            | Live.Off                                                                                                                                                |
| Role            | TextRole.Default                                                                                                                                        |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Today()<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | 40                                                                                                                                                                              |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | 150                                                                                                                                                                             |
| X                      | 40                                                                                                                                                                              |
| Y                      | 40                                                                                                                                                                              |
| ZIndex                 | 48                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47,41,43,1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverBorderColor    | TextBox3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverColor          | TextBox3.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverFill           | TextBox3.Fill                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | TextBox3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedColor        | TextBox3.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedFill         | TextBox3.Fill                                                                                                                                                                                                                                                                                                                                                                                              |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## TextBox4\_1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                            |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                     |
| Live            | Live.Off                                                                                                                                                         |
| Role            | TextRole.Default                                                                                                                                                 |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Ticket details"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table> |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                           |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                            |
| FocusedBorderThickness | 0                                                                                                                                                                           |
| Font                   | Font.'Open Sans'                                                                                                                                                            |
| FontWeight             | FontWeight.Normal                                                                                                                                                           |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                              |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| Overflow               | Overflow.Hidden                                                                                                                                                             |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                        |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                           |
| X                      | 0                                                                                                                                                                           |
| Y                      | 0                                                                                                                                                                           |
| ZIndex                 | 6                                                                                                                                                                           |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                           |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | TextBox4\_1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverBorderColor    | TextBox4\_1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverColor          | TextBox4\_1.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverFill           | TextBox4\_1.Fill                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | TextBox4\_1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedColor        | TextBox4\_1.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedFill         | TextBox4\_1.Fill                                                                                                                                                                                                                                                                                                                                                                                              |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## TextBox5\_50

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                       |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Live            | Live.Off                                                                                                                                                    |
| Role            | TextRole.Default                                                                                                                                            |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Ticket ID"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| BorderThickness        | 0                                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Rectangle5_7.Width<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | 82                                                                                                                                                                              |
| ZIndex                 | 24                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_50.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_50.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_50.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_50.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_50.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_50.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_50.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## TextBox5\_51

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                          |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| Live            | Live.Off                                                                                                                                                       |
| Role            | TextRole.Default                                                                                                                                               |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Created date"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| BorderThickness        | 0                                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Rectangle5_7.Width<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | 166                                                                                                                                                                             |
| ZIndex                 | 51                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_51.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_51.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_51.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_51.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_51.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_51.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_51.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## TextBox5\_52

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| Live            | Live.Off                                                                                                                                                      |
| Role            | TextRole.Default                                                                                                                                              |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Closed date"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| BorderThickness        | 0                                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Rectangle5_7.Width<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | 251                                                                                                                                                                             |
| ZIndex                 | 22                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_52.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_52.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_52.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_52.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_52.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_52.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_52.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## TextBox5\_55

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                        |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Live            | Live.Off                                                                                                                                                     |
| Role            | TextRole.Default                                                                                                                                             |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Created by"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| BorderThickness        | 0                                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                 |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Rectangle5_7.Width<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                |
| X                      | 0                                                                                                                                                                              |
| Y                      | 344                                                                                                                                                                            |
| ZIndex                 | 18                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_55.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_55.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_55.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_55.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_55.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_55.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_55.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## TextBox5\_56

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| Live            | Live.Off                                                                                                                                                      |
| Role            | TextRole.Default                                                                                                                                              |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditRecord.ID<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| BorderThickness        | 0                                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Lighter<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>   |
| Height                 | 40                                                                                                                                                                              |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">14<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Rectangle5_7.Width<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | 112                                                                                                                                                                             |
| ZIndex                 | 25                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_56.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_56.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_56.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_56.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_56.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_56.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_56.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## TextBox5\_57

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                                  |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                           |
| Live            | Live.Off                                                                                                                                                               |
| Role            | TextRole.Default                                                                                                                                                       |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditRecord.DateCreated<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| BorderThickness        | 0                                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Lighter<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>   |
| Height                 | 40                                                                                                                                                                              |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">14<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Rectangle5_7.Width<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | 196                                                                                                                                                                             |
| ZIndex                 | 52                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_57.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_57.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_57.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_57.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_57.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_57.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_57.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## TextBox5\_58

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                            |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                     |
| Live            | Live.Off                                                                                                                                                         |
| Role            | TextRole.Default                                                                                                                                                 |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditRecord.Owner<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| BorderThickness        | 0                                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Lighter<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>   |
| Height                 | 40                                                                                                                                                                              |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">14<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Rectangle5_7.Width<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | 374                                                                                                                                                                             |
| ZIndex                 | 23                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_58.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_58.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_58.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_58.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_58.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_58.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_58.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## TextBox5\_61

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                                                                                                                                         |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                                                  |
| Live            | Live.Off                                                                                                                                                                                                                                                                      |
| Role            | TextRole.Default                                                                                                                                                                                                                                                              |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(IsBlank(EditRecord.DateClosed),"--",EditRecord.DateClosed) //If(IsBlank(EditRecord.DateClosed),"--",EditRecord.DateClosed)<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                         |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                    |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                             |
| BorderThickness        | 0                                                                                                                                                                             |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                              |
| FocusedBorderThickness | 0                                                                                                                                                                             |
| Font                   | Font.'Open Sans'                                                                                                                                                              |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Lighter<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | 40                                                                                                                                                                            |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                               |
| Italic                 | false                                                                                                                                                                         |
| Overflow               | Overflow.Hidden                                                                                                                                                               |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                 |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">14<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                          |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Rectangle5_7.Width<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>               |
| X                      | 0                                                                                                                                                                             |
| Y                      | 281                                                                                                                                                                           |
| ZIndex                 | 19                                                                                                                                                                            |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_61.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_61.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_61.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_61.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_61.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_61.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_61.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Parent Control | TicketdetailsPage |

## TicketDetailsForm

| Property                    | Value      |
| --------------------------- | ---------- |
| ![form](resources/form.png) | Type: form |

### Behavior

| Property  | Value                                                                                                                                                                                   |
| --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSuccess | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(DashboardPage,ScreenTransition.Fade)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                             |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                      |
| DataSource      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Tickets<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| DefaultMode     | FormMode.Edit                                                                                                                                                     |
| Item            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">TicketsGallery.Selected<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                          |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AcceptsFocus           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| BorderStyle            | BorderStyle.Solid                                                                                                                                              |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">4<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">657.9844961240301<td style="background-color:#ffcccc; width:50%;">500</td></tr></table> |
| NumberOfColumns        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| SnapToColumns          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">717<td style="background-color:#ffcccc; width:50%;">800</td></tr></table>               |
| X                      | 307                                                                                                                                                            |
| Y                      | 60                                                                                                                                                             |
| ZIndex                 | 53                                                                                                                                                             |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(180, 180, 180, 1)</td></tr><tr><td style="background-color:#B4B4B4"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, 1)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>    |
| FocusedBorderColor | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value             |
| -------------- | ----------------- |
| Child Control  | DataCard4         |
| Child Control  | DataCard5         |
| Child Control  | DataCard6         |
| Child Control  | DataCard7         |
| Child Control  | DataCard8         |
| Child Control  | DataCard9         |
| Child Control  | DataCard14        |
| Child Control  | DataCard10        |
| Parent Control | TicketdetailsPage |

## Value1

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                                |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                         |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                         |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Default<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                                |
| MaxLength       |                                                                                                                                                                      |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| BorderThickness        | 2                                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| EnableSpellCheck       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">3<td style="background-color:#ffcccc; width:50%;">4</td></tr></table>                                    |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Format                 | TextFormat.Text                                                                                                                                                                 |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">47<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| Mode                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">TextMode.MultiLine<td style="background-color:#ffcccc; width:50%;">TextMode.SingleLine</td></tr></table> |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                     |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                     |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                     |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                     |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">11<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                     |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                                                        |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">676.051724137931<td style="background-color:#ffcccc; width:50%;">320</td></tr></table>                   |
| X                      | 20.948275862068996                                                                                                                                                              |
| Y                      | 54.413793103448285                                                                                                                                                              |
| ZIndex                 | 2                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | If(IsBlank(Parent.Error),  RGBA(204, 204, 204, 1), Color.Red)                                                                                                                                                                                                                                                                                                                                                       |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | Value1.Color                                                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | Value1.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |
| Fill                | subjectfill                                                                                                                                                                                                                                                                                                                                                                                                         |
| FocusedBorderColor  | Value1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204,204,204,1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>       |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | Value1.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | Value1.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedColor        | Value1.Color                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | Value1.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard4 |

## Value12

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                                                                                                   |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                            |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                            |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(type = "Closed", Today(), "")  // If(Parent.Default = "Closed", Today(), "--")<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                                                                                                   |

### Design

| Property               | Value                                                                                                                                                          |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                              |
| BorderThickness        | 2                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                               |
| EnableSpellCheck       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">3<td style="background-color:#ffcccc; width:50%;">4</td></tr></table>                   |
| Font                   | Font.'Open Sans'                                                                                                                                               |
| FontWeight             | FontWeight.Normal                                                                                                                                              |
| Format                 | TextFormat.Text                                                                                                                                                |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">52<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                 |
| Mode                   | TextMode.SingleLine                                                                                                                                            |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| Size                   | 13                                                                                                                                                             |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                                       |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Width - 60<td style="background-color:#ffcccc; width:50%;">320</td></tr></table> |
| X                      | 30                                                                                                                                                             |
| Y                      | Key14.Height                                                                                                                                                   |
| ZIndex                 | 2                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | If(IsBlank(Parent.Error), Parent.BorderColor, Color.Red)                                                                                                                                                                                                                                                                                                                                                            |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 1)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                              |
| Fill                | <table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | Value12.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101, 128, 187, 1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | ColorFade(RGBA(190, 202, 226, 1), 30%)                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | Value12.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                            |
| PressedColor        | Value12.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedFill         | Value12.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard14 |

## Value2

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                                |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                         |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                         |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Default<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                                |

### Design

| Property               | Value                                                                                                                                                                                                                    |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                                                                                               |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                                                                        |
| BorderThickness        | 2                                                                                                                                                                                                                        |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(description_disabled,DisplayMode.Disabled,DisplayMode.Edit)<td style="background-color:#ffcccc; width:50%;">DisplayMode.Edit</td></tr></table> |
| EnableSpellCheck       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                          |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">3<td style="background-color:#ffcccc; width:50%;">4</td></tr></table>                                                                             |
| Font                   | Font.'Open Sans'                                                                                                                                                                                                         |
| FontWeight             | FontWeight.Normal                                                                                                                                                                                                        |
| Format                 | TextFormat.Text                                                                                                                                                                                                          |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">62.142857142857196<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                                           |
| Mode                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">TextMode.MultiLine<td style="background-color:#ffcccc; width:50%;">TextMode.SingleLine</td></tr></table>                                          |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                              |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                              |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                              |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                              |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                                             |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                                             |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                                             |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                                             |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">11<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                                                           |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                              |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                                                                                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">676.051724137931<td style="background-color:#ffcccc; width:50%;">320</td></tr></table>                                                            |
| X                      | 20.948275862068996                                                                                                                                                                                                       |
| Y                      | 41.637931034482804                                                                                                                                                                                                       |
| ZIndex                 | 2                                                                                                                                                                                                                        |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | If(IsBlank(Parent.Error),  RGBA(204, 204, 204, 1), Color.Red)                                                                                                                                                                                                                                                                                                                                                       |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | Value2.Color                                                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | Value2.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |
| Fill                | description\_fill                                                                                                                                                                                                                                                                                                                                                                                                   |
| FocusedBorderColor  | Value2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204,204,204,1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>       |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | Value2.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | Value2.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedColor        | Value2.Color                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | Value2.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard5 |

## Value3

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                                |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                         |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                         |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Parent.Default<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                                |

### Design

| Property               | Value                                                                                                                                                                                                               |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                                                          |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                                                                   |
| BorderThickness        | 2                                                                                                                                                                                                                   |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(commentdisabled,DisplayMode.Disabled,DisplayMode.Edit)<td style="background-color:#ffcccc; width:50%;">DisplayMode.Edit</td></tr></table> |
| EnableSpellCheck       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                     |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">3<td style="background-color:#ffcccc; width:50%;">4</td></tr></table>                                                                        |
| Font                   | Font.'Open Sans'                                                                                                                                                                                                    |
| FontWeight             | FontWeight.Normal                                                                                                                                                                                                   |
| Format                 | TextFormat.Text                                                                                                                                                                                                     |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">46<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                                                      |
| Mode                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">TextMode.MultiLine<td style="background-color:#ffcccc; width:50%;">TextMode.SingleLine</td></tr></table>                                     |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                         |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                         |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                         |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">8<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                         |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                                        |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                                        |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                                        |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                                        |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">11<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                                                      |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                         |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                                                                                            |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">674.6153846153846<td style="background-color:#ffcccc; width:50%;">320</td></tr></table>                                                      |
| X                      | 21.384615384615415                                                                                                                                                                                                  |
| Y                      | 52.92569930069919                                                                                                                                                                                                   |
| ZIndex                 | 2                                                                                                                                                                                                                   |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | If(IsBlank(Parent.Error),  RGBA(204, 204, 204, 1), Color.Red)                                                                                                                                                                                                                                                                                                                                                       |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | Value3.Color                                                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | Value3.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |
| Fill                | commentfill                                                                                                                                                                                                                                                                                                                                                                                                         |
| FocusedBorderColor  | Value3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204,204,204,1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>       |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | Value3.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | Value3.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedColor        | Value3.Color                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | Value3.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard6 |

## Value5

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Behavior

| Property | Value                                                                                                                                                                                                                      |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(CasestatusPage,ScreenTransition.Fade,{EditRecord:EditRecord,type:type})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                      |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">type<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                      |

### Design

| Property               | Value                                                                                                                                            |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                       |
| BorderStyle            | BorderStyle.Solid                                                                                                                                |
| BorderThickness        | 2                                                                                                                                                |
| DisplayMode            | DisplayMode.Edit                                                                                                                                 |
| EnableSpellCheck       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">3<td style="background-color:#ffcccc; width:50%;">4</td></tr></table>     |
| Font                   | Font.'Open Sans'                                                                                                                                 |
| FontWeight             | FontWeight.Normal                                                                                                                                |
| Format                 | TextFormat.Text                                                                                                                                  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">54<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>   |
| Mode                   | TextMode.SingleLine                                                                                                                              |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| Size                   | 13                                                                                                                                               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                         |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">197<td style="background-color:#ffcccc; width:50%;">320</td></tr></table> |
| X                      | 193.57142857142804                                                                                                                               |
| Y                      | 0                                                                                                                                                |
| ZIndex                 | 4                                                                                                                                                |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | If(IsBlank(Parent.Error), RGBA(0,0,0,0), Color.Red)                                                                                                                                                                                                                                                                                                                                                                 |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 0)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 0)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table>    |
| DisabledFill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 0)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(244, 244, 244, 1)</td></tr><tr><td style="background-color:#F4F4F4"></td></tr></table></td></tr></table> |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 0)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |
| FocusedBorderColor  | Value5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101, 128, 187, 0)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(190, 202, 226, 0)</td></tr><tr><td style="background-color:#BECAE2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(186, 202, 226, 1)</td></tr><tr><td style="background-color:#BACAE2"></td></tr></table></td></tr></table> |
| PressedBorderColor  | Value5.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedColor        | Value5.Color                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | Value5.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard7 |

## Value6

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Behavior

| Property | Value                                                                                                                                                                                                                        |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(AssigntoPage,ScreenTransition.Fade,{EditRecord:EditRecord,assign:assign})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                                   |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                            |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                            |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(IsBlank(assign),"None",assign)<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                                                   |

### Design

| Property               | Value                                                                                                                                                                                                     |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                                                |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                                                         |
| BorderThickness        | 2                                                                                                                                                                                                         |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(false,DisplayMode.Disabled,DisplayMode.Edit)<td style="background-color:#ffcccc; width:50%;">DisplayMode.Edit</td></tr></table> |
| EnableSpellCheck       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                           |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">3<td style="background-color:#ffcccc; width:50%;">4</td></tr></table>                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                                                          |
| FontWeight             | FontWeight.Normal                                                                                                                                                                                         |
| Format                 | TextFormat.Text                                                                                                                                                                                           |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">51<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                                            |
| Mode                   | TextMode.SingleLine                                                                                                                                                                                       |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                               |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                              |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                               |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                               |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                              |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                              |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                              |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                                              |
| Size                   | 13                                                                                                                                                                                                        |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                               |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                                                                                  |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">352<td style="background-color:#ffcccc; width:50%;">320</td></tr></table>                                                          |
| X                      | 187.85714285714232                                                                                                                                                                                        |
| Y                      | 0                                                                                                                                                                                                         |
| ZIndex                 | 2                                                                                                                                                                                                         |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | If(IsBlank(Parent.Error), RGBA(204,204,204,0), Color.Red)                                                                                                                                                                                                                                                                                                                                                           |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 0)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 0)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table>    |
| DisabledFill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 0)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(244, 244, 244, 1)</td></tr><tr><td style="background-color:#F4F4F4"></td></tr></table></td></tr></table> |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 0)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |
| FocusedBorderColor  | Value6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101, 128, 187, 0)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(190, 202, 226, 0)</td></tr><tr><td style="background-color:#BECAE2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(186, 202, 226, 1)</td></tr><tr><td style="background-color:#BACAE2"></td></tr></table></td></tr></table> |
| PressedBorderColor  | Value6.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedColor        | Value6.Color                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | Value6.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard8 |

## Value7

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Behavior

| Property | Value                                                                                                                                                                                                                |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(AreaPage,ScreenTransition.Fade,{EditRecord:EditRecord,Area:Area})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                      |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Area<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                      |

### Design

| Property               | Value                                                                                                                                            |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                       |
| BorderStyle            | BorderStyle.Solid                                                                                                                                |
| BorderThickness        | 2                                                                                                                                                |
| DisplayMode            | DisplayMode.Edit                                                                                                                                 |
| EnableSpellCheck       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">3<td style="background-color:#ffcccc; width:50%;">4</td></tr></table>     |
| Font                   | Font.'Open Sans'                                                                                                                                 |
| FontWeight             | FontWeight.Normal                                                                                                                                |
| Format                 | TextFormat.Text                                                                                                                                  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">51<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>   |
| Mode                   | TextMode.SingleLine                                                                                                                              |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;"></td></tr></table>     |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| Size                   | 13                                                                                                                                               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                         |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">225<td style="background-color:#ffcccc; width:50%;">320</td></tr></table> |
| X                      | 187.56503198294263                                                                                                                               |
| Y                      | 0                                                                                                                                                |
| ZIndex                 | 2                                                                                                                                                |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | If(IsBlank(Parent.Error), RGBA(0,0,0,0), Color.Red)                                                                                                                                                                                                                                                                                                                                                                 |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 0)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 0), 70%)                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 0), 50%)                                                                                                                                                                                                                                                                                                                                                                              |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 0)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |
| FocusedBorderColor  | Value7.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101, 128, 187, 0)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | ColorFade(RGBA(190, 202, 226, 0), 30%)                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | Value7.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedColor        | Value7.Color                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | Value7.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value     |
| -------------- | --------- |
| Parent Control | DataCard9 |

## Value8

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                          |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">priority<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                          |

### Design

| Property               | Value                                                                                                                                            |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                       |
| BorderStyle            | BorderStyle.Solid                                                                                                                                |
| BorderThickness        | 2                                                                                                                                                |
| DisplayMode            | DisplayMode.Edit                                                                                                                                 |
| EnableSpellCheck       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">3<td style="background-color:#ffcccc; width:50%;">4</td></tr></table>     |
| Font                   | Font.'Open Sans'                                                                                                                                 |
| FontWeight             | FontWeight.Normal                                                                                                                                |
| Format                 | TextFormat.Text                                                                                                                                  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">52<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>   |
| Mode                   | TextMode.SingleLine                                                                                                                              |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;"></td></tr></table>     |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">5<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>     |
| Size                   | 13                                                                                                                                               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                         |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">190<td style="background-color:#ffcccc; width:50%;">320</td></tr></table> |
| X                      | 187.28571428571422                                                                                                                               |
| Y                      | 1                                                                                                                                                |
| ZIndex                 | 2                                                                                                                                                |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | If(IsBlank(Parent.Error), RGBA(0,0,0,0), Color.Red)                                                                                                                                                                                                                                                                                                                                                                 |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 0)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 0), 70%)                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 0), 50%)                                                                                                                                                                                                                                                                                                                                                                              |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 0)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |
| FocusedBorderColor  | Value8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101, 128, 187, 0)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | ColorFade(RGBA(190, 202, 226, 0), 30%)                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | Value8.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedColor        | Value8.Color                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | Value8.Fill                                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard10 |
