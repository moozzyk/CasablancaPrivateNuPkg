Casablanca Private NuGet Package
======== 

Allows building private Casablanca NuGet package. The package is dropped in the bin folder.

Usage:

msbuild build.msbuild {/p:Platform=Win32} {/p:Configuration=Debug} {/p:PlatformToolset=v120} {/p:ApplicationType=Desktop} {/p:Branch=develoment} {/p:NuGetPackageVersion=2.5.0-dev}

Parameters:
- Platform = Win32 | x64 | arm
- Configuration = Debug | Release
- PlatfromToolset = v120 | v110 | v140 etc. (see Casablanca source code for supported toolsets)
- ApplicationType = Desktop | WinRT etc. (see Casablanca source code for supported toolsets)
- Branch = branch to build the NuGet package from
- NuGetPackageVersion=The version of the package to be build - default is {package-version from-.nuspec}-{Branch}
