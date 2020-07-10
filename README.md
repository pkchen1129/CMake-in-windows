# CMake-in-windows
## cmake, make, g++, gcc in windows.

1. Make sure installing MinGW: 

    - [Download link](https://www.youtube.com/watch?v=bhxqI6xmsuA&t=115s)
    - Adding environment to the PATH:\
      Search for "Edit the system environment" -> Environment variables -> click system value "Path" then click edit\
      Add "C:\MinGW\bin" to the PATH

2. CMake:

    - Download CMake at [Link](https://cmake.org/download/) (The .msi file)
    - Adding environeent to the PATH:\
      Search for "Edit the system environment" -> Environment variables -> click system value "Path" then click edit\
      Add "C:\Program Files\CMake\bin"
    - Open the powershell and cd into the build/ directory
    - Then type $cmake.exe -G "MinGW Makefiles" .. 
    - P.S: Should clean the build/ directory everytime.

5. Make:
    - Go to powershell and type: $copy c:\MinGW\bin\mingw32-make.exe c:\MinGW\bin\make.exe
    - Add "C:\MinGW\bin\make.exe" into environment path\
      Then you can make in the build folder
