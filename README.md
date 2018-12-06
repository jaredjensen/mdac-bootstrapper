# Microsoft Access Database Engine 2010 Bootstrapper Package

When packaging the MS Access driver with a .NET application installer, you can specify it as a prerequisite.

For Visual Studio 2017:

1. Clone this repo
2. [Download](https://www.microsoft.com/en-us/download/details.aspx?id=13255) AccessDatabaseEngine.exe and AccessDatabaseEngine_X64.exe
3. Installer project properties dialog > Configuration Properties > Build > Prerequisites > **Microsoft Access Database Engine 2010 (x86, x64)**

The required folder structure is:

```text
%ProgramFiles(x86)%\Microsoft SDKs\ClickOnce Bootstrapper\Packages\MSAccessDBEng2010*
|-- en
|   |-- license.txt
|   |-- package.xml
|-- AccessDatabaseEngine.exe
|-- AccessDatabaseEngine_X64.exe
|-- product.xml
```

\* This path varies depending on VS version and didn't match the registry entry.
