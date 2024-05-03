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

## AreaPage

| Property                        | Value        |
| ------------------------------- | ------------ |
| ![screen](resources/screen.png) | Type: screen |

### Design

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Height              | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Max(App.Height, App.DesignHeight)<td style="background-color:#ffcccc; width:50%;">Max(App.Height, App.MinScreenHeight)</td></tr></table>                                                                                                                                                                                                |
| ImagePosition       | ImagePosition.Fit                                                                                                                                                                                                                                                                                                                                                                                              |
| LoadingSpinner      | LoadingSpinner.None                                                                                                                                                                                                                                                                                                                                                                                            |
| LoadingSpinnerColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 51, 102, 1)</td></tr><tr><td style="background-color:#003366"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table> |
| Orientation         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(AreaPage.Width < AreaPage.Height, Layout.Vertical, Layout.Horizontal)<td style="background-color:#ffcccc; width:50%;">If(Self.Width < Self.Height, Layout.Vertical, Layout.Horizontal)</td></tr></table>                                                                                                                             |
| Size                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1 + CountRows(App.SizeBreakpoints) - CountIf(App.SizeBreakpoints, Value >= AreaPage.Width)<td style="background-color:#ffcccc; width:50%;">1 + CountRows(App.SizeBreakpoints) - CountIf(App.SizeBreakpoints, Value >= Self.Width)</td></tr></table>                                                                                     |
| Width               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Max(App.Width, App.DesignWidth)<td style="background-color:#ffcccc; width:50%;">Max(App.Width, App.MinScreenWidth)</td></tr></table>                                                                                                                                                                                                    |

### Color Properties

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                           |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fill     | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>White</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property      | Value          |
| ------------- | -------------- |
| Child Control | Rectangle1\_11 |
| Child Control | TextBox4\_6    |
| Child Control | Rectangle1\_13 |
| Child Control | icon5\_2       |
| Child Control | AreaGallery    |
| Child Control | Group6\_1      |

## AreaGallery

| Property                          | Value         |
| --------------------------------- | ------------- |
| ![gallery](resources/gallery.png) | Type: gallery |

### Data

| Property        | Value                                                                                                                                                                         |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| Items           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">AccountNameTypes<td style="background-color:#ffcccc; width:50%;">CustomGallerySample</td></tr></table> |
| Reset           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                               |
| Selectable      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |

### Design

| Property               | Value                                                                                                                                                                                 |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                       |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                                     |
| DelayItemLoading       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                       |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                      |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">4<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                           |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">708<td style="background-color:#ffcccc; width:50%;">575</td></tr></table>                                      |
| Layout                 | Layout.Vertical                                                                                                                                                                       |
| LoadingSpinner         | LoadingSpinner.None                                                                                                                                                                   |
| LoadingSpinnerColor    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">AreaGallery.BorderColor<td style="background-color:#ffcccc; width:50%;">Self.BorderColor</td></tr></table>     |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                          |
| TemplateMaximumWidth   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                           |
| TemplatePadding        | 0                                                                                                                                                                                     |
| TemplateSize           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">45.78236914600549<td style="background-color:#ffcccc; width:50%;">Min(160, Self.Height - 60)</td></tr></table> |
| Transition             | Transition.None                                                                                                                                                                       |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;">640</td></tr></table>                                     |
| X                      | 0                                                                                                                                                                                     |
| Y                      | 60                                                                                                                                                                                    |
| ZIndex                 | 4                                                                                                                                                                                     |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>     |
| DisabledBorderColor | AreaGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | AreaGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                               |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 244, 249, .5)</td></tr><tr><td style="background-color:#F2F4F9"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| FocusedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                               |
| HoverBorderColor    | AreaGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                        |
| HoverFill           | AreaGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                               |
| PressedBorderColor  | AreaGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedFill         | AreaGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                               |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Child Control  | galleryTemplate3\_2 |
| Child Control  | Rectangle7\_1       |
| Child Control  | TextBox8\_2         |
| Child Control  | icon1\_2            |
| Child Control  | Rectangle7\_12      |
| Child Control  | Group16\_1          |
| Parent Control | AreaPage            |

## galleryTemplate3\_2

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

| Property       | Value       |
| -------------- | ----------- |
| Parent Control | AreaGallery |

## Group16\_1

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

| Property       | Value       |
| -------------- | ----------- |
| Parent Control | AreaGallery |

## Group6\_1

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
| ZIndex   | 20                                                                                                                                            |

### Color Properties

### Child & Parent Controls

| Property       | Value    |
| -------------- | -------- |
| Parent Control | AreaPage |

## icon1\_2

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

| Property               | Value                                                                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                  |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                     |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                     |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                      |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                     |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">26<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                    |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.Check<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                            |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                     |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                     |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                     |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                     |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                     |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                     |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(ThisItem.AccountNameTypes='Microsoft.MeasureInMR.MeasurementType'.Area,true,false)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">26<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                    |
| X                      | 975.7974683544235                                                                                                                                                                                                               |
| Y                      | 9.89118457300275                                                                                                                                                                                                                |
| ZIndex                 | 2                                                                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(115,115,115,1)</td></tr><tr><td style="background-color:#737373"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon1\_2.Fill                                                                                                                                                                                                                                                                                                                                 |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon1\_2.BorderColor                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | ColorFade(icon1\_2.BorderColor, 20%)                                                                                                                                                                                                                                                                                                          |
| HoverColor          | ColorFade(icon1\_2.Color, 20%)                                                                                                                                                                                                                                                                                                                |
| HoverFill           | icon1\_2.Fill                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | ColorFade(icon1\_2.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                        |
| PressedColor        | ColorFade(icon1\_2.Color, \-20%)                                                                                                                                                                                                                                                                                                              |
| PressedFill         | icon1\_2.Fill                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value       |
| -------------- | ----------- |
| Parent Control | AreaGallery |

## icon5\_2

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
| ZIndex                 | 22                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon5\_2.Fill                                                                                                                                                                                                                                                                                                                                 |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon5\_2.BorderColor                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | ColorFade(icon5\_2.BorderColor, 20%)                                                                                                                                                                                                                                                                                                          |
| HoverColor          | ColorFade(icon5\_2.Color, 20%)                                                                                                                                                                                                                                                                                                                |
| HoverFill           | icon5\_2.Fill                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | ColorFade(icon5\_2.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                        |
| PressedColor        | ColorFade(icon5\_2.Color, \-20%)                                                                                                                                                                                                                                                                                                              |
| PressedFill         | icon5\_2.Fill                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value    |
| -------------- | -------- |
| Parent Control | AreaPage |

## Rectangle1\_11

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
| ZIndex                 | 2                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle1\_11.Fill                                                                                                                                                                                                                                                                                                                    |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_11.BorderColor                                                                                                                                                                                                                                                                                                             |
| HoverFill          | Rectangle1\_11.Fill                                                                                                                                                                                                                                                                                                                    |
| PressedFill        | Rectangle1\_11.Fill                                                                                                                                                                                                                                                                                                                    |

### Child & Parent Controls

| Property       | Value    |
| -------------- | -------- |
| Parent Control | AreaPage |

## Rectangle1\_13

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
| ZIndex                 | 21                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle1\_13.Fill                                                                                                                                                                                                                                                                                                                    |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_13.BorderColor                                                                                                                                                                                                                                                                                                             |
| HoverFill          | Rectangle1\_13.Fill                                                                                                                                                                                                                                                                                                                    |
| PressedFill        | Rectangle1\_13.Fill                                                                                                                                                                                                                                                                                                                    |

### Child & Parent Controls

| Property       | Value    |
| -------------- | -------- |
| Parent Control | AreaPage |

## Rectangle7\_1

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                                    |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(TicketdetailsPage,ScreenTransition.Fade,{Area:AreaGallery.Selected.AccountNameTypes})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

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
| DisabledFill       | Rectangle7\_1.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(62,96,170,0)</td></tr><tr><td style="background-color:#3E60AA"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>  |
| FocusedBorderColor | Rectangle7\_1.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle7\_1.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle7\_1.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value       |
| -------------- | ----------- |
| Parent Control | AreaGallery |

## Rectangle7\_12

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
| DisabledFill       | Rectangle7\_12.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_12.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_12.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_12.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value       |
| -------------- | ----------- |
| Parent Control | AreaGallery |

## TextBox4\_6

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
| ZIndex                 | 3                                                                                                                                                                           |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                           |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | TextBox4\_6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverBorderColor    | TextBox4\_6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverColor          | TextBox4\_6.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverFill           | TextBox4\_6.Fill                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | TextBox4\_6.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedColor        | TextBox4\_6.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedFill         | TextBox4\_6.Fill                                                                                                                                                                                                                                                                                                                                                                                              |

### Child & Parent Controls

| Property       | Value    |
| -------------- | -------- |
| Parent Control | AreaPage |

## TextBox8\_2

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                                    |
| -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(TicketdetailsPage,ScreenTransition.Fade,{Area:AreaGallery.Selected.AccountNameTypes})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                     |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                              |
| Live            | Live.Off                                                                                                                                                                  |
| Role            | TextRole.Default                                                                                                                                                          |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.AccountNameTypes<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

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
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">15<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                                  |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                                           |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">759.8736696740102<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                 |
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
| FocusedBorderColor  | TextBox8\_2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                    |
| HoverBorderColor    | TextBox8\_2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                    |
| HoverColor          | TextBox8\_2.Color                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverFill           | TextBox8\_2.Fill                                                                                                                                                                                                                                                                                                                                                                                           |
| PressedBorderColor  | TextBox8\_2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                    |
| PressedColor        | TextBox8\_2.Color                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedFill         | TextBox8\_2.Fill                                                                                                                                                                                                                                                                                                                                                                                           |

### Child & Parent Controls

| Property       | Value       |
| -------------- | ----------- |
| Parent Control | AreaGallery |
