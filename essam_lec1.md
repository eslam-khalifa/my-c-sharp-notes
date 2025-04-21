- Most Modern Apps depend on:
    - Data Integrity:
        - all should enter the email and password. it is not optional to enter an email.
    - Security:
        - to secure my website by finding any danger that face this app
    - Reliability:
        - I need my App to run all the time not to work sometimes and become down another times.
    - Performance:
        - Very Responsive (fast)
- Full stack Developer:
    - he is responsible for making Front-End and Back-End
    - He needs to know:
        - Front-End:
            - HTML
            - CSS
            - JavaScript
            - Framework:
                - Angular
                - Vue
                - React
        - Back-End:
            - Distributed Systems
            - Micro Services
            - Back-End Programming Language:
                - C#
            - Database:
                - MS SQL Server
        - Version Source Control:
            - Git & GitHub
- What is .NET?
    - it is a platform to build Apps
        - .Net Framework: last version -> 4.8.1
        - .Net Core: last verion -> 3.1
        - .Net: first version -> .NET 5
    
    - what and when was first version of .NET?
        - it was .NET framework 1.0 in 2002.
    - where was .NET framework used?
        - on windows platform only
    - when was .NET Core created and when was the last version?
        - 2016, version 3.1
        - it was cross-platform
    - what is the first .NET open source project?
        - .NET Core 1.0 and from this version on, all .NET versions are open source
    - What is the next of .NET core 3.1?
        - it was .NET 5.0
        - Microsoft had to release .NET Core 4.X but it found that it will be confusing with .NET framework. So, it launched .NET 5.0
- You need to install visual studio and .NET framework:
    - .NET:
        - [Download .NET (Linux, macOS, and Windows) (microsoft.com)](https://dotnet.microsoft.com/en-us/download)
    - Visual Studio (from here you can download visual studio and see how to install it):
        - [Install Visual Studio and choose your preferred features | Microsoft Learn](https://learn.microsoft.com/en-us/visualstudio/install/install-visual-studio?view=vs-2022)
- Exploring Visual Studio:
    - we need to adjust where to save our project:
        - tools —> options —> project & solution —> general —> location
    - we need to adjust color theme:
        - tools —> options —> Environment —> color theme
    - we need to create new project:
        - file —> new —> project
        - from here you can filter which type you need to make your program. We will start with Console App (deal with CMD).
        - Why to choose CMD?
            - to learn the programming concepts and then learn another tools you need to build something like Web App.
- Solution vs Project?
    - Solution has many projects. each project has namespaces. each namespace has classes.
    - you can put a namespace in another namespace
    - it is better to write a namespace that has all other namespaces and within it write another namespaces if wanted
    - in solution folder, there is solution file and project folder
    - in project folder, there is bin folder, obj folder, project file and class file
    - Shortcut to build your code:
        - Ctrl + Shift + B
    - how to build and run without debugging:
        - Ctrl + F5
    - what is bin folder:
        - Source code you write should be converted to Machine Code (build).
        - after building the code, we will find an exe file in bin folder.
    - How to make the program exe file wait and don’t close the CMD Window after execution immediately?
        - Console.ReadKey(); —> will wait until it reads any key from the keyboard
    - bin vs obj:
        - in compilation time, all project parts will be compiled and stored in a obj folder
        - before run time starts, all project parts will be assembled (linked) and stored in a bin folder
- csproj file:
    - double click on project name from solution explorer
    - its name is: project_name.csproj
- Visual Studio Code terminal commands you need:
    - requirements needed:
        - .NET SDK
        - C# extension
    - create a solution folder:
        
        ```powershell
        mkdir solution_folder_name
        cd MyApp
        ```
        
    - create a solution file (.sln):
        
        ```powershell
        dotnet new sln -n solution_file_name
        ```
        
    - create a console project:
        
        ```powershell
        dotnet new console -n project_file_name
        ```
        
    - add the project file to the solution:
        
        ```powershell
        dotnet sln solution_file_name.sln add project_file_name/project_file_name.csproj
        ```
        
    - create a class library project:
        
        ```powershell
        dotnet new classlib -n class_library_project_name
        ```
        
    - add the class library project to the solution:
        
        ```powershell
        dotnet sln solution_name.sln add class_Library_project_name/class_library_project_name.csproj
        ```
        
    - link the library to the console app:
        
        ```powershell
        dotnet add console_project_name/console_project_name.csproj reference library_class_project_name/library_class_project_name.csproj
        ```
        
    - run the console app (you should be in the solution directory itself e.g. solution_name)
        
        ```powershell
        cd project_name
        dotnet run
        ```
        
    - run a project app (without needing to be inside the directory of it):
        
        ```powershell
        dotnet run --project project_name
        ```
        
    - build the project app (you should be in the solution directory itself e.g. project_name)
        
        ```powershell
        cd project_name
        dotnet build
        ```
        
    - build a project app (without needing to be inside the directory of it):
        
        ```powershell
        dotnet build project_name
        ```
