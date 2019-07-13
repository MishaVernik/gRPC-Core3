# gRPC-Core3
How to launch Razor pages + using protoBuf + .Net Core3 (unstable for this moment)

# Rules to launch on Windows 
* 1. Open the project
* 2. Build the project 
(you need to install Core3.0 sdk)
---How to install .net core 3.0 
Download via this link
1. https://dotnet.microsoft.com/download/dotnet-core/3.0
2. Restart Visual Studio 2019
3. Activate checkbox "Use preview of the .Net Coe SDK" 
-- pic --
Go to the menu-bar: 
Tools - Options - Projects and Solutions - .Net Core
or
Tools - Options - Preview Features 
---
* 3. Open cmd and go to this path where is your project located
(example: 
 c:\> g:
 g:\> cd grpc.Server
 g:\grpc.Server > dotnet build
 g:\grpc.Server > dotnet run -f netcoreapp3.0
-- pic -- 
By the way, you can use "Multiple start" in the Visual Studio 
1. Right-click on the Soluion 
2. Set StartUp Projects
3. Use start in each drop list 
-- pic --   
* 4. Run project 
 
