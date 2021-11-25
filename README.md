# OpenGLTemplate

A template for OpenGL projects that uses [GLFW](https://www.glfw.org/), [GLEW](http://glew.sourceforge.net/) and [GLM](https://github.com/g-truc/glm). [Google Test](https://github.com/google/googletest) is also included for unit
testing. 

## About
This repository contains a simple template that can be used to build graphics projects that rely on OpenGL. It is meant to be used in any machine that supports OpenGL and CMAKE, so it does not make any assumptions about the IDE/text editor you use or your operating system. 

## How to use
To make your project with this template the following steps are suggested. I have tried to make every step as explicit as possible so please do **not** be intimidated by the number of them.
1. Download the code of this repository. Feel free to download it either as a plain file or a Git repository. 
2. Open the directory of the project with cmake. This is done by running `$cmake path/to/OpenGlTemplate`.
3. Build the template. This is done by running `$cmake --build .` (you might get some warnings that you can ignore). You can of course use your favorite IDE with CMAKE integration for this. In this case, set it up and skip to step 6.
4. Now an executable called `template` should have been created. Run it with `./template`. You should now is a black window with "Template" as the title.
5. You have now made sure that the template works for you!
6. Now time to personalise the template. Open the main `CmMakeLists.txt` (can be directly under the template's root) and change every appearance of `template` to your project's name. Any future dependencies should be added here as well.
7. The `main.cpp` file contains the standard GLFW code to open a window, you can change the title of the window from there.
8. Under `Google_tests` you can find `DummyTest.cpp` which is a simple test case that you can delete/replace.
9. Last but not least, you should now that all the dependencies can be found under `dependencies`. You should not have to touch these unless you want to edit the dependencies' source code.

## Some final notes
Feel free to use this template for your project. Should you encounter any difficulties please open an issue here.
Thank you and have fun with OpenGL.
