# cdis2410-net48
Ported my [cdis2410](https://github.com/mbodm/cdis2410) tool from .NET8 AOT to .NET Framework 4.8

### What?

I quickly ported my [cdis2410](https://github.com/mbodm/cdis2410) tool from .NET8 AOT to .NET Framework 4.8, for various reasons. It was more or less the result of some testing.

### Notes/Differences?

- Project format (*.csproj*) is also "*SDK-sytle project format*"
- *Target Framework Moniker* is "*net48*" instead of "*net8.0*"
- Removed `<ImplicitUsings>enable</ImplicitUsings>` setting (since it's C# 7.3)
- Added missing usings (for above reason)
- Removed `<Nullable>enable</Nullable>` setting (since it's C# 7.3)
- Souce code is ported 1:1 without any further changes
- Published with default setttings (in a *net48* project you can't change them)
- Built on a Windows 10 machine
- Runs on Windows 11 or Windows 10 ("*May 2019 Update*" or later)
- Runs on any Windows (7, 8, 10 before 05/19) with an installed .NET 4.8 runtime

For anything else, please have a look at https://github.com/mbodm/cdis2410

#### Have fun.
