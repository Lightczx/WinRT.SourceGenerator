# WinRT.SourceGenerator

Orignal codes are copied from [CsWinRT](https://github.com/microsoft/CsWinRT/tree/master/src/Authoring/WinRT.SourceGenerator)

Modifed the `Generator.SourceGenerator` and related code to implements `IIncrementalGenerator`.
Use `RegisterImplementationSourceOutput` to avoid unnecessary generation attempt.

## Usage
1. Download the `WinRT.SourceGenerator.dll` from release or clone this repo and build yourself.
2. Find the Microsoft.Windows.CsWinRT nuget package local cache and the correct version.
3. Find `analyzers/dotnet/cs/WinRT.SourceGenerator.dll`
3. Replace the file and restart Visual Studio.

Now you should see your CPU calm down again.

> Not fully tested and should use the official build once Microsoft implement this.