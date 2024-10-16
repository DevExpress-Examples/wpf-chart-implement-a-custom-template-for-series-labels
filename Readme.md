<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128570103/22.2.2%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/E1258)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
[![](https://img.shields.io/badge/💬_Leave_Feedback-feecdd?style=flat-square)](#does-this-example-address-your-development-requirementsobjectives)
<!-- default badges end -->

# WPF Chart - How to Implement a Custom Template for Series Labels

The following example demonstrates how to change the appearance of [series labels](https://docs.devexpress.com/WPF/6341/controls-and-libraries/charts-suite/chart-control/chart-elements/series/series-point-labels?p=netframework).

![Chart](./image/Chart.png)

To accomplish this, create a [System.Windows.DataTemplate](https://docs.microsoft.com/en-us/dotnet/api/system.windows.datatemplate?view=net-5.0) that specifies the appearance of series labels, and add it to a window's resource. Then, this template can be applied to a series label with its [ChartTextElement.ElementTemplate](https://docs.devexpress.com/WPF/DevExpress.Xpf.Charts.ChartTextElement.ElementTemplate?p=netframework) property.

**Note** that the chart control displays a [crosshair cursor](https://docs.devexpress.com/WPF/14680/controls-and-libraries/charts-suite/chart-control/end-user-features/tooltip-and-crosshair-cursor/crosshair-cursor?p=netframework) instead of series labels in the diagram by default. 

To implement series labels customization, enable series labels (set the [Series.LabelsVisibility](https://docs.devexpress.com/WPF/DevExpress.Xpf.Charts.Series.LabelsVisibility?p=netframework) property to **true**). If you wish, you can disable the crosshair cursor (set the [ChartControl.CrosshairEnabled](https://docs.devexpress.com/WPF/DevExpress.Xpf.Charts.ChartControlBase.CrosshairEnabled?p=netframework) property to **false**).

## Files to Review

* [Window1.xaml](./CS/Window1.xaml) (VB: [Window1.xaml](./VB/Window1.xaml))

## Documentation

* [Series Point Labels](https://docs.devexpress.com/WPF/6341/controls-and-libraries/charts-suite/chart-control/series/series-point-labels)
<!-- feedback -->
## Does this example address your development requirements/objectives?

[<img src="https://www.devexpress.com/support/examples/i/yes-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=wpf-chart-implement-a-custom-template-for-series-labels&~~~was_helpful=yes) [<img src="https://www.devexpress.com/support/examples/i/no-button.svg"/>](https://www.devexpress.com/support/examples/survey.xml?utm_source=github&utm_campaign=wpf-chart-implement-a-custom-template-for-series-labels&~~~was_helpful=no)

(you will be redirected to DevExpress.com to submit your response)
<!-- feedback end -->
