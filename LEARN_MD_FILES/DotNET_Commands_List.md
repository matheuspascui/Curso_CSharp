# DotNET Commands List

### Simple Commands

- Shows the version of the .NET Framework :arrow_right: `dotnet --version `
- Shows a list of the main commands of .NET CLI :arrow_right: `dotnet help`
- list the SDK's downloaded. Note that  **Many versions of SDKs can coexist in the PC** :arrow_right: `dotnet --list-sdks`

### Project Types and How to Start Them

- The Command `dotnet new` creates a new project based on the type informed in the **actual folder**.

- Console Application :arrow_right: `dotnet new console`

- Class Library :arrow_right: `dotnet new classlib`

- ASP.NET Core Project :arrow_right: `dotnet new web`

- ASP.NET Core Project :arrow_right: `dotnet new mvc`

- ASP.NET Core Project :arrow_right: `dotnet new webapi`

- Microsoft Test Project :arrow_right: `dotnet new mstest`

### Execution Flow

- To Restore all packages needed by the application to work properly :arrow_right: `dotnet restore`

- To Compile the application :arrow_right: `dotnet compile` or `dotnet build`

- To Clean previous compilations, it cleans the cache files :arrow_right: `dotnet clean`

- To Compile and Run the application :arrow_right: `dotnet run`

    #### Environment Variables
    - To ensure that my application is running on a specific environment, I must set which environment to run, using the "`--environment`" parameter of the RUN command. Example:
        
        `dotnet run --environment=development`
        
        That command will ensure that my application is running on a **development** environment (and not a production one).
        The `run` command do **not** debug the application, thus it does not break on the breakpoints.

