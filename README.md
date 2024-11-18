# cdis2410-net48
Port of [cdis2410](https://github.com/mbodm/cdis2410) tool (from .NET8 AOT to .NET Framework 4.8)

### What?
I quickly ported my [cdis2410](https://github.com/mbodm/cdis2410) tool from .NET8 AOT to .NET Framework 4.8, for various reasons. It was more or less the result of some testing.

### But, why?
Nowadays .NET 8 AOT does a great job in creating smaller binaries (around 2MB). But a .NET 4.8 binary is still much smaller (around 7KB). Of course this battle is easy to win for the latter, just because for the simple fact, that a NET48 binary is framework-dependent by default. Of course a NET8 framework-dependent variant is also that small. But since every Windows 10/11 machine contains the NET48 runtime, out of the box, a NET48 binary runs, without the need of separately installing a runtime. Which feels like you get that smaller size "for free" (in contrast of installing a runtime). Therefore i thought it's worth to provide both variants.

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
- Runs on any Windows (7, 8, or 10 before 05/19) with an installed .NET 4.8 runtime

For anything else please have a look at https://github.com/mbodm/cdis2410

#### Have fun.
