# How to Bind Array Collection Values in Syncfusion Blazor Chart

## Overview

This sample demonstrates how to display array-based data in a Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts) component. The implementation uses a model that contains a `double[]` array and exposes a calculated property that returns a specific indexed value from that array.

This approach is useful when application data is stored in arrays or collections but chart series require a single numeric field for binding. The sample maps the calculated property to the chart series so that array elements can be rendered as chart points without restructuring the original data source.

## Key Features

- Uses the `SfChart` component to render chart data.
- Configures the primary X-axis through `ChartPrimaryXAxis`.
- Sets `ValueType="Syncfusion.Blazor.Charts.ValueType.Category"` for categorical axis values.
- Binds chart data through the `ChartSeries.DataSource` property.
- Maps category values using `XName="X"`.
- Maps array-derived numeric values using `YName="YValue"`.
- Renders data with `Type="ChartSeriesType.Column"`.
- Demonstrates a `ChartData` model containing:
  - `string X`
  - `double[] Y`
  - `double YValue` computed property returning an indexed array value.
- Uses a collection of `ChartData` objects as the chart data source.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download the repository.
2. Open the project file from the `BlazorApp1` folder.
3. Restore NuGet packages when prompted.
4. Build the project.
5. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Clone or download the repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory.

```bash
cd BlazorApp1
dotnet restore
dotnet run
```

5. Open the local URL displayed in the terminal after the application starts.

## Project Structure

`BlazorApp1/Pages/Index.razor` - Main sample page containing the `SfChart` implementation, chart configuration, model definition, and data binding logic.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the Syncfusion Blazor Chart documentation: https://help.syncfusion.com/chart-sdk/blazor/charts/getting-started

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.