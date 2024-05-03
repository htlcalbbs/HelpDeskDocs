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

## CreatenewticketPage

| Property                        | Value        |
| ------------------------------- | ------------ |
| ![screen](resources/screen.png) | Type: screen |

### Behavior

| Property  | Value                                                                                                                                                                        |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnVisible | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">UpdateContext({msg_visible:false})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value |
| --------------- | ----- |
| BackgroundImage |       |

### Design

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Height              | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Max(App.Height, App.DesignHeight)<td style="background-color:#ffcccc; width:50%;">Max(App.Height, App.MinScreenHeight)</td></tr></table>                                                                                                                                                                                                |
| ImagePosition       | ImagePosition.Fit                                                                                                                                                                                                                                                                                                                                                                                              |
| LoadingSpinner      | LoadingSpinner.None                                                                                                                                                                                                                                                                                                                                                                                            |
| LoadingSpinnerColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 51, 102, 1)</td></tr><tr><td style="background-color:#003366"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table> |
| Orientation         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(CreatenewticketPage.Width < CreatenewticketPage.Height, Layout.Vertical, Layout.Horizontal)<td style="background-color:#ffcccc; width:50%;">If(Self.Width < Self.Height, Layout.Vertical, Layout.Horizontal)</td></tr></table>                                                                                                       |
| Size                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1 + CountRows(App.SizeBreakpoints) - CountIf(App.SizeBreakpoints, Value >= CreatenewticketPage.Width)<td style="background-color:#ffcccc; width:50%;">1 + CountRows(App.SizeBreakpoints) - CountIf(App.SizeBreakpoints, Value >= Self.Width)</td></tr></table>                                                                          |
| Width               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Max(App.Width, App.DesignWidth)<td style="background-color:#ffcccc; width:50%;">Max(App.Width, App.MinScreenWidth)</td></tr></table>                                                                                                                                                                                                    |

### Color Properties

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                              |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fill     | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>White</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property      | Value          |
| ------------- | -------------- |
| Child Control | Rectangle1\_6  |
| Child Control | TextBox4\_3    |
| Child Control | Rectangle1\_7  |
| Child Control | icon6          |
| Child Control | TextBox1\_25   |
| Child Control | TextBox1\_26   |
| Child Control | TextBox1\_27   |
| Child Control | TextBox1\_28   |
| Child Control | TextBox1\_29   |
| Child Control | Rectangle1\_8  |
| Child Control | Rectangle6\_15 |
| Child Control | Rectangle6\_16 |
| Child Control | Rectangle6\_17 |
| Child Control | Rectangle6\_18 |
| Child Control | Rectangle6\_19 |
| Child Control | TextBox2\_25   |
| Child Control | TextBox2\_26   |
| Child Control | TextBox2\_27   |
| Child Control | TextBox2\_28   |
| Child Control | TextBox2\_29   |
| Child Control | Rectangle7\_23 |
| Child Control | NewTicketForm  |
| Child Control | TextBox5\_43   |
| Child Control | Subject        |
| Child Control | TextBox5\_44   |
| Child Control | Description    |
| Child Control | TextBox2       |
| Child Control | Button1\_1     |
| Child Control | Group7         |
| Child Control | Group2\_1      |
| Child Control | Group11\_1     |
| Child Control | Group12\_1     |
| Child Control | Group13\_1     |
| Child Control | Group14\_1     |

## Button1\_1

| Property                        | Value        |
| ------------------------------- | ------------ |
| ![button](resources/button.png) | Type: button |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If( IsBlank(Subject.Text) || IsBlank(Description.Text), UpdateContext({msg_visible: true}), SubmitForm(NewTicketForm); UpdateContext( { New: Patch( Tickets, LookUp( Tickets, ID = NewTicketForm.LastSubmit.ID //Text(Max(Tickets,ID)) ), { //ID: Max(Tickets, ID) + 1, Subject: Subject.Text, Description: Description.Text } ) } ) )<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                             |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                      |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Create ticket"<td style="background-color:#ffcccc; width:50%;">"Button"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                             |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Center                                                                                                                                      |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| BorderStyle            | BorderStyle.Solid                                                                                                                                 |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">2</td></tr></table>      |
| DisplayMode            | DisplayMode.Edit                                                                                                                                  |
| FocusedBorderThickness | 4                                                                                                                                                 |
| Font                   | Font.'Open Sans'                                                                                                                                  |
| FontWeight             | FontWeight.Semibold                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">50<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>    |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">10</td></tr></table>     |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">10</td></tr></table>     |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">10</td></tr></table>     |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">10</td></tr></table>     |
| Size                   | 15                                                                                                                                                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>       |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                              |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;">160</td></tr></table> |
| X                      | 0                                                                                                                                                 |
| Y                      | 718                                                                                                                                               |
| ZIndex                 | 13                                                                                                                                                |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | ColorFade(Button1\_1.Fill, \-15%)                                                                                                                                                                                                                                                                                                                                                                                |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |
| DisabledBorderColor | ColorFade(Button1\_1.BorderColor, 70%)                                                                                                                                                                                                                                                                                                                                                                           |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                              |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                           |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(107,0,64,.8)</td></tr><tr><td style="background-color:#6B0040"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table>     |
| FocusedBorderColor  | Button1\_1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverBorderColor    | Button1\_1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverColor          | Button1\_1.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverFill           | Button1\_1.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedBorderColor  | Button1\_1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| PressedColor        | Button1\_1.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | ColorFade(Button1\_1.Fill, 20%)                                                                                                                                                                                                                                                                                                                                                                                  |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## DataCard15

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                    |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Owner"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.Owner<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Created by *"<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>           |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value13.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |

### Design

| Property    | Value                                                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">80<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">401.05714634486605<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X           | 0                                                                                                                                                            |
| Y           | 0                                                                                                                                                            |
| ZIndex      | 1                                                                                                                                                            |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                   |
| ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230,230,230,1)</td></tr><tr><td style="background-color:#E6E6E6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>    |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Child Control  | Key15          |
| Child Control  | StarVisible15  |
| Child Control  | Value13        |
| Child Control  | ErrorMessage15 |
| Parent Control | NewTicketForm  |

## DataCard16

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                                                                                 |
| ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Priority"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                  |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.Priority<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                           |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Priority *"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                        |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Dropdown4.SelectedText.'data-ADB4D7A662F548B49FAC2B986E348A1BPriorityTypes'<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property    | Value                                                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">109.30769230769218<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">401.05714634486605<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X           | 0                                                                                                                                                            |
| Y           | 1                                                                                                                                                            |
| ZIndex      | 2                                                                                                                                                            |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                   |
| ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230,230,230,1)</td></tr><tr><td style="background-color:#E6E6E6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>    |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Child Control  | Key16          |
| Child Control  | StarVisible16  |
| Child Control  | Dropdown4      |
| Child Control  | ErrorMessage16 |
| Parent Control | NewTicketForm  |

## DataCard17

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                                                                                    |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"AccountName"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                  |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.AccountName<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                           |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Area *"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                       |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                           |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Dropdown5.SelectedText.'data-ADB4D7A662F548B49FAC2B986E348A1BAccountNameTypes'<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property    | Value                                                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">138<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">401.05714634486605<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X           | 0                                                                                                                                                            |
| Y           | 2                                                                                                                                                            |
| ZIndex      | 3                                                                                                                                                            |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                   |
| ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230,230,230,1)</td></tr><tr><td style="background-color:#E6E6E6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>    |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Child Control  | Key17          |
| Child Control  | StarVisible17  |
| Child Control  | Dropdown5      |
| Child Control  | ErrorMessage17 |
| Parent Control | NewTicketForm  |

## DataCard19

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
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value17.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>    |

### Design

| Property    | Value                                                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">80<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Visible     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">401.05714634486605<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X           | 0                                                                                                                                                            |
| Y           | 3                                                                                                                                                            |
| ZIndex      | 5                                                                                                                                                            |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Child Control  | StarVisible19  |
| Child Control  | Key19          |
| Child Control  | Value17        |
| Child Control  | ErrorMessage19 |
| Parent Control | NewTicketForm  |

## DataCard20

| Property                                      | Value               |
| --------------------------------------------- | ------------------- |
| ![typedDataCard](resources/typedDataCard.png) | Type: typedDataCard |

### Data

| Property    | Value                                                                                                                                                          |
| ----------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| DataField   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"DateCreated"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Default     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.DateCreated<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| DisplayName | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"DateCreated"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>        |
| Required    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Update      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Value18.Text<td style="background-color:#ffcccc; width:50%;"></td></tr></table>         |

### Design

| Property    | Value                                                                                                                                                        |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderStyle | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| DisplayMode | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| Height      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">80<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Visible     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| Width       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">401.05714634486605<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| WidthFit    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X           | 0                                                                                                                                                            |
| Y           | 4                                                                                                                                                            |
| ZIndex      | 6                                                                                                                                                            |

### Color Properties

| Property    | Value                                                                                                                                                                                                                                                                                                                                |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| Fill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Child Control  | StarVisible20  |
| Child Control  | Key20          |
| Child Control  | Value18        |
| Child Control  | ErrorMessage20 |
| Parent Control | NewTicketForm  |

## Description

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                                             |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                      |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                      |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table>                          |
| DelayOutput     | false                                                                                                                                                                             |
| HintText        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Thoroughly describe the problem here."<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Reset           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Button2.Pressed<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                         |

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">237.140323579729<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                    |
| Mode                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">TextMode.MultiLine<td style="background-color:#ffcccc; width:50%;">TextMode.SingleLine</td></tr></table> |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                    |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                     |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                                                        |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">554.5777160686325<td style="background-color:#ffcccc; width:50%;">320</td></tr></table>                  |
| X                      | 428.0996649535468                                                                                                                                                               |
| Y                      | 362.2594142259424                                                                                                                                                               |
| ZIndex                 | 12                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230,230,230,1)</td></tr><tr><td style="background-color:#E6E6E6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>       |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 1)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                              |
| Fill                | <table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | Description.BorderColor                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverBorderColor    | Description.BorderColor                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverColor          | Description.Color                                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverFill           | Description.Fill                                                                                                                                                                                                                                                                                                                                                                                                    |
| PressedBorderColor  | Description.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedColor        | Description.Color                                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedFill         | Description.Fill                                                                                                                                                                                                                                                                                                                                                                                                    |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Dropdown4

| Property                            | Value          |
| ----------------------------------- | -------------- |
| ![dropdown](resources/dropdown.png) | Type: dropdown |

### Data

| Property            | Value                                                                                                                                                                 |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                          |
| AllowEmptySelection | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                       |
| ContentLanguage     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                          |
| Items               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">PriorityTypes<td style="background-color:#ffcccc; width:50%;">DropDownSample</td></tr></table> |
| Reset               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Button2.Pressed<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |

### Design

| Property                  | Value                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle               | BorderStyle.Solid                                                                                                                                                                                                                                                                                                                                                                                                               |
| BorderThickness           | 2                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ChevronBackground         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table>                  |
| ChevronDisabledBackground | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 1)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table>             |
| ChevronDisabledFill       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ColorFade(RGBA(47, 41, 43, 1), 70%)<td style="background-color:#ffcccc; width:50%;">RGBA(244, 244, 244, 1)</td></tr></table>                                                                                                                                                                                                                             |
| ChevronFill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(225, 225, 225, 1)</td></tr><tr><td style="background-color:#E1E1E1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table>             |
| ChevronHoverBackground    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>ColorFade(RGBA(56, 96, 178, 1), -20%)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| ChevronHoverFill          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ColorFade(RGBA(255,255,255,1), -5%)<td style="background-color:#ffcccc; width:50%;">RGBA(255, 255, 255, 1)</td></tr></table>                                                                                                                                                                                                                             |
| DisplayMode               | DisplayMode.Edit                                                                                                                                                                                                                                                                                                                                                                                                                |
| FocusedBorderThickness    | 4                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Font                      | Font.'Open Sans'                                                                                                                                                                                                                                                                                                                                                                                                                |
| FontWeight                | FontWeight.Normal                                                                                                                                                                                                                                                                                                                                                                                                               |
| Height                    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">44<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                                                                                                                                                                                                                                                                  |
| Size                      | 13                                                                                                                                                                                                                                                                                                                                                                                                                              |
| TabIndex                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                                                                                                                                                                                                     |
| Width                     | 328                                                                                                                                                                                                                                                                                                                                                                                                                             |
| X                         | 40                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Y                         | 42.92307692307688                                                                                                                                                                                                                                                                                                                                                                                                               |
| ZIndex                    | 5                                                                                                                                                                                                                                                                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230,230,230,1)</td></tr><tr><td style="background-color:#E6E6E6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>       |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 1)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                              |
| Fill                | <table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | Dropdown4.BorderColor                                                                                                                                                                                                                                                                                                                                                                                               |
| HoverBorderColor    | ColorFade(Dropdown4.BorderColor, 15%)                                                                                                                                                                                                                                                                                                                                                                               |
| HoverColor          | Dropdown4.Color                                                                                                                                                                                                                                                                                                                                                                                                     |
| HoverFill           | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(225,225,225,1)</td></tr><tr><td style="background-color:#E1E1E1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(186, 202, 226, 1)</td></tr><tr><td style="background-color:#BACAE2"></td></tr></table></td></tr></table>    |
| PressedBorderColor  | Dropdown4.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table>    |
| PressedFill         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(137,51,102,1)</td></tr><tr><td style="background-color:#893366"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>        |
| SelectionColor      | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table>    |
| SelectionFill       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(137,51,102,1)</td></tr><tr><td style="background-color:#893366"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table>       |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard16 |

## Dropdown5

| Property                            | Value          |
| ----------------------------------- | -------------- |
| ![dropdown](resources/dropdown.png) | Type: dropdown |

### Data

| Property            | Value                                                                                                                                                                    |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| AccessibleLabel     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| AllowEmptySelection | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                          |
| ContentLanguage     | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| Items               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">AccountNameTypes<td style="background-color:#ffcccc; width:50%;">DropDownSample</td></tr></table> |
| Reset               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Button2.Pressed<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |

### Design

| Property                  | Value                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle               | BorderStyle.Solid                                                                                                                                                                                                                                                                                                                                                                                                               |
| BorderThickness           | 2                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ChevronBackground         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table>                  |
| ChevronDisabledBackground | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 1)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table>             |
| ChevronDisabledFill       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ColorFade(RGBA(47, 41, 43, 1), 70%)<td style="background-color:#ffcccc; width:50%;">RGBA(244, 244, 244, 1)</td></tr></table>                                                                                                                                                                                                                             |
| ChevronFill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(225, 225, 225, 1)</td></tr><tr><td style="background-color:#E1E1E1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table>             |
| ChevronHoverBackground    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101,128,187,1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>ColorFade(RGBA(56, 96, 178, 1), -20%)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| ChevronHoverFill          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ColorFade(RGBA(255,255,255,1), -5%)<td style="background-color:#ffcccc; width:50%;">RGBA(255, 255, 255, 1)</td></tr></table>                                                                                                                                                                                                                             |
| DisplayMode               | DisplayMode.Edit                                                                                                                                                                                                                                                                                                                                                                                                                |
| FocusedBorderThickness    | 4                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Font                      | Font.'Open Sans'                                                                                                                                                                                                                                                                                                                                                                                                                |
| FontWeight                | FontWeight.Normal                                                                                                                                                                                                                                                                                                                                                                                                               |
| Height                    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">44<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                                                                                                                                                                                                                                                                  |
| Size                      | 13                                                                                                                                                                                                                                                                                                                                                                                                                              |
| TabIndex                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                                                                                                                                                                                                     |
| Width                     | 328                                                                                                                                                                                                                                                                                                                                                                                                                             |
| X                         | 40.61538461538464                                                                                                                                                                                                                                                                                                                                                                                                               |
| Y                         | 31.15384615384615                                                                                                                                                                                                                                                                                                                                                                                                               |
| ZIndex                    | 5                                                                                                                                                                                                                                                                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230,230,230,1)</td></tr><tr><td style="background-color:#E6E6E6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>       |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 1)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                              |
| Fill                | <table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | Dropdown5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                               |
| HoverBorderColor    | ColorFade(Dropdown5.BorderColor, 15%)                                                                                                                                                                                                                                                                                                                                                                               |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(225,225,225,1)</td></tr><tr><td style="background-color:#E1E1E1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(186, 202, 226, 1)</td></tr><tr><td style="background-color:#BACAE2"></td></tr></table></td></tr></table>    |
| PressedBorderColor  | Dropdown5.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table>    |
| PressedFill         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(137,51,102,1)</td></tr><tr><td style="background-color:#893366"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>        |
| SelectionColor      | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table>    |
| SelectionFill       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(137,51,102,1)</td></tr><tr><td style="background-color:#893366"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table>       |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard17 |

## ErrorMessage15

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
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Lighter<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>   |
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
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">328<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                |
| X                      | 42                                                                                                                                                                              |
| Y                      | Value13.Y + Value13.Height                                                                                                                                                      |
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
| FocusedBorderColor  | ErrorMessage15.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | ErrorMessage15.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | ErrorMessage15.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | ErrorMessage15.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | ErrorMessage15.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | ErrorMessage15.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | ErrorMessage15.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard15 |

## ErrorMessage16

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
| Y                      | Dropdown4.Y + Dropdown4.Height                                                                                                                                                  |
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
| FocusedBorderColor  | ErrorMessage16.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | ErrorMessage16.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | ErrorMessage16.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | ErrorMessage16.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | ErrorMessage16.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | ErrorMessage16.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | ErrorMessage16.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard16 |

## ErrorMessage17

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
| Y                      | Dropdown5.Y + Dropdown5.Height                                                                                                                                                  |
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
| FocusedBorderColor  | ErrorMessage17.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | ErrorMessage17.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | ErrorMessage17.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | ErrorMessage17.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | ErrorMessage17.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | ErrorMessage17.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | ErrorMessage17.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard17 |

## ErrorMessage19

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
| Y                      | Value17.Y + Value17.Height                                                                                                                                                      |
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
| FocusedBorderColor  | ErrorMessage19.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | ErrorMessage19.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | ErrorMessage19.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | ErrorMessage19.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | ErrorMessage19.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | ErrorMessage19.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | ErrorMessage19.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard19 |

## ErrorMessage20

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
| Y                      | Value18.Y + Value18.Height                                                                                                                                                      |
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
| FocusedBorderColor  | ErrorMessage20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | ErrorMessage20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | ErrorMessage20.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | ErrorMessage20.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | ErrorMessage20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | ErrorMessage20.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | ErrorMessage20.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard20 |

## Group11\_1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![group](resources/group.png) | Type: group |

### Design

| Property | Value                                                                                                                                                         |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Height   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                |
| Width    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150.00000000000003<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| X        | 231.8926627959                                                                                                                                                |
| Y        | 47.5300931183284                                                                                                                                              |
| ZIndex   | 3                                                                                                                                                             |

### Color Properties

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Group12\_1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![group](resources/group.png) | Type: group |

### Design

| Property | Value                                                                                                                                          |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Height   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| Width    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| X        | 435.439215686274                                                                                                                               |
| Y        | 47.5300931183284                                                                                                                               |
| ZIndex   | 4                                                                                                                                              |

### Color Properties

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Group13\_1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![group](resources/group.png) | Type: group |

### Design

| Property | Value                                                                                                                                          |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Height   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| Width    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| X        | 638.890013169452                                                                                                                               |
| Y        | 47.5300931183284                                                                                                                               |
| ZIndex   | 5                                                                                                                                              |

### Color Properties

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Group14\_1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![group](resources/group.png) | Type: group |

### Design

| Property | Value                                                                                                                                          |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Height   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| Width    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| X        | 848.058018729887                                                                                                                               |
| Y        | 47.5300931183284                                                                                                                               |
| ZIndex   | 6                                                                                                                                              |

### Color Properties

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Group2\_1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![group](resources/group.png) | Type: group |

### Design

| Property | Value                                                                                                                                          |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Height   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| Width    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| X        | 27.4                                                                                                                                           |
| Y        | 47.5300931183284                                                                                                                               |
| ZIndex   | 2                                                                                                                                              |

### Color Properties

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Group7

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![group](resources/group.png) | Type: group |

### Design

| Property | Value                                                                                                                                         |
| -------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Height   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">58<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| Width    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| X        | 0                                                                                                                                             |
| Y        | 0                                                                                                                                             |
| ZIndex   | 1                                                                                                                                             |

### Color Properties

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## icon6

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Behavior

| Property | Value                                                                                                                                                                                                            |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(DashboardPage,ScreenTransition.Fade);ResetForm(NewTicketForm)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">27.5333333333333<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.ChevronLeft<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">28<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 16                                                                                                                                                          |
| Y                      | 15.23333333333335                                                                                                                                           |
| ZIndex                 | 21                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon6.Fill                                                                                                                                                                                                                                                                                                                                    |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon6.BorderColor                                                                                                                                                                                                                                                                                                                             |
| HoverBorderColor    | ColorFade(icon6.BorderColor, 20%)                                                                                                                                                                                                                                                                                                             |
| HoverColor          | ColorFade(icon6.Color, 20%)                                                                                                                                                                                                                                                                                                                   |
| HoverFill           | icon6.Fill                                                                                                                                                                                                                                                                                                                                    |
| PressedBorderColor  | ColorFade(icon6.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                           |
| PressedColor        | ColorFade(icon6.Color, \-20%)                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | icon6.Fill                                                                                                                                                                                                                                                                                                                                    |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Key15

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">52<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                 |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| PaddingBottom          | 5                                                                                                                                                                              |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">40<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| PaddingRight           | 5                                                                                                                                                                              |
| PaddingTop             | 5                                                                                                                                                                              |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">370.057146344866<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 0                                                                                                                                                                              |
| Y                      | 3.8461538461538462                                                                                                                                                             |
| ZIndex                 | 1                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(92,92,92,1)</td></tr><tr><td style="background-color:#5C5C5C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key15.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | Key15.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverColor          | Key15.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| HoverFill           | Key15.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | Key15.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | Key15.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| PressedFill         | Key15.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard15 |

## Key16

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">51<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                 |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| PaddingBottom          | 5                                                                                                                                                                              |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">40<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| PaddingRight           | 5                                                                                                                                                                              |
| PaddingTop             | 5                                                                                                                                                                              |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">370.057146344866<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                  |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 0                                                                                                                                                                              |
| Y                      | 1.153846153846154                                                                                                                                                              |
| ZIndex                 | 1                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(92,92,92,1)</td></tr><tr><td style="background-color:#5C5C5C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key16.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | Key16.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverColor          | Key16.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| HoverFill           | Key16.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | Key16.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | Key16.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| PressedFill         | Key16.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard16 |

## Key17

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">55<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | 5                                                                                                                                                                               |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">40<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                   |
| PaddingRight           | 5                                                                                                                                                                               |
| PaddingTop             | 5                                                                                                                                                                               |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">370.057146344866<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                   |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | 0                                                                                                                                                                               |
| ZIndex                 | 1                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(92,92,92,1)</td></tr><tr><td style="background-color:#5C5C5C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | Key17.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | Key17.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverColor          | Key17.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| HoverFill           | Key17.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | Key17.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | Key17.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| PressedFill         | Key17.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard17 |

## Key19

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
| FocusedBorderColor  | Key19.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | Key19.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverColor          | Key19.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| HoverFill           | Key19.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | Key19.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | Key19.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| PressedFill         | Key19.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard19 |

## Key20

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
| FocusedBorderColor  | Key20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | Key20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverColor          | Key20.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| HoverFill           | Key20.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | Key20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | Key20.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| PressedFill         | Key20.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard20 |

## NewTicketForm

| Property                    | Value      |
| --------------------------- | ---------- |
| ![form](resources/form.png) | Type: form |

### Behavior

| Property  | Value                                                                                                                                                                                                            |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSuccess | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(DashboardPage,ScreenTransition.Fade);ResetForm(NewTicketForm)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                       |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| DataSource      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Tickets<td style="background-color:#ffcccc; width:50%;"></td></tr></table>           |
| DefaultMode     | FormMode.Edit                                                                                                                                               |
| Item            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Defaults(Tickets)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                           |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AcceptsFocus           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| BorderStyle            | BorderStyle.Solid                                                                                                                                               |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                     |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">4<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                     |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">458.5402252068918<td style="background-color:#ffcccc; width:50%;">500</td></tr></table>  |
| NumberOfColumns        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                     |
| SnapToColumns          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">401.05714634486605<td style="background-color:#ffcccc; width:50%;">800</td></tr></table> |
| X                      | 0                                                                                                                                                               |
| Y                      | 219                                                                                                                                                             |
| ZIndex                 | 34                                                                                                                                                              |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(180, 180, 180, 1)</td></tr><tr><td style="background-color:#B4B4B4"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>    |
| FocusedBorderColor | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Child Control  | DataCard15          |
| Child Control  | DataCard16          |
| Child Control  | DataCard17          |
| Child Control  | DataCard19          |
| Child Control  | DataCard20          |
| Parent Control | CreatenewticketPage |

## Rectangle1\_6

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
| ZIndex                 | 9                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle1\_6.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_6.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle1\_6.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle1\_6.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Rectangle1\_7

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                            |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(DashboardPage,ScreenTransition.Fade);ResetForm(NewTicketForm)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">58<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 0                                                                                                                                                           |
| Y                      | 0                                                                                                                                                           |
| ZIndex                 | 20                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle1\_7.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_7.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle1\_7.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle1\_7.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Rectangle1\_8

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">147.7012987012987<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X                      | 0                                                                                                                                                           |
| Y                      | 60                                                                                                                                                          |
| ZIndex                 | 14                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle1\_8.Fill                                                                                                                                                                                                                                                                                                                          |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 242, 242, .5)</td></tr><tr><td style="background-color:#F2F2F2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_8.BorderColor                                                                                                                                                                                                                                                                                                                   |
| HoverFill          | Rectangle1\_8.Fill                                                                                                                                                                                                                                                                                                                          |
| PressedFill        | Rectangle1\_8.Fill                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Rectangle6\_15

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">100<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| X                      | 0                                                                                                                                                           |
| Y                      | 78.8235294117628                                                                                                                                            |
| ZIndex                 | 15                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle6\_15.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle6\_15.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle6\_15.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle6\_15.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Rectangle6\_16

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">100<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| X                      | 204.49266279590034                                                                                                                                          |
| Y                      | 78.8235294117628                                                                                                                                            |
| ZIndex                 | 16                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle6\_16.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle6\_16.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle6\_16.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle6\_16.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Rectangle6\_17

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">100<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| X                      | 409.1321118611379                                                                                                                                           |
| Y                      | 78.8235294117628                                                                                                                                            |
| ZIndex                 | 17                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle6\_17.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle6\_17.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle6\_17.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle6\_17.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Rectangle6\_18

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">100<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| X                      | 613.4636973799783                                                                                                                                           |
| Y                      | 78.8235294117628                                                                                                                                            |
| ZIndex                 | 18                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle6\_18.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle6\_18.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle6\_18.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle6\_18.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Rectangle6\_19

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">100<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| X                      | 817.8842105263159                                                                                                                                           |
| Y                      | 78.8235294117628                                                                                                                                            |
| ZIndex                 | 19                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle6\_19.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle6\_19.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle6\_19.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle6\_19.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Rectangle7\_23

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X                      | 0                                                                                                                                                           |
| Y                      | 207                                                                                                                                                         |
| ZIndex                 | 33                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_23.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_23.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_23.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_23.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## StarVisible15

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key15.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                        |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key15.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                  |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key15.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key15.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key15.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key15.Y                                                                                                                                                                         |
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
| FocusedBorderColor  | StarVisible15.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | StarVisible15.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | StarVisible15.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | StarVisible15.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | StarVisible15.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | StarVisible15.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | StarVisible15.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard15 |

## StarVisible16

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key16.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                        |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key16.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                  |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key16.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key16.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key16.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key16.Y                                                                                                                                                                         |
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
| FocusedBorderColor  | StarVisible16.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | StarVisible16.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | StarVisible16.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | StarVisible16.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | StarVisible16.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | StarVisible16.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | StarVisible16.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard16 |

## StarVisible17

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key17.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                        |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key17.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                  |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key17.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key17.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key17.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key17.Y                                                                                                                                                                         |
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
| FocusedBorderColor  | StarVisible17.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | StarVisible17.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | StarVisible17.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | StarVisible17.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | StarVisible17.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | StarVisible17.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | StarVisible17.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard17 |

## StarVisible19

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key19.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                        |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key19.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                  |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key19.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key19.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key19.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key19.Y                                                                                                                                                                         |
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
| FocusedBorderColor  | StarVisible19.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | StarVisible19.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | StarVisible19.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | StarVisible19.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | StarVisible19.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | StarVisible19.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | StarVisible19.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard19 |

## StarVisible20

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key20.Height<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                        |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key20.PaddingBottom<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                  |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key20.PaddingLeft<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                    |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key20.PaddingRight<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Key20.PaddingTop<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                     |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 0                                                                                                                                                                               |
| Y                      | Key20.Y                                                                                                                                                                         |
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
| FocusedBorderColor  | StarVisible20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverBorderColor    | StarVisible20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| HoverColor          | StarVisible20.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | StarVisible20.Fill                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedBorderColor  | StarVisible20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                  |
| PressedColor        | StarVisible20.Color                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | StarVisible20.Fill                                                                                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard20 |

## Subject

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                                        |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table>                     |
| DelayOutput     | false                                                                                                                                                                        |
| HintText        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Short Description of the Problem"<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| MaxLength       |                                                                                                                                                                              |
| Reset           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Button2.Pressed<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">44<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                 |
| Mode                   | TextMode.SingleLine                                                                                                                                            |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                   |
| Size                   | 13                                                                                                                                                             |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                                       |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">554.6268656716418<td style="background-color:#ffcccc; width:50%;">320</td></tr></table> |
| X                      | 428.0750901520428                                                                                                                                              |
| Y                      | 264.850355436258                                                                                                                                               |
| ZIndex                 | 11                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230,230,230,1)</td></tr><tr><td style="background-color:#E6E6E6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>       |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 1)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                              |
| Fill                | <table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | Subject.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverBorderColor    | Subject.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverColor          | Subject.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverFill           | Subject.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedBorderColor  | Subject.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                            |
| PressedColor        | Subject.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedFill         | Subject.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox1\_25

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                              |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                       |
| Live            | Live.Off                                                                                                                                                           |
| Role            | TextRole.Default                                                                                                                                                   |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">CountRows(Tickets)<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>    |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">32<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | 150                                                                                                                                                                            |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 27.400000000000005                                                                                                                                                             |
| Y                      | 47.5300931183284                                                                                                                                                               |
| ZIndex                 | 22                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0,0,0,1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>       |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1\_25.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox1\_25.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox1\_25.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox1\_25.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox1\_25.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox1\_25.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox1\_25.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox1\_26

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                                   |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                            |
| Live            | Live.Off                                                                                                                                                                                |
| Role            | TextRole.Default                                                                                                                                                                        |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">CountRows(Filter(Tickets,Status="New"))<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>    |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">32<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | 150                                                                                                                                                                            |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 231.89266279590035                                                                                                                                                             |
| Y                      | 47.5300931183284                                                                                                                                                               |
| ZIndex                 | 24                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56,86,153,1)</td></tr><tr><td style="background-color:#385699"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1\_26.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox1\_26.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox1\_26.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox1\_26.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox1\_26.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox1\_26.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox1\_26.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox1\_27

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                                           |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                    |
| Live            | Live.Off                                                                                                                                                                                        |
| Role            | TextRole.Default                                                                                                                                                                                |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">CountRows(Filter(Tickets,Status="In progress"))<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>    |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">32<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | 150                                                                                                                                                                            |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 435.43921568627445                                                                                                                                                             |
| Y                      | 47.5300931183284                                                                                                                                                               |
| ZIndex                 | 26                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(195,179,5,1)</td></tr><tr><td style="background-color:#C3B305"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1\_27.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox1\_27.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox1\_27.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox1\_27.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox1\_27.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox1\_27.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox1\_27.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox1\_28

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                                      |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                               |
| Live            | Live.Off                                                                                                                                                                                   |
| Role            | TextRole.Default                                                                                                                                                                           |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">CountRows(Filter(Tickets,Status="Closed"))<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>    |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">32<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | 150                                                                                                                                                                            |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 638.890013169452                                                                                                                                                               |
| Y                      | 47.5300931183284                                                                                                                                                               |
| ZIndex                 | 29                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(71,185,50,1)</td></tr><tr><td style="background-color:#47B932"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1\_28.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox1\_28.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox1\_28.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox1\_28.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox1\_28.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox1\_28.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox1\_28.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox1\_29

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                                       |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                |
| Live            | Live.Off                                                                                                                                                                                    |
| Role            | TextRole.Default                                                                                                                                                                            |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">CountRows(Filter(Tickets,Status="On hold"))<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>    |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">32<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | 150                                                                                                                                                                            |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 848.0580187298873                                                                                                                                                              |
| Y                      | 47.5300931183284                                                                                                                                                               |
| ZIndex                 | 30                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(227,48,12,1)</td></tr><tr><td style="background-color:#E3300C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1\_29.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox1\_29.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox1\_29.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox1\_29.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox1\_29.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox1\_29.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox1\_29.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox2

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                                                   |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                            |
| Live            | Live.Off                                                                                                                                                                                |
| Role            | TextRole.Default                                                                                                                                                                        |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Please fill out the required fields *"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table> |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                           |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                            |
| FocusedBorderThickness | 0                                                                                                                                                                           |
| Font                   | Font.'Open Sans'                                                                                                                                                            |
| FontWeight             | FontWeight.Normal                                                                                                                                                           |
| Height                 | 40                                                                                                                                                                          |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| Overflow               | Overflow.Hidden                                                                                                                                                             |
| Size                   | 13                                                                                                                                                                          |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                        |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">msg_visible<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                       |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                           |
| X                      | 0                                                                                                                                                                           |
| Y                      | 679.4285714285716                                                                                                                                                           |
| ZIndex                 | 32                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(237, 28, 36, 1)</td></tr><tr><td style="background-color:#ED1C24"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                           |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230, 229, 229, 1)</td></tr><tr><td style="background-color:#E6E5E5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| FocusedBorderColor  | TextBox2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | TextBox2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverColor          | TextBox2.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| HoverFill           | TextBox2.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | TextBox2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | TextBox2.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| PressedFill         | TextBox2.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox2\_25

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| Live            | Live.Off                                                                                                                                                      |
| Role            | TextRole.Default                                                                                                                                              |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"All tickets"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table> |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                           |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                            |
| FocusedBorderThickness | 0                                                                                                                                                                           |
| Font                   | Font.'Open Sans'                                                                                                                                                            |
| FontWeight             | FontWeight.Normal                                                                                                                                                           |
| Height                 | 40                                                                                                                                                                          |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| Overflow               | Overflow.Hidden                                                                                                                                                             |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                        |
| Width                  | 150                                                                                                                                                                         |
| X                      | 27.400000000000005                                                                                                                                                          |
| Y                      | 133.2017349093727                                                                                                                                                           |
| ZIndex                 | 23                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0,0,0,1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>       |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox2\_25.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox2\_25.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox2\_25.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox2\_25.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox2\_25.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox2\_25.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox2\_25.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox2\_26

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                                               |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                        |
| Live            | Live.Off                                                                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(TextBox1_21.Text="1","New ticket","New tickets")<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table> |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                           |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                            |
| FocusedBorderThickness | 0                                                                                                                                                                           |
| Font                   | Font.'Open Sans'                                                                                                                                                            |
| FontWeight             | FontWeight.Normal                                                                                                                                                           |
| Height                 | 40                                                                                                                                                                          |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| Overflow               | Overflow.Hidden                                                                                                                                                             |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                        |
| Width                  | 150                                                                                                                                                                         |
| X                      | 231.89266279590035                                                                                                                                                          |
| Y                      | 133.2017349093737                                                                                                                                                           |
| ZIndex                 | 25                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56,86,153,1)</td></tr><tr><td style="background-color:#385699"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox2\_26.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox2\_26.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox2\_26.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox2\_26.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox2\_26.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox2\_26.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox2\_26.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox2\_27

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| Live            | Live.Off                                                                                                                                                      |
| Role            | TextRole.Default                                                                                                                                              |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"In progress"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table> |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                           |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                            |
| FocusedBorderThickness | 0                                                                                                                                                                           |
| Font                   | Font.'Open Sans'                                                                                                                                                            |
| FontWeight             | FontWeight.Normal                                                                                                                                                           |
| Height                 | 40                                                                                                                                                                          |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| Overflow               | Overflow.Hidden                                                                                                                                                             |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                        |
| Width                  | 150                                                                                                                                                                         |
| X                      | 435.43921568627445                                                                                                                                                          |
| Y                      | 133.2017349093737                                                                                                                                                           |
| ZIndex                 | 27                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(195,179,5,1)</td></tr><tr><td style="background-color:#C3B305"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox2\_27.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox2\_27.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox2\_27.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox2\_27.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox2\_27.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox2\_27.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox2\_27.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox2\_28

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                    |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| Live            | Live.Off                                                                                                                                                 |
| Role            | TextRole.Default                                                                                                                                         |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Closed"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table> |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                           |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                            |
| FocusedBorderThickness | 0                                                                                                                                                                           |
| Font                   | Font.'Open Sans'                                                                                                                                                            |
| FontWeight             | FontWeight.Normal                                                                                                                                                           |
| Height                 | 40                                                                                                                                                                          |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| Overflow               | Overflow.Hidden                                                                                                                                                             |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                        |
| Width                  | 150                                                                                                                                                                         |
| X                      | 638.890013169452                                                                                                                                                            |
| Y                      | 133.2017349093737                                                                                                                                                           |
| ZIndex                 | 28                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(71,185,50,1)</td></tr><tr><td style="background-color:#47B932"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox2\_28.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox2\_28.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox2\_28.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox2\_28.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox2\_28.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox2\_28.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox2\_28.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox2\_29

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                     |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| Live            | Live.Off                                                                                                                                                  |
| Role            | TextRole.Default                                                                                                                                          |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"On hold"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table> |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                           |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                            |
| FocusedBorderThickness | 0                                                                                                                                                                           |
| Font                   | Font.'Open Sans'                                                                                                                                                            |
| FontWeight             | FontWeight.Normal                                                                                                                                                           |
| Height                 | 40                                                                                                                                                                          |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| Overflow               | Overflow.Hidden                                                                                                                                                             |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                        |
| Width                  | 150                                                                                                                                                                         |
| X                      | 848.0580187298873                                                                                                                                                           |
| Y                      | 133.2017349093737                                                                                                                                                           |
| ZIndex                 | 31                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(227,48,12,1)</td></tr><tr><td style="background-color:#E3300C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox2\_29.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox2\_29.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox2\_29.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox2\_29.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox2\_29.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox2\_29.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox2\_29.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox4\_3

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                               |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                        |
| Live            | Live.Off                                                                                                                                                            |
| Role            | TextRole.Default                                                                                                                                                    |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Create new ticket"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

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
| ZIndex                 | 10                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                           |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | TextBox4\_3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverBorderColor    | TextBox4\_3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverColor          | TextBox4\_3.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverFill           | TextBox4\_3.Fill                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | TextBox4\_3.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedColor        | TextBox4\_3.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedFill         | TextBox4\_3.Fill                                                                                                                                                                                                                                                                                                                                                                                              |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox5\_43

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                       |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Live            | Live.Off                                                                                                                                                    |
| Role            | TextRole.Default                                                                                                                                            |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Subject *"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">31.2332015810276<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                    |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">225<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                |
| X                      | 421.24588684266973                                                                                                                                                              |
| Y                      | 234.13993274733                                                                                                                                                                 |
| ZIndex                 | 8                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(92,92,92,1)</td></tr><tr><td style="background-color:#5C5C5C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_43.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_43.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_43.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_43.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_43.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_43.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_43.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## TextBox5\_44

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                           |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| Live            | Live.Off                                                                                                                                                        |
| Role            | TextRole.Default                                                                                                                                                |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Description *"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">31.2332015810276<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                    |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">225<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                |
| X                      | 420.5487677889628                                                                                                                                                               |
| Y                      | 330.402985074627                                                                                                                                                                |
| ZIndex                 | 7                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(92,92,92,1)</td></tr><tr><td style="background-color:#5C5C5C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_44.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_44.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_44.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_44.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_44.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_44.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_44.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Parent Control | CreatenewticketPage |

## Value13

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                                                                              |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                       |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                       |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(Len(Parent.Default) = 0, User().FullName, Parent.Default)<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                                                                              |
| MaxLength       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">100<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                      |
| Reset           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Button2.Pressed<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                          |

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">44<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>   |
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
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">328<td style="background-color:#ffcccc; width:50%;">320</td></tr></table> |
| X                      | 42.30769230769235                                                                                                                                |
| Y                      | 45.769230769230774                                                                                                                               |
| ZIndex                 | 2                                                                                                                                                |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | If(IsBlank(Parent.Error), Parent.BorderColor, Color.Red)                                                                                                                                                                                                                                                                                                                                                            |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 1)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                              |
| Fill                | <table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | Value13.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230,230,230,1)</td></tr><tr><td style="background-color:#E6E6E6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>       |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | ColorFade(RGBA(190, 202, 226, 0), 30%)                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | Value13.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                            |
| PressedColor        | Value13.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedFill         | Value13.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard15 |

## Value17

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                       |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"New"<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                       |

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
| Y                      | Key19.Height                                                                                                                                                   |
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
| FocusedBorderColor  | Value17.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101, 128, 187, 1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | ColorFade(RGBA(190, 202, 226, 1), 30%)                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | Value17.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                            |
| PressedColor        | Value17.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedFill         | Value17.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard19 |

## Value18

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                       |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Now()<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                       |

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
| Y                      | Key20.Height                                                                                                                                                   |
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
| FocusedBorderColor  | Value18.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(101, 128, 187, 1)</td></tr><tr><td style="background-color:#6580BB"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | ColorFade(RGBA(190, 202, 226, 1), 30%)                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | Value18.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                            |
| PressedColor        | Value18.Color                                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedFill         | Value18.Fill                                                                                                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value      |
| -------------- | ---------- |
| Parent Control | DataCard20 |
