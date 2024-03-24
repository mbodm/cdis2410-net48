# cdis2410-net48
Port of my cdis2410 tool from .NET8 AOT to .NET Framework 4.8

### What?

I quickly ported my [cdis24010](https://github.com/mbodm/cdis2410) tool from .NET8 AOT to .NET Framework 4.8, for various reasons.

### Notes/Differences

- Project format (*.csproj*) is also "*SDK-sytle project format*"
- *Target Framework Moniker* is "*net48*" instead of "*net8.0*"
- Removed `<ImplicitUsings>enable</ImplicitUsings>` setting (since it's C# language version 7.3)
- Added missing usings (for above reason)
- Removed `<Nullable>enable</Nullable>` setting (since it's C# language version 7.3)
- Souce code is 1:1 ported without any changes
- Published with default setttings (in a *net48* project you can't change them anyway)
- Built on a Windows 10 machine

For anything else, please have a look at https://github.com/mbodm/cdis2410

#### Have fun.
