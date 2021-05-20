# Java Chromium Embedded example for Windows only
 JCEF (Java Chromium Embedded Frameword) Chromium version 88 with all necessary binaries working in Java

**Java Chromium Embedded Framework binary distrib**

This is the binary version of the JCEF project [java-cef](https://bitbucket.org/chromiumembedded/java-cef) that integrates the Chromium browser (version 88).

This binary version is a release build for x64 architecture and was compiled with Visual Studio 2013 (C++).


---

## Download

Download the entire repository in a folder on your computer.


---

## Running

You will need a JVM to run this software.

To run the software, simply go into the repository folder and then launch run.bat


---

## Result

If it works fine on your computer, a new window will appear. After that, you can type a URL and it will display the associated website.


---

## How to do it yourself

If you want to compile JCEF yourself on Windows, follow these steps below.

1. Download and install CMake (cmake.org)
2. Go into the directory where you will find vcvars64.bat in c:\Program Files (x86)  
You usually find this file into C:\Program Files (x86)\"Your version of Visual Studio"\VC\bin\"your x64 architecture"
3. Open a command prompt and run vcvars64.bat into the folder of your version of Visual Studio\VC\bin
4. Go into the directory where you downloaded [JCEF project](https://bitbucket.org/chromiumembedded/java-cef)
5. Create a directory javacef_build into the src directory of JCEF project
6. Go into this directory
7. Run this command cmake -G "Visual Studio" -A x64 ..  
You will now search the correct name of your Visual Studio at the output text
8. Run this command cmake -G "&lt;The correct name of your Visual Studio&gt;" -A x64 ..  
If it works fine, it will download the CEF package automatically.
If not, try another architecture name like Win64 or windows64.
9. When it's finished, you have a jcef.sln file. Double click on this file.
10. When Visual Studio is started and the project is loaded, select Release into the Configuraton Manager
11. Build the solution  
This build takes almost two days depending on your computer's performance. When it's finished you will have the compiled .dll
12. Go to tools from the directory src of java_cef
14. Run make_distrib.bat
 
