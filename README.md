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
![Blazor gRPC - Microsoft Visual Studio 7_14_2019 11_26_46 AM](https://user-images.githubusercontent.com/41151124/61181132-667fce80-a62a-11e9-8c29-5eeec634c132.png)

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
![Blazor gRPC - Microsoft Visual Studio 7_13_2019 7_42_35 PM (2)](https://user-images.githubusercontent.com/41151124/61174271-866dae80-a5a6-11e9-85db-dba66ceffa72.png)

### Step 6
* Open gRPC.Client - Pages - Index.razor
##### Change to the remebmbered applicationUrl
![Blazor gRPC - Microsoft Visual Studio 7_13_2019 7_45_39 PM (2)](https://user-images.githubusercontent.com/41151124/61174311-f2e8ad80-a5a6-11e9-9548-4e205bbb8d50.png)

### Step 7 
* Run gRPC.Client
![gRPC Client - Google Chrome 7_13_2019 7_51_19 PM](https://user-images.githubusercontent.com/41151124/61174370-b5d0eb00-a5a7-11e9-9fc8-de10e5ecd870.png)

## That's all

### But with the following updates you need to do some changes in the project file
![Blazor gRPC - Microsoft Visual Studio 7_13_2019 7_54_37 PM (2)](https://user-images.githubusercontent.com/41151124/61174403-2415ad80-a5a8-11e9-8414-e0d66d7984e6.png)

