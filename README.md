# .NET MAUI Microcharts Sample
 
This sample app demonstrates how to use Microcharts with .NET MAUI. Because the official Microcharts packages for .NET MAUI are not yet available, I published a set of packages to a separate NuGet package feed on MyGet.

To use the packages, add a NuGet.config to your solution's folder (or just add the `microcharts-preview` feed to an existing NuGet.config file):

```xml
<?xml version="1.0" encoding="utf-8"?>
<configuration>
	<packageSources>
		<!--To inherit the global NuGet package sources remove the <clear/> line below -->
		<clear />
		<add key="nuget" value="https://api.nuget.org/v3/index.json" />
		<add key="microcharts-preview" value="https://www.myget.org/F/microcharts-preview/api/v3/index.json" />
	</packageSources>
</configuration>
```

Then add a reference to the `Microcharts.Maui` package (ensure that the "Include prerelease" option is enabled).

And then use Microcharts! To see how it's used in this app, check out these two files:

1. Register the Microchart controls in [MauiProgram.cs](MauiMicrochartsSample/MauiProgram.cs)
1. Use the control in a XAML file such as [MainPage.xaml](MauiMicrochartsSample/MainPage.xaml)
1. Set the charts contents in a XAML.CS file such as [MainPage.xaml.cs](MauiMicrochartsSample/MainPage.xaml.cs)

To report issues with Microcharts, please check out the [Microcharts repo](https://github.com/microcharts-dotnet/Microcharts).
