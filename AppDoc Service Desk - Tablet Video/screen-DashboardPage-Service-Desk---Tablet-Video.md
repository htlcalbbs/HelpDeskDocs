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

## DashboardPage

| Property                        | Value        |
| ------------------------------- | ------------ |
| ![screen](resources/screen.png) | Type: screen |

### Behavior

| Property  | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| --------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnVisible | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(FilterGallery.Selected.TicketTypes="All tickets", UpdateContext({type:"All"}), FilterGallery.Selected.TicketTypes="New tickets", UpdateContext({type:"New"}), FilterGallery.Selected.TicketTypes="Tickets in progress", UpdateContext({type:"In progress"}), FilterGallery.Selected.TicketTypes="Tickets closed", UpdateContext({type:"Closed"}), FilterGallery.Selected.TicketTypes="Tickets on hold", UpdateContext({type:"On hold"}), FilterGallery.Selected.TicketTypes="Tickets older than 3 days", UpdateContext({datetype:Text(DateAdd(DateValue(Text(Today()), "en"), -3)),type:"Tickets older than 3 days"}), FilterGallery.Selected.TicketTypes="Tickets closed today", UpdateContext({datetype:Text(DateAdd(DateValue(Text(Today()), "en"), 0)),type:"Tickets closed today"}), FilterGallery.Selected.TicketTypes="Tickets opened today", UpdateContext({datetype:Text(DateAdd(DateValue(Text(Today()), "en"), 0)),type:"Tickets opened today"}))<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Height              | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Max(App.Height, App.DesignHeight)<td style="background-color:#ffcccc; width:50%;">Max(App.Height, App.MinScreenHeight)</td></tr></table>                                                                                                                                                                                                |
| ImagePosition       | ImagePosition.Fit                                                                                                                                                                                                                                                                                                                                                                                              |
| LoadingSpinner      | LoadingSpinner.None                                                                                                                                                                                                                                                                                                                                                                                            |
| LoadingSpinnerColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 51, 102, 1)</td></tr><tr><td style="background-color:#003366"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table> |
| Orientation         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(DashboardPage.Width < DashboardPage.Height, Layout.Vertical, Layout.Horizontal)<td style="background-color:#ffcccc; width:50%;">If(Self.Width < Self.Height, Layout.Vertical, Layout.Horizontal)</td></tr></table>                                                                                                                   |
| Size                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1 + CountRows(App.SizeBreakpoints) - CountIf(App.SizeBreakpoints, Value >= DashboardPage.Width)<td style="background-color:#ffcccc; width:50%;">1 + CountRows(App.SizeBreakpoints) - CountIf(App.SizeBreakpoints, Value >= Self.Width)</td></tr></table>                                                                                |
| Width               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Max(App.Width, App.DesignWidth)<td style="background-color:#ffcccc; width:50%;">Max(App.Width, App.MinScreenWidth)</td></tr></table>                                                                                                                                                                                                    |

### Color Properties

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                              |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Fill     | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>White</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |

### Child & Parent Controls

| Property      | Value          |
| ------------- | -------------- |
| Child Control | Rectangle1\_12 |
| Child Control | TextBox4\_5    |
| Child Control | Button2        |
| Child Control | TextBox5       |
| Child Control | icon3\_2       |
| Child Control | Timer1         |
| Child Control | TextBox1\_20   |
| Child Control | TextBox1\_21   |
| Child Control | TextBox1\_22   |
| Child Control | TextBox1\_23   |
| Child Control | TextBox1\_24   |
| Child Control | Rectangle1\_2  |
| Child Control | Rectangle6\_10 |
| Child Control | Rectangle6\_11 |
| Child Control | Rectangle6\_12 |
| Child Control | Rectangle6\_13 |
| Child Control | Rectangle6\_14 |
| Child Control | TextBox2\_20   |
| Child Control | TextBox2\_21   |
| Child Control | TextBox2\_22   |
| Child Control | TextBox2\_23   |
| Child Control | TextBox2\_24   |
| Child Control | Rectangle7\_19 |
| Child Control | Rectangle7\_15 |
| Child Control | Rectangle3\_4  |
| Child Control | TicketsGallery |
| Child Control | FilterGallery  |
| Child Control | Rectangle7\_17 |
| Child Control | Rectangle7\_18 |
| Child Control | Rectangle7\_20 |
| Child Control | Rectangle7\_21 |
| Child Control | Group2         |
| Child Control | Group11        |
| Child Control | Group12        |
| Child Control | Group13        |
| Child Control | Group14        |

## Button2

| Property                        | Value        |
| ------------------------------- | ------------ |
| ![button](resources/button.png) | Type: button |

### Behavior

| Property | Value                                                                                                                                                                                                                 |
| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(CreatenewticketPage,ScreenTransition.Fade); NewForm(NewTicketForm)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>         |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;">"Button"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                           |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Center                                                                                                                                    |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| BorderStyle            | BorderStyle.Solid                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                |
| FocusedBorderThickness | 4                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                |
| FontWeight             | FontWeight.Semibold                                                                                                                             |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>  |
| Size                   | 15                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>     |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                            |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60<td style="background-color:#ffcccc; width:50%;">160</td></tr></table> |
| X                      | 964                                                                                                                                             |
| Y                      | 0                                                                                                                                               |
| ZIndex                 | 37                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | ColorFade(Button2.Fill, \-15%)                                                                                                                                                                                                                                                                                                                                                                                   |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table> |
| DisabledBorderColor | ColorFade(Button2.BorderColor, 70%)                                                                                                                                                                                                                                                                                                                                                                              |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                              |
| DisabledFill        | ColorFade(RGBA(159, 167, 165, 1), 50%)                                                                                                                                                                                                                                                                                                                                                                           |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table>      |
| FocusedBorderColor  | Button2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                              |
| HoverBorderColor    | Button2.BorderColor                                                                                                                                                                                                                                                                                                                                                                                              |
| HoverColor          | Button2.Color                                                                                                                                                                                                                                                                                                                                                                                                    |
| HoverFill           | Button2.Fill                                                                                                                                                                                                                                                                                                                                                                                                     |
| PressedBorderColor  | Button2.Fill                                                                                                                                                                                                                                                                                                                                                                                                     |
| PressedColor        | Button2.Color                                                                                                                                                                                                                                                                                                                                                                                                    |
| PressedFill         | Button2.Fill                                                                                                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## FilterGallery

| Property                          | Value         |
| --------------------------------- | ------------- |
| ![gallery](resources/gallery.png) | Type: gallery |

### Data

| Property        | Value                                                                                                                                                                    |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                             |
| Items           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">TicketTypes<td style="background-color:#ffcccc; width:50%;">CustomGallerySample</td></tr></table> |
| Reset           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                          |
| Selectable      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                           |

### Design

| Property               | Value                                                                                                                                                                                 |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                       |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                                     |
| DelayItemLoading       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                       |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                      |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">4<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                           |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">559.874635568513<td style="background-color:#ffcccc; width:50%;">575</td></tr></table>                         |
| Layout                 | Layout.Vertical                                                                                                                                                                       |
| LoadingSpinner         | LoadingSpinner.None                                                                                                                                                                   |
| LoadingSpinnerColor    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FilterGallery.BorderColor<td style="background-color:#ffcccc; width:50%;">Self.BorderColor</td></tr></table>   |
| ShowScrollbar          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                       |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                          |
| TemplateMaximumWidth   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                           |
| TemplatePadding        | 0                                                                                                                                                                                     |
| TemplateSize           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">54.37995540456163<td style="background-color:#ffcccc; width:50%;">Min(160, Self.Height - 60)</td></tr></table> |
| Transition             | Transition.None                                                                                                                                                                       |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">286<td style="background-color:#ffcccc; width:50%;">640</td></tr></table>                                      |
| X                      | 0                                                                                                                                                                                     |
| Y                      | 208.12536443148687                                                                                                                                                                    |
| ZIndex                 | 23                                                                                                                                                                                    |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| DisabledBorderColor | FilterGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                     |
| DisabledFill        | FilterGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(212, 193, 221,.3)</td></tr><tr><td style="background-color:#D4C1DD"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| FocusedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                              |
| HoverBorderColor    | FilterGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                     |
| HoverFill           | FilterGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                            |
| PressedBorderColor  | FilterGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                     |
| PressedFill         | FilterGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                            |

### Child & Parent Controls

| Property       | Value            |
| -------------- | ---------------- |
| Child Control  | galleryTemplate1 |
| Child Control  | Rectangle2       |
| Child Control  | TextBox1         |
| Child Control  | icon2            |
| Child Control  | Rectangle7\_22   |
| Child Control  | Group1           |
| Parent Control | DashboardPage    |

## galleryTemplate1

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

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | FilterGallery |

## galleryTemplate2\_2

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

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## Group1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![group](resources/group.png) | Type: group |

### Design

| Property | Value                                                                                                                                                         |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Height   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">51.9620896374532<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>   |
| Width    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">285.99999999999983<td style="background-color:#ffcccc; width:50%;">5</td></tr></table> |
| X        | 0                                                                                                                                                             |
| Y        | 2                                                                                                                                                             |
| ZIndex   | 3                                                                                                                                                             |

### Color Properties

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | FilterGallery |

## Group11

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
| ZIndex   | 2                                                                                                                                                             |

### Color Properties

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Group12

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
| ZIndex   | 3                                                                                                                                              |

### Color Properties

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Group13

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
| ZIndex   | 4                                                                                                                                              |

### Color Properties

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Group14

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
| ZIndex   | 5                                                                                                                                              |

### Color Properties

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Group2

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
| ZIndex   | 1                                                                                                                                              |

### Color Properties

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## icon2

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(ThisItem.field_0 = "All tickets", UpdateContext({type:"All"}), ThisItem.TicketTypes="New tickets", UpdateContext({type:"New"}), ThisItem.TicketTypes="Tickets in progress", UpdateContext({type:"In progress"}), ThisItem.TicketTypes="Tickets closed", UpdateContext({type:"Closed"}), ThisItem.TicketTypes="Tickets on hold", UpdateContext({type:"On hold"}), ThisItem.TicketTypes="Tickets older than 3 days", UpdateContext({datetype:Text(DateAdd(Today(), -3)),type:"Tickets older than 3 days"}), ThisItem.TicketTypes="Tickets closed today", UpdateContext({datetype:Text(Today()),type:"Tickets closed today"}), ThisItem.TicketTypes="Tickets opened today", UpdateContext({datetype:Text(Today()),type:"Tickets opened today"}))<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                        |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Tooltip         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                        |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoDisableOnSelect    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                               |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">19.6083357122465<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.ChevronRight<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(ThisItem.IsSelected,true,false)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20.6415396952688<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| X                      | 265.358460304731                                                                                                                                                             |
| Y                      | 18.3080368231383                                                                                                                                                             |
| ZIndex                 | 6                                                                                                                                                                            |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>         |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon2.Fill                                                                                                                                                                                                                                                                                                                                    |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon2.BorderColor                                                                                                                                                                                                                                                                                                                             |
| HoverBorderColor    | ColorFade(icon2.BorderColor, 20%)                                                                                                                                                                                                                                                                                                             |
| HoverColor          | ColorFade(icon2.Color, 20%)                                                                                                                                                                                                                                                                                                                   |
| HoverFill           | icon2.Fill                                                                                                                                                                                                                                                                                                                                    |
| PressedBorderColor  | ColorFade(icon2.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                           |
| PressedColor        | ColorFade(icon2.Color, \-20%)                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | icon2.Fill                                                                                                                                                                                                                                                                                                                                    |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | FilterGallery |

## icon2\_2

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate(TicketdetailsPage,ScreenTransition.Fade, {EditRecord:ThisItem, type:ThisItem.Status, assign:ThisItem.AssignedTo, Area:ThisItem.AccountName, priority:ThisItem.Priority, subjectdisabled:true, subjectfill:RGBA(0,0,0,0), subject_visible:true, description_disabled:true, description_bordercolor:RGBA(0,0,0,0), description_fill:RGBA(0,0,0,0), description_visible:true, commentdisabled:true, commentbordercolor:RGBA(0,0,0,0), commentfill:RGBA(0,0,0,0), commentvisible:true})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

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
| X                      | 706.011870817191                                                                                                                                            |
| Y                      | 77.92571006141111                                                                                                                                           |
| ZIndex                 | 8                                                                                                                                                           |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>        |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon2\_2.Fill                                                                                                                                                                                                                                                                                                                                 |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon2\_2.BorderColor                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | ColorFade(icon2\_2.BorderColor, 20%)                                                                                                                                                                                                                                                                                                          |
| HoverColor          | ColorFade(icon2\_2.Color, 20%)                                                                                                                                                                                                                                                                                                                |
| HoverFill           | icon2\_2.Fill                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | ColorFade(icon2\_2.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                        |
| PressedColor        | ColorFade(icon2\_2.Color, \-20%)                                                                                                                                                                                                                                                                                                              |
| PressedFill         | icon2\_2.Fill                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## icon3\_2

| Property                    | Value      |
| --------------------------- | ---------- |
| ![icon](resources/icon.png) | Type: icon |

### Behavior

| Property | Value                                                                                                                                                                                         |
| -------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Navigate(CreatenewticketPage,ScreenTransition.Fade)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

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
| Icon                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Icon.Add<td style="background-color:#ffcccc; width:50%;"></td></tr></table>          |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Rotation               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                |
| X                      | 979                                                                                                                                                         |
| Y                      | 15                                                                                                                                                          |
| ZIndex                 | 26                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>    |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>       |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(193, 193, 193, 0.95)</td></tr><tr><td style="background-color:#C1C1C1"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill        | icon3\_2.Fill                                                                                                                                                                                                                                                                                                                                 |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>          |
| FocusedBorderColor  | icon3\_2.BorderColor                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | ColorFade(icon3\_2.BorderColor, 20%)                                                                                                                                                                                                                                                                                                          |
| HoverColor          | ColorFade(icon3\_2.Color, 20%)                                                                                                                                                                                                                                                                                                                |
| HoverFill           | icon3\_2.Fill                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | ColorFade(icon3\_2.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                        |
| PressedColor        | ColorFade(icon3\_2.Color, \-20%)                                                                                                                                                                                                                                                                                                              |
| PressedFill         | icon3\_2.Fill                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle1

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate( TicketdetailsPage, ScreenTransition.Fade, { EditRecord: ThisItem, type: ThisItem.Status, assign: ThisItem.AssignedTo, Area: ThisItem.AccountName, priority: ThisItem.Priority, subjectdisabled: true, subjectfill: RGBA( 0, 0, 0, 0 ), subject_visible: true, description_disabled: true, description_bordercolor: RGBA( 0, 0, 0, 0 ), description_fill: RGBA( 0, 0, 0, 0 ), description_visible: true, commentdisabled: true, commentbordercolor: RGBA( 0, 0, 0, 0 ), commentfill: RGBA( 0, 0, 0, 0 ), commentvisible: true } )<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">177<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">504<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 0                                                                                                                                                           |
| ZIndex                 | 13                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle1.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>   |
| FocusedBorderColor | Rectangle1.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle1.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle1.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## Rectangle1\_12

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
| ZIndex                 | 7                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle1\_12.Fill                                                                                                                                                                                                                                                                                                                    |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(109,49,162,1)</td></tr><tr><td style="background-color:#6D31A2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_12.BorderColor                                                                                                                                                                                                                                                                                                             |
| HoverFill          | Rectangle1\_12.Fill                                                                                                                                                                                                                                                                                                                    |
| PressedFill        | Rectangle1\_12.Fill                                                                                                                                                                                                                                                                                                                    |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle1\_2

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">148.2987012987013<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X                      | 0                                                                                                                                                           |
| Y                      | 58.701298701298704                                                                                                                                          |
| ZIndex                 | 6                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle1\_2.Fill                                                                                                                                                                                                                                                                                                                          |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(242, 242, 242, .5)</td></tr><tr><td style="background-color:#F2F2F2"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle1\_2.BorderColor                                                                                                                                                                                                                                                                                                                   |
| HoverFill          | Rectangle1\_2.Fill                                                                                                                                                                                                                                                                                                                          |
| PressedFill        | Rectangle1\_2.Fill                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle2

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

| Property               | Value                                                                                                                                                                        |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Solid<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                  |
| DisplayMode            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">DisplayMode.Edit<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">54.0586419753091<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(ThisItem.IsSelected,true,false)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">286<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| X                      | 0                                                                                                                                                                            |
| Y                      | 0                                                                                                                                                                            |
| ZIndex                 | 1                                                                                                                                                                            |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle2.Fill                                                                                                                                                                                                                                                                                                                            |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(212, 193, 221,.5)</td></tr><tr><td style="background-color:#D4C1DD"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle2.BorderColor                                                                                                                                                                                                                                                                                                                     |
| HoverFill          | Rectangle2.Fill                                                                                                                                                                                                                                                                                                                            |
| PressedFill        | Rectangle2.Fill                                                                                                                                                                                                                                                                                                                            |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | FilterGallery |

## Rectangle3\_4

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">558.9365889212828<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| X                      | 306.95845481049565                                                                                                                                          |
| Y                      | 207.8869404904817                                                                                                                                           |
| ZIndex                 | 8                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle3\_4.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(92,92,92,.1)</td></tr><tr><td style="background-color:#5C5C5C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>  |
| FocusedBorderColor | Rectangle3\_4.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle3\_4.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle3\_4.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle6\_10

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
| ZIndex                 | 12                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle6\_10.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle6\_10.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle6\_10.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle6\_10.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle6\_11

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
| ZIndex                 | 13                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle6\_11.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle6\_11.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle6\_11.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle6\_11.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle6\_12

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
| ZIndex                 | 14                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle6\_12.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle6\_12.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle6\_12.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle6\_12.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle6\_13

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
| ZIndex                 | 15                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle6\_13.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle6\_13.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle6\_13.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle6\_13.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle6\_14

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
| ZIndex                 | 16                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle6\_14.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle6\_14.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle6\_14.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle6\_14.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle7\_15

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
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">307<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 207.8235294117647                                                                                                                                           |
| ZIndex                 | 9                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle7\_15.Fill                                                                                                                                                                                                                                                                                                                    |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(92,92,92,.1)</td></tr><tr><td style="background-color:#5C5C5C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>  |
| FocusedBorderColor | Rectangle7\_15.BorderColor                                                                                                                                                                                                                                                                                                             |
| HoverFill          | Rectangle7\_15.Fill                                                                                                                                                                                                                                                                                                                    |
| PressedFill        | Rectangle7\_15.Fill                                                                                                                                                                                                                                                                                                                    |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle7\_16

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">2<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">738<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 176.55714115118243                                                                                                                                          |
| ZIndex                 | 2                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_16.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_16.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_16.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_16.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## Rectangle7\_17

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
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">307<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 260.28767123287525                                                                                                                                          |
| ZIndex                 | 17                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle7\_17.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_17.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle7\_17.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle7\_17.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle7\_18

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
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">307<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 311.3150684931518                                                                                                                                           |
| ZIndex                 | 19                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle7\_18.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_18.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle7\_18.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle7\_18.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle7\_19

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
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1024<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| X                      | 0                                                                                                                                                           |
| Y                      | 207                                                                                                                                                         |
| ZIndex                 | 18                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_19.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_19.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_19.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_19.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle7\_20

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
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">307<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 363.84931506849625                                                                                                                                          |
| ZIndex                 | 20                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle7\_20.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_20.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle7\_20.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle7\_20.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle7\_21

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
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">307<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 416.2465753424715                                                                                                                                           |
| ZIndex                 | 21                                                                                                                                                          |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                       |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>      |
| DisabledFill       | Rectangle7\_21.Fill                                                                                                                                                                                                                                                                                                                         |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, .1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_21.BorderColor                                                                                                                                                                                                                                                                                                                  |
| HoverFill          | Rectangle7\_21.Fill                                                                                                                                                                                                                                                                                                                         |
| PressedFill        | Rectangle7\_21.Fill                                                                                                                                                                                                                                                                                                                         |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## Rectangle7\_22

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
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">307<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| X                      | 0                                                                                                                                                           |
| Y                      | 53.5586419753091                                                                                                                                            |
| ZIndex                 | 2                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                      |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table>     |
| DisabledFill       | Rectangle7\_22.Fill                                                                                                                                                                                                                                                                                                                        |
| Fill               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| FocusedBorderColor | Rectangle7\_22.BorderColor                                                                                                                                                                                                                                                                                                                 |
| HoverFill          | Rectangle7\_22.Fill                                                                                                                                                                                                                                                                                                                        |
| PressedFill        | Rectangle7\_22.Fill                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | FilterGallery |

## Rectangle9\_1

| Property                              | Value           |
| ------------------------------------- | --------------- |
| ![rectangle](resources/rectangle.png) | Type: rectangle |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate(TicketdetailsPage,ScreenTransition.Fade, {EditRecord:ThisItem, type:ThisItem.Status, assign:ThisItem.AssignedTo, Area:ThisItem.AccountName, priority:ThisItem.Priority, subjectdisabled:true, subjectfill:RGBA(0,0,0,0), subject_visible:true, description_disabled:true, description_bordercolor:RGBA(0,0,0,0), description_fill:RGBA(0,0,0,0), description_visible:true, commentdisabled:true, commentbordercolor:RGBA(0,0,0,0), commentfill:RGBA(0,0,0,0), commentvisible:true})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

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
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">177<td style="background-color:#ffcccc; width:50%;"></td></tr></table>               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">6.01979727589484<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| X                      | 0                                                                                                                                                           |
| Y                      | 0                                                                                                                                                           |
| ZIndex                 | 7                                                                                                                                                           |

### Color Properties

| Property           | Value                                                                                                                                                                                                                                                                                                                                  |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 255, 1)</td></tr><tr><td style="background-color:#0000FF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td></td></tr></table></td></tr></table> |
| DisabledFill       | Rectangle9\_1.Fill                                                                                                                                                                                                                                                                                                                     |
| Fill               | If(ThisItem.Status\="In progress",RGBA(195,179,5,1),If(ThisItem.Status\="On hold",RGBA(227,48,12,1),If(ThisItem.Status\="Closed",RGBA(71,185,50,1),RGBA(56,56,153,1))))                                                                                                                                                                |
| FocusedBorderColor | Rectangle9\_1.BorderColor                                                                                                                                                                                                                                                                                                              |
| HoverFill          | Rectangle9\_1.Fill                                                                                                                                                                                                                                                                                                                     |
| PressedFill        | Rectangle9\_1.Fill                                                                                                                                                                                                                                                                                                                     |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## TextBox1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(ThisItem.field_0 = "All tickets", UpdateContext({type:"All"}), ThisItem.TicketTypes="New tickets", UpdateContext({type:"New"}), ThisItem.TicketTypes="Tickets in progress", UpdateContext({type:"In progress"}), ThisItem.TicketTypes="Tickets closed", UpdateContext({type:"Closed"}), ThisItem.TicketTypes="Tickets on hold", UpdateContext({type:"On hold"}), ThisItem.TicketTypes="Tickets older than 3 days", UpdateContext({datetype:Text(DateAdd(Today(), -3)),type:"Tickets older than 3 days"}), ThisItem.TicketTypes="Tickets closed today", UpdateContext({datetype:Text(Today()),type:"Tickets closed today"}), ThisItem.TicketTypes="Tickets opened today", UpdateContext({datetype:Text(Today()),type:"Tickets opened today"}))<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                         |
| Live            | Live.Off                                                                                                                                                             |
| Role            | TextRole.Default                                                                                                                                                     |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.TicketTypes<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                        |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Left                                                                                                                                                   |
| BorderStyle            | BorderStyle.Solid                                                                                                                                            |
| DisplayMode            | DisplayMode.Edit                                                                                                                                             |
| FocusedBorderThickness | 0                                                                                                                                                            |
| Font                   | Font.'Open Sans'                                                                                                                                             |
| FontWeight             | FontWeight.Normal                                                                                                                                            |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">51.9620896374532<td style="background-color:#ffcccc; width:50%;">40</td></tr></table> |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>              |
| Overflow               | Overflow.Hidden                                                                                                                                              |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">20<td style="background-color:#ffcccc; width:50%;">5</td></tr></table>                |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">12<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>               |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                 |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                                         |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">273.50040096231<td style="background-color:#ffcccc; width:50%;">150</td></tr></table> |
| X                      | 0                                                                                                                                                            |
| Y                      | 2                                                                                                                                                            |
| ZIndex                 | 5                                                                                                                                                            |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverBorderColor    | TextBox1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverColor          | TextBox1.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverFill           | TextBox1.Fill                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | TextBox1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedColor        | TextBox1.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedFill         | TextBox1.Fill                                                                                                                                                                                                                                                                                                                                                                                              |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | FilterGallery |

## TextBox1\_20

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
| ZIndex                 | 27                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0,0,0,1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>       |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1\_20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox1\_20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox1\_20.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox1\_20.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox1\_20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox1\_20.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox1\_20.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox1\_21

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
| ZIndex                 | 29                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56,86,153,1)</td></tr><tr><td style="background-color:#385699"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1\_21.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox1\_21.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox1\_21.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox1\_21.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox1\_21.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox1\_21.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox1\_21.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox1\_22

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
| ZIndex                 | 31                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(195,179,5,1)</td></tr><tr><td style="background-color:#C3B305"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1\_22.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox1\_22.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox1\_22.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox1\_22.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox1\_22.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox1\_22.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox1\_22.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox1\_23

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
| ZIndex                 | 33                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(71,185,50,1)</td></tr><tr><td style="background-color:#47B932"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1\_23.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox1\_23.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox1\_23.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox1\_23.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox1\_23.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox1\_23.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox1\_23.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox1\_24

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
| ZIndex                 | 35                                                                                                                                                                             |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(227,48,12,1)</td></tr><tr><td style="background-color:#E3300C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox1\_24.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox1\_24.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox1\_24.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox1\_24.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox1\_24.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox1\_24.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox1\_24.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox2\_20

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
| ZIndex                 | 28                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0,0,0,1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>       |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox2\_20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox2\_20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox2\_20.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox2\_20.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox2\_20.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox2\_20.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox2\_20.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox2\_21

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
| ZIndex                 | 30                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56,86,153,1)</td></tr><tr><td style="background-color:#385699"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox2\_21.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox2\_21.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox2\_21.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox2\_21.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox2\_21.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox2\_21.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox2\_21.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox2\_22

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
| ZIndex                 | 32                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(195,179,5,1)</td></tr><tr><td style="background-color:#C3B305"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox2\_22.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox2\_22.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox2\_22.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox2\_22.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox2\_22.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox2\_22.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox2\_22.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox2\_23

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
| ZIndex                 | 34                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(71,185,50,1)</td></tr><tr><td style="background-color:#47B932"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox2\_23.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox2\_23.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox2\_23.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox2\_23.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox2\_23.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox2\_23.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox2\_23.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox2\_24

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
| ZIndex                 | 36                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(227,48,12,1)</td></tr><tr><td style="background-color:#E3300C"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox2\_24.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox2\_24.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox2\_24.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox2\_24.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox2\_24.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox2\_24.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox2\_24.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox4\_5

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Data

| Property        | Value                                                                                                                                                          |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| Live            | Live.Off                                                                                                                                                       |
| Role            | TextRole.Default                                                                                                                                               |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Service desk"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

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
| ZIndex                 | 11                                                                                                                                                                          |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                           |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | TextBox4\_5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverBorderColor    | TextBox4\_5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverColor          | TextBox4\_5.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverFill           | TextBox4\_5.Fill                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | TextBox4\_5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedColor        | TextBox4\_5.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedFill         | TextBox4\_5.Fill                                                                                                                                                                                                                                                                                                                                                                                              |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox5

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
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                  |
| Width                  | 150                                                                                                                                                                             |
| X                      | 743                                                                                                                                                                             |
| Y                      | 15                                                                                                                                                                              |
| ZIndex                 | 38                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                           |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | TextBox5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverBorderColor    | TextBox5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| HoverColor          | TextBox5.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| HoverFill           | TextBox5.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedBorderColor  | TextBox5.BorderColor                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedColor        | TextBox5.Color                                                                                                                                                                                                                                                                                                                                                                                                |
| PressedFill         | TextBox5.Fill                                                                                                                                                                                                                                                                                                                                                                                                 |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## TextBox5\_63

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate(TicketdetailsPage,ScreenTransition.Fade, {EditRecord:ThisItem, type:ThisItem.Status, assign:ThisItem.AssignedTo, Area:ThisItem.AccountName, priority:ThisItem.Priority, subjectdisabled:true, subjectfill:RGBA(0,0,0,0), subject_visible:true, description_disabled:true, description_bordercolor:RGBA(0,0,0,0), description_fill:RGBA(0,0,0,0), description_visible:true, commentdisabled:true, commentbordercolor:RGBA(0,0,0,0), commentfill:RGBA(0,0,0,0), commentvisible:true})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                          |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                   |
| Live            | Live.Off                                                                                                                                                       |
| Role            | TextRole.Default                                                                                                                                               |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Assigned to:"<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">25.748593878410116<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">99<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| X                      | 14.8333333333339                                                                                                                                                                |
| Y                      | 141.90611273694367                                                                                                                                                              |
| ZIndex                 | 5                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table>    |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(128, 128, 128, 1)</td></tr><tr><td style="background-color:#808080"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                           |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| FocusedBorderColor  | TextBox5\_63.BorderColor                                                                                                                                                                                                                                                                                                                                                                                      |
| HoverBorderColor    | TextBox5\_63.BorderColor                                                                                                                                                                                                                                                                                                                                                                                      |
| HoverColor          | TextBox5\_63.Color                                                                                                                                                                                                                                                                                                                                                                                            |
| HoverFill           | TextBox5\_63.Fill                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedBorderColor  | TextBox5\_63.BorderColor                                                                                                                                                                                                                                                                                                                                                                                      |
| PressedColor        | TextBox5\_63.Color                                                                                                                                                                                                                                                                                                                                                                                            |
| PressedFill         | TextBox5\_63.Fill                                                                                                                                                                                                                                                                                                                                                                                             |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## TextBox5\_64

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate(TicketdetailsPage,ScreenTransition.Fade, {EditRecord:ThisItem, type:ThisItem.Status, assign:ThisItem.AssignedTo, Area:ThisItem.AccountName, priority:ThisItem.Priority, subjectdisabled:true, subjectfill:RGBA(0,0,0,0), subject_visible:true, description_disabled:true, description_bordercolor:RGBA(0,0,0,0), description_fill:RGBA(0,0,0,0), description_visible:true, commentdisabled:true, commentbordercolor:RGBA(0,0,0,0), commentfill:RGBA(0,0,0,0), commentvisible:true})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                                                          |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                   |
| Live            | Live.Off                                                                                                                                                                                                       |
| Role            | TextRole.Default                                                                                                                                                                                               |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">If(IsBlank(ThisItem.AssignedTo), "None", ThisItem.AssignedTo) <td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">25.748593878410116<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">99<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                 |
| X                      | 99.6823899371075                                                                                                                                                                |
| Y                      | 141.90611273694367                                                                                                                                                              |
| ZIndex                 | 6                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_64.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_64.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_64.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_64.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_64.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_64.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_64.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## TextBox5\_73

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate(TicketdetailsPage,ScreenTransition.Fade, {EditRecord:ThisItem, type:ThisItem.Status, assign:ThisItem.AssignedTo, Area:ThisItem.AccountName, priority:ThisItem.Priority, subjectdisabled:true, subjectfill:RGBA(0,0,0,0), subject_visible:true, description_disabled:true, description_bordercolor:RGBA(0,0,0,0), description_fill:RGBA(0,0,0,0), description_visible:true, commentdisabled:true, commentbordercolor:RGBA(0,0,0,0), commentfill:RGBA(0,0,0,0), commentvisible:true})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                          |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                   |
| Live            | Live.Off                                                                                                                                                                       |
| Role            | TextRole.Default                                                                                                                                                               |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Created by: "& ThisItem.Owner<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Lighter<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>   |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30.548807672953497<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">223.519592055824<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                   |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 127.303937355941                                                                                                                                                                |
| Y                      | 7.033272986082783                                                                                                                                                               |
| ZIndex                 | 9                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_73.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_73.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_73.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_73.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_73.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_73.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_73.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## TextBox5\_74

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate(TicketdetailsPage,ScreenTransition.Fade, {EditRecord:ThisItem, type:ThisItem.Status, assign:ThisItem.AssignedTo, Area:ThisItem.AccountName, priority:ThisItem.Priority, subjectdisabled:true, subjectfill:RGBA(0,0,0,0), subject_visible:true, description_disabled:true, description_bordercolor:RGBA(0,0,0,0), description_fill:RGBA(0,0,0,0), description_visible:true, commentdisabled:true, commentbordercolor:RGBA(0,0,0,0), commentfill:RGBA(0,0,0,0), commentvisible:true})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                       |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                |
| Live            | Live.Off                                                                                                                                                                    |
| Role            | TextRole.Default                                                                                                                                                            |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Ticket ID: " & ThisItem.ID<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Lighter<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>   |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30.700246547335105<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">104.840579710145<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                   |
| X                      | 14.0130288391164                                                                                                                                                                |
| Y                      | 6.982793361288898                                                                                                                                                               |
| ZIndex                 | 10                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_74.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_74.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_74.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_74.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_74.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_74.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_74.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## TextBox5\_75

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate(TicketdetailsPage,ScreenTransition.Fade, {EditRecord:ThisItem, type:ThisItem.Status, assign:ThisItem.AssignedTo, Area:ThisItem.AccountName, priority:ThisItem.Priority, subjectdisabled:true, subjectfill:RGBA(0,0,0,0), subject_visible:true, description_disabled:true, description_bordercolor:RGBA(0,0,0,0), description_fill:RGBA(0,0,0,0), description_visible:true, commentdisabled:true, commentbordercolor:RGBA(0,0,0,0), commentfill:RGBA(0,0,0,0), commentvisible:true})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                                                            |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                     |
| Live            | Live.Off                                                                                                                                                                                                         |
| Role            | TextRole.Default                                                                                                                                                                                                 |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Created: " & Text(ThisItem.DateCreated, "mm/dd/yy hh:mm am/pm")<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">TextPosition.Right<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>          |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30.700246547335105<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">218.879344330321<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                   |
| X                      | 491.3556193180601                                                                                                                                                               |
| Y                      | 6.932313736495033                                                                                                                                                               |
| ZIndex                 | 11                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_75.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_75.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_75.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_75.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_75.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_75.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_75.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## TextBox5\_76

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate(TicketdetailsPage,ScreenTransition.Fade, {EditRecord:ThisItem, type:ThisItem.Status, assign:ThisItem.AssignedTo, Area:ThisItem.AccountName, priority:ThisItem.Priority, subjectdisabled:true, subjectfill:RGBA(0,0,0,0), subject_visible:true, description_disabled:true, description_bordercolor:RGBA(0,0,0,0), description_fill:RGBA(0,0,0,0), description_visible:true, commentdisabled:true, commentbordercolor:RGBA(0,0,0,0), commentfill:RGBA(0,0,0,0), commentvisible:true})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                            |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                     |
| Live            | Live.Off                                                                                                                                                                         |
| Role            | TextRole.Default                                                                                                                                                                 |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">"Priority: " & ThisItem.Priority<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">LayoutAlignItems.Center<td style="background-color:#ffcccc; width:50%;">Align.Left</td></tr></table>     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Lighter<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>   |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">30.700246547335105<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">128.697722567287<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                   |
| X                      | 356.635756747438                                                                                                                                                                |
| Y                      | 7.083752610876637                                                                                                                                                               |
| ZIndex                 | 12                                                                                                                                                                              |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>   |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | TextBox5\_76.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverBorderColor    | TextBox5\_76.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| HoverColor          | TextBox5\_76.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverFill           | TextBox5\_76.Fill                                                                                                                                                                                                                                                                                                                                                                                          |
| PressedBorderColor  | TextBox5\_76.BorderColor                                                                                                                                                                                                                                                                                                                                                                                   |
| PressedColor        | TextBox5\_76.Color                                                                                                                                                                                                                                                                                                                                                                                         |
| PressedFill         | TextBox5\_76.Fill                                                                                                                                                                                                                                                                                                                                                                                          |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## TicketsGallery

| Property                          | Value         |
| --------------------------------- | ------------- |
| ![gallery](resources/gallery.png) | Type: gallery |

### Data

| Property        | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AccessibleLabel | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Items           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Sort( If( type = "All", Tickets, If( type = "Tickets older than 3 days", Filter( Tickets, DateCreated <> datetype && DateCreated <> Text(Today()), DateCreated <> Text( DateAdd( Today(), -2 ) ), DateCreated <> Text( DateAdd( Today(), -1 ) ) || DateClosed <> datetype && DateClosed <> Text(Today()), DateClosed <> Text( DateAdd( Today(), -2 ) ), DateClosed <> Text( DateAdd( Today(), -1 ) ) ), If( type = "Tickets opened today", Filter( Tickets, datetype in DateCreated ), If( type = "Tickets closed today", Filter( Tickets, datetype in DateClosed ), Filter( Tickets, type in Status ) ) ) ) ), DateCreated, SortOrder.Descending )<td style="background-color:#ffcccc; width:50%;">CustomGallerySample</td></tr></table> |
| Reset           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Selectable      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">true<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |

### Design

| Property               | Value                                                                                                                                                                                |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| AutoHeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                                    |
| DelayItemLoading       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                      |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                     |
| FocusedBorderThickness | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">4<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                          |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">559.9969834087477<td style="background-color:#ffcccc; width:50%;">575</td></tr></table>                       |
| Layout                 | Layout.Vertical                                                                                                                                                                      |
| LoadingSpinner         | LoadingSpinner.None                                                                                                                                                                  |
| LoadingSpinnerColor    | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">TicketsGallery.BorderColor<td style="background-color:#ffcccc; width:50%;">Self.BorderColor</td></tr></table> |
| ShowScrollbar          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                      |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                         |
| TemplateMaximumWidth   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                          |
| TemplatePadding        | 0                                                                                                                                                                                    |
| TemplateSize           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">178.728206352997<td style="background-color:#ffcccc; width:50%;">Min(160, Self.Height - 60)</td></tr></table> |
| Transition             | Transition.None                                                                                                                                                                      |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">738<td style="background-color:#ffcccc; width:50%;">640</td></tr></table>                                     |
| X                      | 286                                                                                                                                                                                  |
| Y                      | 208.0030165912522                                                                                                                                                                    |
| ZIndex                 | 10                                                                                                                                                                                   |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| DisabledBorderColor | TicketsGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                 |
| DisabledFill        | TicketsGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                        |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| FocusedBorderColor  | Self.BorderColor                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverBorderColor    | TicketsGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                 |
| HoverFill           | TicketsGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                        |
| PressedBorderColor  | TicketsGallery.BorderColor                                                                                                                                                                                                                                                                                                                                                                                 |
| PressedFill         | TicketsGallery.Fill                                                                                                                                                                                                                                                                                                                                                                                        |

### Child & Parent Controls

| Property       | Value               |
| -------------- | ------------------- |
| Child Control  | galleryTemplate2\_2 |
| Child Control  | Rectangle9\_1       |
| Child Control  | Rectangle1          |
| Child Control  | TextBox5\_75        |
| Child Control  | TextBox5\_74        |
| Child Control  | TextBox5\_73        |
| Child Control  | TextBox5\_76        |
| Child Control  | txtSubject          |
| Child Control  | icon2\_2            |
| Child Control  | txtDescription      |
| Child Control  | TextBox5\_63        |
| Child Control  | TextBox5\_64        |
| Child Control  | Rectangle7\_16      |
| Parent Control | DashboardPage       |

## Timer1

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![timer](resources/timer.png) | Type: timer |

### Behavior

| Property   | Value                                                                                                                                                      |
| ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnTimerEnd | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Refresh(Tickets)<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                                                                                  |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| AutoPause       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                        |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                           |
| Duration        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60000<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                                                                        |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">Text(Time(0, 0, Timer1.Value/1000), "hh:mm:ss")<td style="background-color:#ffcccc; width:50%;">Text(Time(0, 0, Self.Value/1000), "hh:mm:ss")</td></tr></table> |

### Design

| Property               | Value                                                                                                                                            |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| Align                  | Align.Center                                                                                                                                     |
| BorderStyle            | BorderStyle.Solid                                                                                                                                |
| DisplayMode            | DisplayMode.Edit                                                                                                                                 |
| FocusedBorderThickness | 4                                                                                                                                                |
| Font                   | Font.'Open Sans'                                                                                                                                 |
| FontWeight             | FontWeight.Normal                                                                                                                                |
| Height                 | 40                                                                                                                                               |
| maximumHeight          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">768<td style="background-color:#ffcccc; width:50%;"></td></tr></table>    |
| maximumWidth           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1366<td style="background-color:#ffcccc; width:50%;"></td></tr></table>   |
| PaddingBottom          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| PaddingLeft            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| PaddingRight           | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| PaddingTop             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| RadiusBottomLeft       | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| RadiusBottomRight      | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| RadiusTopLeft          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| RadiusTopRight         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">11<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>   |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">0<td style="background-color:#ffcccc; width:50%;"></td></tr></table>      |
| VerticalAlign          | VerticalAlign.Middle                                                                                                                             |
| Visible                | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>  |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">150<td style="background-color:#ffcccc; width:50%;">160</td></tr></table> |
| X                      | 41                                                                                                                                               |
| Y                      | 39                                                                                                                                               |
| ZIndex                 | 39                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>ColorFade(Self.Fill, -15%)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>          |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(255,255,255,1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(255, 255, 255, 1)</td></tr><tr><td style="background-color:#FFFFFF"></td></tr></table></td></tr></table>           |
| DisabledBorderColor | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>ColorFade(Self.BorderColor, 70%)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledColor       | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(186, 186, 186, 1)</td></tr><tr><td style="background-color:#BABABA"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>ColorFade(Self.Fill, 90%)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>     |
| DisabledFill        | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(119, 119, 119, 1)</td></tr><tr><td style="background-color:#777777"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>ColorFade(Self.Fill, 70%)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>     |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(62,96,170,1)</td></tr><tr><td style="background-color:#3E60AA"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(56, 96, 178, 1)</td></tr><tr><td style="background-color:#3860B2"></td></tr></table></td></tr></table>               |
| FocusedBorderColor  | Timer1.BorderColor                                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverBorderColor    | ColorFade(Timer1.BorderColor, 20%)                                                                                                                                                                                                                                                                                                                                                                                         |
| HoverColor          | Timer1.Color                                                                                                                                                                                                                                                                                                                                                                                                               |
| HoverFill           | ColorFade(Timer1.Fill, 20%)                                                                                                                                                                                                                                                                                                                                                                                                |
| PressedBorderColor  | ColorFade(Timer1.BorderColor, \-20%)                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedColor        | Timer1.Color                                                                                                                                                                                                                                                                                                                                                                                                               |
| PressedFill         | ColorFade(Timer1.Fill, \-20%)                                                                                                                                                                                                                                                                                                                                                                                              |

### Child & Parent Controls

| Property       | Value         |
| -------------- | ------------- |
| Parent Control | DashboardPage |

## txtDescription

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate(TicketdetailsPage,ScreenTransition.Fade, {EditRecord:ThisItem, type:ThisItem.Status, assign:ThisItem.AssignedTo, Area:ThisItem.AccountName, priority:ThisItem.Priority, subjectdisabled:true, subjectfill:RGBA(0,0,0,0), subject_visible:true, description_disabled:true, description_bordercolor:RGBA(0,0,0,0), description_fill:RGBA(0,0,0,0), description_visible:true, commentdisabled:true, commentbordercolor:RGBA(0,0,0,0), commentfill:RGBA(0,0,0,0), commentvisible:true})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                                |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                         |
| Live            | Live.Off                                                                                                                                                             |
| Role            | TextRole.Default                                                                                                                                                     |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.Description<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">BorderStyle.Dashed<td style="background-color:#ffcccc; width:50%;">BorderStyle.Solid</td></tr></table>   |
| BorderThickness        | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">1<td style="background-color:#ffcccc; width:50%;">0</td></tr></table>                                    |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | FontWeight.Normal                                                                                                                                                               |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">60 <td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                 |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">10<td style="background-color:#ffcccc; width:50%;">13</td></tr></table>                                  |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">651<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                |
| X                      | 14.2091140941637                                                                                                                                                                |
| Y                      | 80                                                                                                                                                                              |
| ZIndex                 | 4                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(204, 204, 204, 1)</td></tr><tr><td style="background-color:#CCCCCC"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(29,33,35,.9)</td></tr><tr><td style="background-color:#1D2123"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>         |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                               |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                              |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                                  |
| Fill                | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(230, 230, 230, 1)</td></tr><tr><td style="background-color:#E6E6E6"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table>    |
| FocusedBorderColor  | txtDescription.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverBorderColor    | txtDescription.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| HoverColor          | txtDescription.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| HoverFill           | txtDescription.Fill                                                                                                                                                                                                                                                                                                                                                                                              |
| PressedBorderColor  | txtDescription.BorderColor                                                                                                                                                                                                                                                                                                                                                                                       |
| PressedColor        | txtDescription.Color                                                                                                                                                                                                                                                                                                                                                                                             |
| PressedFill         | txtDescription.Fill                                                                                                                                                                                                                                                                                                                                                                                              |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |

## txtSubject

| Property                      | Value       |
| ----------------------------- | ----------- |
| ![label](resources/label.png) | Type: label |

### Behavior

| Property | Value                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OnSelect | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">EditForm(TicketDetailsForm); Navigate(TicketdetailsPage,ScreenTransition.Fade, {EditRecord:ThisItem, type:ThisItem.Status, assign:ThisItem.AssignedTo, Area:ThisItem.AccountName, priority:ThisItem.Priority, subjectdisabled:true, subjectfill:RGBA(0,0,0,0), subject_visible:true, description_disabled:true, description_bordercolor:RGBA(0,0,0,0), description_fill:RGBA(0,0,0,0), description_visible:true, commentdisabled:true, commentbordercolor:RGBA(0,0,0,0), commentfill:RGBA(0,0,0,0), commentvisible:true})<td style="background-color:#ffcccc; width:50%;"></td></tr></table> |

### Data

| Property        | Value                                                                                                                                                            |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ContentLanguage | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">""<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                     |
| Live            | Live.Off                                                                                                                                                         |
| Role            | TextRole.Default                                                                                                                                                 |
| Text            | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">ThisItem.Subject<td style="background-color:#ffcccc; width:50%;">"Text"</td></tr></table> |

### Design

| Property               | Value                                                                                                                                                                           |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Align                  | Align.Left                                                                                                                                                                      |
| BorderStyle            | BorderStyle.Solid                                                                                                                                                               |
| DisplayMode            | DisplayMode.Edit                                                                                                                                                                |
| FocusedBorderThickness | 0                                                                                                                                                                               |
| Font                   | Font.'Open Sans'                                                                                                                                                                |
| FontWeight             | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">FontWeight.Semibold<td style="background-color:#ffcccc; width:50%;">FontWeight.Normal</td></tr></table>  |
| Height                 | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">34<td style="background-color:#ffcccc; width:50%;">40</td></tr></table>                                  |
| IsErrorMessage         | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| Overflow               | Overflow.Hidden                                                                                                                                                                 |
| Size                   | 13                                                                                                                                                                              |
| TabIndex               | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">-1<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                    |
| VerticalAlign          | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">VerticalAlign.Top<td style="background-color:#ffcccc; width:50%;">VerticalAlign.Middle</td></tr></table> |
| Width                  | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">651<td style="background-color:#ffcccc; width:50%;">150</td></tr></table>                                |
| Wrap                   | <table border="0"><tr><td style="background-color:#ccffcc; width:50%;">false<td style="background-color:#ffcccc; width:50%;"></td></tr></table>                                 |
| X                      | 14                                                                                                                                                                              |
| Y                      | 43                                                                                                                                                                              |
| ZIndex                 | 3                                                                                                                                                                               |

### Color Properties

| Property            | Value                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BorderColor         | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 18, 107, 1)</td></tr><tr><td style="background-color:#00126B"></td></tr></table></td></tr></table> |
| Color               | <table border="0"><tr><td style="width:50%; background-color:#ccffcc; color:black;"><table border="0"><tr><td>RGBA(47, 47, 47, 1)</td></tr><tr><td style="background-color:#2F2F2F"></td></tr></table></td><td style="width:50%; background-color:#ffcccc; color:black;"><table border="0"><tr><td>RGBA(0, 0, 0, 1)</td></tr><tr><td style="background-color:#000000"></td></tr></table></td></tr></table> |
| DisabledBorderColor | <table border="0"><tr><td>RGBA(56, 56, 56, 1)</td></tr><tr><td style="background-color:#383838"></td></tr></table>                                                                                                                                                                                                                                                                                         |
| DisabledColor       | ColorFade(RGBA(47, 41, 43, 1), 70%)                                                                                                                                                                                                                                                                                                                                                                        |
| DisabledFill        | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| Fill                | <table border="0"><tr><td>RGBA(0, 0, 0, 0)</td></tr><tr><td style="background-color:#000000"></td></tr></table>                                                                                                                                                                                                                                                                                            |
| FocusedBorderColor  | txtSubject.BorderColor                                                                                                                                                                                                                                                                                                                                                                                     |
| HoverBorderColor    | txtSubject.BorderColor                                                                                                                                                                                                                                                                                                                                                                                     |
| HoverColor          | txtSubject.Color                                                                                                                                                                                                                                                                                                                                                                                           |
| HoverFill           | txtSubject.Fill                                                                                                                                                                                                                                                                                                                                                                                            |
| PressedBorderColor  | txtSubject.BorderColor                                                                                                                                                                                                                                                                                                                                                                                     |
| PressedColor        | txtSubject.Color                                                                                                                                                                                                                                                                                                                                                                                           |
| PressedFill         | txtSubject.Fill                                                                                                                                                                                                                                                                                                                                                                                            |

### Child & Parent Controls

| Property       | Value          |
| -------------- | -------------- |
| Parent Control | TicketsGallery |
