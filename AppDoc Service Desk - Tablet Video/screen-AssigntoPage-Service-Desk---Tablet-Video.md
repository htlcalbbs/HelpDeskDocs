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

## AssigntoPage

| Property                        | Value        |
| ------------------------------- | ------------ |
| ![screen](resources/screen.png) | Type: screen |

### Behavior

| Property  | Value                                                                                                                                                                                                            |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnVisible | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">UpdateContext({search_reset:true});UpdateContext({search_reset:false})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Height              | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Max(App.Height, App.DesignHeight)<td style="background-color:#ffcccc; width:50%;">Max(App.Height, App.MinScreenHeight)</td></tr></table>                                                                                                                                                                                                |
| ImagePosition       | ImagePosition.Fit                                                                                                                                                                                                                                                                                                                                                                                              |
| LoadingSpinner      | LoadingSpinner.None                                                                                                                                                                                                                                                                                                                                                                                            |
| LoadingSpinnerColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 51, 102, 1)</td></tr><tr><td style="background-color:#003366"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table> |
| Orientation         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(AssigntoPage.Width < AssigntoPage.Height, Layout.Vertical, Layout.Horizontal)<td style="background-color:#ffcccc; width:50%;">If(Self.Width < Self.Height, Layout.Vertical, Layout.Horizontal)</td></tr></table>                                                                                                                     |
| Size                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1 + CountRows(App.SizeBreakpoints) - CountIf(App.SizeBreakpoints, Value >= AssigntoPage.Width)<td style="background-color:#ffcccc; width:50%;">1 + CountRows(App.SizeBreakpoints) - CountIf(App.SizeBreakpoints, Value >= Self.Width)</td></tr></table>                                                                                 |
| Width               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Max(App.Width, App.DesignWidth)<td style="background-color:#ffcccc; width:50%;">Max(App.Width, App.MinScreenWidth)</td></tr></table>                                                                                                                                                                                                    |

### Color Properties

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fill     | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>White</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property      | Value           |
| ------------- | --------------- |
| Child Control | Rectangle3\_2   |
| Child Control | Rectangle1\_4   |
| Child Control | TextBox4\_2     |
| Child Control | Rectangle1\_5   |
| Child Control | icon5           |
| Child Control | Rectangle4\_3   |
| Child Control | TextInput2\_2   |
| Child Control | icon7\_2        |
| Child Control | AssignToGallery |
| Child Control | Group5          |

## AssignToGallery

| Property                          | Value         |
| --------------------------------- | ------------- |
| ![gallery](resources/gallery.png) | Type: gallery |

### Data

| Property        | Value                                                                                                                                                                                                                                                     |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                              |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                              |
| Items           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(IsBlank(TextInput2_2.Text), Attendants, Filter( Attendants, TextInput2_2.Text in Name ) )<td style="background-color:#ffcccc; width:50%;">CustomGallerySample</td></tr></table> |
| Reset           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                           |
| Selectable      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                            |

### Design

| Property               | Value                                                                                                                                                                                 |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                       |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                                     |
| DelayItemLoading       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                       |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                      |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">4<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                           |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">662<td style="background-color:#ffcccc; width:50%;">575</td></tr></table>                                      |
| Layout                 | Layout.Vertical                                                                                                                                                                       |
| LoadingSpinner         | LoadingSpinner.None                                                                                                                                                                   |
| LoadingSpinnerColor    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">AssignToGallery.BorderColor<td style="background-color:#ffcccc; width:50%;">Self.BorderColor</td></tr></table> |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                          |
| TemplateMaximumWidth   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                           |
| TemplatePadding        | 0                                                                                                                                                                                     |
| TemplateSize           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">45.78236914600549<td style="background-color:#ffcccc; width:50%;">Min(160, Self.Height - 60)</td></tr></table> |
| Transition             | Transition.None                                                                                                                                                                       |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;">640</td></tr></table>                                     |
| X                      | 0                                                                                                                                                                                     |
| Y                      | 106                                                                                                                                                                                   |
| ZIndex                 | 5                                                                                                                                                                                     |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>     |
| DisabledBorderColor | AssignToGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                    |
| DisabledFill        | AssignToGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                           |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| FocusedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                               |
| HoverBorderColor    | AssignToGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                    |
| HoverFill           | AssignToGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                           |
| PressedBorderColor  | AssignToGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                    |
| PressedFill         | AssignToGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                           |

### Child & Parent Controls

| Property       | Value            |
| -------------- | ---------------- |
| Child Control  | galleryTemplate3 |
| Child Control  | Rectangle5       |
| Child Control  | TextBox8         |
| Child Control  | icon1            |
| Child Control  | Rectangle7\_9    |
| Child Control  | Group15          |
| Parent Control | AssigntoPage     |

## galleryTemplate3

| Property                                          | Value                 |
| ------------------------------------------------- | --------------------- |
| ![galleryTemplate](resources/galleryTemplate.png) | Type: galleryTemplate |

### Behavior

| Property | Value                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property            | Value                                                                                                                                        |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| ItemAccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property     | Value                                                                                                                                                                                                                                                                                                                                |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| TemplateFill | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |

### Color Properties

### Child & Parent Controls

| Property       | Value           |
| -------------- | --------------- |
| Parent Control | AssignToGallery |

## Group15

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![group](resources/group.png) | Type: group |

### Design

| Property | Value                                                                                                                                                       |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Height   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">45.7823691460055<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| Width    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>             |
| X        | 0                                                                                                                                                           |
| Y        | 0                                                                                                                                                           |
| ZIndex   | 3                                                                                                                                                           |

### Color Properties

### Child & Parent Controls

| Property       | Value           |
| -------------- | --------------- |
| Parent Control | AssignToGallery |

## Group5

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
| ZIndex   | 21                                                                                                                                            |

### Color Properties

### Child & Parent Controls

| Property       | Value        |
| -------------- | ------------ |
| Parent Control | AssigntoPage |

## icon1

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                         |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">26<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.Check<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                          |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(ThisItem.Name=assign,true,false)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">26<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| X                      | 980                                                                                                                                                                           |
| Y                      | 10                                                                                                                                                                            |
| ZIndex                 | 2                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(115,115,115,1)</td></tr><tr><td style="background-color:#737373"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon1.Fill                                                                                                                                                                                                                                                                                                                                    |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon1.BorderColor                                                                                                                                                                                                                                                                                                                             |
| HoverBorderColor    | ColorFade(icon1.BorderColor, 20%)                                                                                                                                                                                                                                                                                                             |
| HoverColor          | ColorFade(icon1.Color, 20%)                                                                                                                                                                                                                                                                                                                   |
| HoverFill           | icon1.Fill                                                                                                                                                                                                                                                                                                                                    |
| PressedBorderColor  | ColorFade(icon1.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                           |
| PressedColor        | ColorFade(icon1.Color, \-20%)                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | icon1.Fill                                                                                                                                                                                                                                                                                                                                    |

### Child & Parent Controls

| Property       | Value           |
| -------------- | --------------- |
| Parent Control | AssignToGallery |

## icon5

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Behavior

| Property | Value                                                                                                                                            |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Back()<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.Cancel<td style="background-color:#ffcccc; width:50%;"></td></tr></table>       |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 15                                                                                                                                                          |
| Y                      | 15                                                                                                                                                          |
| ZIndex                 | 23                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon5.Fill                                                                                                                                                                                                                                                                                                                                    |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon5.BorderColor                                                                                                                                                                                                                                                                                                                             |
| HoverBorderColor    | ColorFade(icon5.BorderColor, 20%)                                                                                                                                                                                                                                                                                                             |
| HoverColor          | ColorFade(icon5.Color, 20%)                                                                                                                                                                                                                                                                                                                   |
| HoverFill           | icon5.Fill                                                                                                                                                                                                                                                                                                                                    |
| PressedBorderColor  | ColorFade(icon5.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                           |
| PressedColor        | ColorFade(icon5.Color, \-20%)                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | icon5.Fill                                                                                                                                                                                                                                                                                                                                    |

### Child & Parent Controls

| Property       | Value        |
| -------------- | ------------ |
| Parent Control | AssigntoPage |

## icon7\_2

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">21<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.Search<td style="background-color:#ffcccc; width:50%;"></td></tr></table>       |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 17.528112127211805                                                                                                                                          |
| Y                      | 72.51546391752578                                                                                                                                           |
| ZIndex                 | 20                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(115,115,115,1)</td></tr><tr><td style="background-color:#737373"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon7\_2.Fill                                                                                                                                                                                                                                                                                                                                 |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon7\_2.BorderColor                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | ColorFade(icon7\_2.BorderColor, 20%)                                                                                                                                                                                                                                                                                                          |
| HoverColor          | ColorFade(icon7\_2.Color, 20%)                                                                                                                                                                                                                                                                                                                |
| HoverFill           | icon7\_2.Fill                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | ColorFade(icon7\_2.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                        |
| PressedColor        | ColorFade(icon7\_2.Color, \-20%)                                                                                                                                                                                                                                                                                                              |
| PressedFill         | icon7\_2.Fill                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value        |
| -------------- | ------------ |
| Parent Control | AssigntoPage |

## Rectangle1\_4

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
| ZIndex                 | 3                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle1\_4.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_4.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle1\_4.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle1\_4.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value        |
| -------------- | ------------ |
| Parent Control | AssigntoPage |

## Rectangle1\_5

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                            |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Back()<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

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
| ZIndex                 | 22                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle1\_5.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_5.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle1\_5.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle1\_5.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value        |
| -------------- | ------------ |
| Parent Control | AssigntoPage |

## Rectangle3\_2

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">768<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| X                      | 0                                                                                                                                                           |
| Y                      | 0                                                                                                                                                           |
| ZIndex                 | 2                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle3\_2.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle3\_2.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle3\_2.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle3\_2.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value        |
| -------------- | ------------ |
| Parent Control | AssigntoPage |

## Rectangle4\_3

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">46<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1023<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X                      | 1                                                                                                                                                           |
| Y                      | 60                                                                                                                                                          |
| ZIndex                 | 18                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                   |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>  |
| DisabledFill       | Rectangle4\_3.Fill                                                                                                                                                                                                                                                                                                                      |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(244,242,242,1)</td></tr><tr><td style="background-color:#F4F2F2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle4\_3.BorderColor                                                                                                                                                                                                                                                                                                               |
| HoverFill          | Rectangle4\_3.Fill                                                                                                                                                                                                                                                                                                                      |
| PressedFill        | Rectangle4\_3.Fill                                                                                                                                                                                                                                                                                                                      |

### Child & Parent Controls

| Property       | Value        |
| -------------- | ------------ |
| Parent Control | AssigntoPage |

## Rectangle5

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                              |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(TicketdetailsPage,ScreenTransition.Fade,{assign:AssignToGallery.Selected.Name})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">45.7823691460055<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X                      | 0                                                                                                                                                           |
| Y                      | 0                                                                                                                                                           |
| ZIndex                 | 4                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle5.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(62,96,170,0)</td></tr><tr><td style="background-color:#3E60AA"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>  |
| FocusedBorderColor | Rectangle5.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle5.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle5.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value           |
| -------------- | --------------- |
| Parent Control | AssignToGallery |

## Rectangle7\_9

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
| Y                      | 44.7823691460055                                                                                                                                            |
| ZIndex                 | 1                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_9.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_9.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle7\_9.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle7\_9.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value           |
| -------------- | --------------- |
| Parent Control | AssignToGallery |

## TextBox4\_2

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                       |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| Live            | Live.Off                                                                                                                                                    |
| Role            | TextRole.Default                                                                                                                                            |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Assign to"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

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
| ZIndex                 | 4                                                                                                                                                                           |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                           |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | TextBox4\_2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverBorderColor    | TextBox4\_2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverColor          | TextBox4\_2.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverFill           | TextBox4\_2.Fill                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | TextBox4\_2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedColor        | TextBox4\_2.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedFill         | TextBox4\_2.Fill                                                                                                                                                                                                                                                                                                                                                                                              |

### Child & Parent Controls

| Property       | Value        |
| -------------- | ------------ |
| Parent Control | AssigntoPage |

## TextBox8

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                              |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(TicketdetailsPage,ScreenTransition.Fade,{assign:AssignToGallery.Selected.Name})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| Live            | Live.Off                                                                                                                                                      |
| Role            | TextRole.Default                                                                                                                                              |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.Name<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                          |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                              |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                               |
| FocusedBorderThickness | 0                                                                                                                                                                              |
| Font                   | Font.'Open Sans'                                                                                                                                                               |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table> |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">45.7823691460055<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                   |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Overflow               | Overflow.Hidden                                                                                                                                                                |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">942<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                               |
| X                      | 0                                                                                                                                                                              |
| Y                      | 0                                                                                                                                                                              |
| ZIndex                 | 5                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverBorderColor    | TextBox8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverColor          | TextBox8.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverFill           | TextBox8.Fill                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | TextBox8.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedColor        | TextBox8.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedFill         | TextBox8.Fill                                                                                                                                                                                                                                                                                                                                                                                              |

### Child & Parent Controls

| Property       | Value           |
| -------------- | --------------- |
| Parent Control | AssignToGallery |

## TextInput2\_2

| Property                    | Value      |
| --------------------------- | ---------- |
| ![text](resources/text.png) | Type: text |

### Data

| Property        | Value                                                                                                                                                    |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>             |
| Default         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;">"Text input"</td></tr></table> |
| DelayOutput     | false                                                                                                                                                    |
| HintText        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Search"<td style="background-color:#ffcccc; width:50%;"></td></tr></table>       |
| Reset           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">search_reset<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |

### Design

| Property               | Value                                                                                                                                                          |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                              |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;">2</td></tr></table>                   |
| DisplayMode            | DisplayMode.Edit                                                                                                                                               |
| EnableSpellCheck       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">3<td style="background-color:#ffcccc; width:50%;">4</td></tr></table>                   |
| Font                   | Font.'Open Sans'                                                                                                                                               |
| FontWeight             | FontWeight.Normal                                                                                                                                              |
| Format                 | TextFormat.Text                                                                                                                                                |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">29<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                 |
| Mode                   | TextMode.SingleLine                                                                                                                                            |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                    |
| VirtualKeyboardMode    | VirtualKeyboardMode.Auto                                                                                                                                       |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">998.3016569790402<td style="background-color:#ffcccc; width:50%;">320</td></tr></table> |
| X                      | 13.69834302095977                                                                                                                                              |
| Y                      | 68                                                                                                                                                             |
| ZIndex                 | 19                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(159, 167, 165, 1)</td></tr><tr><td style="background-color:#9FA7A5"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(166, 166, 166, 1)</td></tr><tr><td style="background-color:#A6A6A6"></td></tr></table></td></tr></table> |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                              |
| Fill                | <table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | TextInput2\_2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverBorderColor    | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230,230,230,1)</td></tr><tr><td style="background-color:#E6E6E6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>       |
| HoverColor          | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 41, 43, 1)</td></tr><tr><td style="background-color:#2F292B"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| HoverFill           | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(186, 202, 226, 1)</td></tr><tr><td style="background-color:#BACAE2"></td></tr></table></td></tr></table>    |
| PressedBorderColor  | TextInput2\_2.HoverBorderColor                                                                                                                                                                                                                                                                                                                                                                                      |
| PressedColor        | TextInput2\_2.Color                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | TextInput2\_2.Fill                                                                                                                                                                                                                                                                                                                                                                                                  |

### Child & Parent Controls

| Property       | Value        |
| -------------- | ------------ |
| Parent Control | AssigntoPage |
