# .netcoresteps
1. Install the .net SDK
   - Go to https://dotnet.microsoft.com/download to get the .Net Core SDK
   - Click on the 'All .Net Core Downloads...' and download the latest stable (3.1 in my case)
2. Install NodeJs
   - Go to https://nodejs.org/en/ to get NodeJs
   - Click on the option with the LTS and install
3. You may need postman
   - Go to https://www.postman.com/downloads/ to get Postman
4. Open VSCode at the project root you are working on, then...
   - Install extensions...C# (OmniSharp), C# extensions (Jchannon. project no longer developed) , Nuget Package Manager (jmrog), 
  
5. Go to File -> Settings
   - Search for 'Exclude' in the search box, Click on Files, Click 'Add Pattern', Add pattern '**/bin' and '**/obj'
   
6. Open terminal in code and type dotnet run
7. Remember "dotnet watch run" would auto restart our web server
8. Install migration tool (dotnet-ef), type "dotnet tool install --global dotnet-ef" in your project command line

9. The debugger may currently not be available when you go to the debugger tab in VSCode
   - Add a configuration
   - Select .Net Core
   - Select .Net: Attach to local .Net Console App (this adds a new configuration to the configurations in launch.json)
   - Select the configuration and click the play button.
   - Select the {application}.dll from the context menu
