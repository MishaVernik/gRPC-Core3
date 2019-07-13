# gRPC-Core3
How to launch Razor pages + using protoBuf + .Net Core3 (unstable at this moment)

# Rules to launch on Windows 
### Step 1
* Open the project
### Step 2
* Build the project 
(you need to install Core3.0 sdk)
### How to install .net core 3.0 
Download via this link
  1. https://dotnet.microsoft.com/download/dotnet-core/3.0
  1. Restart Visual Studio 2019
  1. Activate checkbox "Use preview of the .Net Coe SDK" 
-- pic --
Go to the menu-bar: 
```
Tools - Options - Projects and Solutions - .Net Core
or
Tools - Options - Preview Features 
```
### Step 3
* Open cmd and go to this path where is your project located
##### example:
```
 c:\> g:
 g:\> cd grpc.Server
 g:\grpc.Server > dotnet build
 g:\grpc.Server > dotnet run -f netcoreapp3.0
```

![rule3](https://user-images.githubusercontent.com/41151124/61174065-e31b9a00-a5a3-11e9-83c7-198b2bdc06ae.png)

### By the way, you can use "Multiple start" in the Visual Studio 
  1. Right-click on the Soluion  
  1. Set StartUp Projects
  1. Use start in each drop list 
 ![Blazor gRPC - Microsoft Visual Studio 7_13_2019 7_27_06 PM](https://user-images.githubusercontent.com/41151124/61174096-4b6a7b80-a5a4-11e9-9ba2-0db929acd2d6.png)
### Step 4
* Open gRPC.Server project - Properties - launchSetting.json
### Step 5
* Remember **gRPC.Server - applicationUrl**
> (at the first glance it seems ridiculous, but Windows wishes you all the best). Every time, when you **restart** Visual Studio/Restart Windows, **applicationUrl changes**.
_So do not worry if your application does not work by chance._   
 
