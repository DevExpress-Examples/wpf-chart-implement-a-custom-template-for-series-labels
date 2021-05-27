<!-- default file list -->
*Files to look at*:

* [Window1.xaml](./CS/Window1.xaml) (VB: [Window1.xaml](./VB/Window1.xaml))
<!-- default file list end -->
# How to provide a custom template for series labels

The following example demonstrates how to change the appearance of [series labels](https://docs.devexpress.com/WPF/6341/controls-and-libraries/charts-suite/chart-control/chart-elements/series/series-point-labels?p=netframework).

To accomplish this, it is necessary to create a [System.Windows.DataTemplate](https://docs.microsoft.com/en-us/dotnet/api/system.windows.datatemplate?view=net-5.0) that specifies the appearance of series labels, and add it to a window's resource. Then, this template can be applied to a series label via its [ChartTextElement.ElementTemplate](https://docs.devexpress.com/WPF/DevExpress.Xpf.Charts.ChartTextElement.ElementTemplate?p=netframework) property.

**Note** that the chart control displays a [crosshair cursor](https://docs.devexpress.com/WPF/14680/controls-and-libraries/charts-suite/chart-control/end-user-features/tooltip-and-crosshair-cursor/crosshair-cursor?p=netframework) instead of series labels in the diagram by default. 

To provide series labels customization, enable series labels (set the [Series.LabelsVisibility](https://docs.devexpress.com/WPF/DevExpress.Xpf.Charts.Series.LabelsVisibility?p=netframework) property to **true**). If you wish, you can disable the crosshair cursor (set the [ChartControl.CrosshairEnabled](https://docs.devexpress.com/WPF/DevExpress.Xpf.Charts.ChartControlBase.CrosshairEnabled?p=netframework) property to **false**).
