- what is blank solution?
    - it is a solution without any project in it.
- what if I open sln file with notepad?
    - it will show some documented text that describe this solution
        
- What is meant if the project type name has the word application?
    - it means it can be an exe file
- Best way to name a project:
    - solution_name.project_name
- Can I add a project of another language?
    - yes, in .NET ecosystem you can add any project in any programming language.
    - why?!
        
        - in compilation process, all the files will be converted into intermediate language (IL) before converting into machine language. (source code → IL)
        - The CLR is responsible for:
            - Just-In-Time (JIT) compilation (IL → native/machine code)
            - Memory management
            - Garbage collection
            - Security
            - Exception handling
        - then OS takes this compiled program and give it all what it need to be a running process
- Content of project file of class library?
    - difference between class library and console app file is the output type. class library doesn’t have output type.
    - it generate .dll files
    - class library and project file reference .netcore.app found in dependencies.
        
    - a tricky way to run class library:
        
- can you use a project object in another project?
    - solution file should be automatically edited after each adding a new item, … you rarely need to edit in this project file.
    - you should add reference project.
    - the object should be accessible from outer projects. (public not internal)
    - right click on the project you need it to use another project in the solution —> add —> project reference —> check the wanted project
    - there will be a change in the project file a new item added:
        
- Compatibility:
    - the framework has many many features. So, there should be compatibility between all the tools and features
        
    - if you have a project a and you need to reference a project b in a. So, project b version (.net 5.0) should be the same or less than project a version (.net 6.0) to achieve compatability.
- Main method:
    
    - each application project should have only one main method (entry point)
    - only the application project should have this main method. So, class library project for example doesn’t have main method.
    - if you have more than one application project and you click run, the project that set as startup project will run only.
    - to make an app startup project, right click on project name —> set as startup project
- how to use namespace?
    - if you want to manage and order classes. like files in directories on your pc.
    - namespace is like a folder and each class is like a file
- to make the help list appear while writing:
    - ctrl + space
- A fully qualified name and how to avoid it:
    - fifo.auto.asia.japan.toyota
    - if you write (using fifo.auto.asia.japan;) above namespace, you will use toyota directly without referencing the fully qualified name
- if we have many classes in our project application what is the solution?
    - we said before we can classify them using namespace but imagine we have many and many classes.
    - the solution here is to put every class in a new file (class library) and put all the classes in a folder. but I made the classes and classified them into namespaces. click left on each class and then: Ctrl + .  —> move to: this will put this class into a new file with its namespaces.
