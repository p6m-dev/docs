#.NET

## Install .NET 8.0
[https://dotnet.microsoft.com/en-us/download/dotnet/8.0](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)

## Usage
Version
```sh
dotnet --version
```
Build
```sh
dotnet build
```
Test
```sh
dotnet test
```

## Setup NuGet with JFrog Artifactory
1. Go to [https://p6m.jfrog.io] (https://p6m.jfrog.io)
2. Login
3. Profile → Set me Up → NuGet → Generate Token and Instructions
4. `dotnet nuget add source  https://p6m.jfrog.io/artifactory/api/nuget/v3/{your_repo}-nuget/index.json --name Artifactory  --username {your_username} --password {your_password_token}`

List NuGet sources
```sh 
dotnet nuget list source
```