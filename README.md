

Introduction
--


This OBS Plugin wraps the OBSApi in Python and provides an embedded Python environment for development of custom Python sources.

This allows you to create custom sources using easily editable Python scripts.

This project is a fork of https://github.com/TheAndyRoid/PythonPlugin, and brings certain improvements:


- Checkout and compile with Visual Studio 2013 directly, no other dependencies. 
- Easy copy/paste installation, integrated with Python and other necessary libraries.
- Fix some bugs in ExampleScripts.

But, this project is not completed yet, for example, missing AudioSource Python wrapper. It is written by pure Python C API, the pro: it's a good example to show how to write a Python Wrapper, the con: there is no [boost::python](http://www.boost.org/doc/libs/1_64_0/libs/python/doc/html/index.html) magic thus no power to make the Python wrapper neat and clean.



Running Demo
--


Here are the ExampleScripts running gifs:
![DateTime demo](https://raw.githubusercontent.com/fyrestone/PythonPlugin/master/images/PythonPlugin_datetime_running.gif)
**DateTime Demo**
![ColorSquare demo](https://raw.githubusercontent.com/fyrestone/PythonPlugin/master/images/PythonPlugin_colorsquare_running.gif)
**ColorSquare Demo**



Usage Instruction
--



Before play ExampleScripts, you should make sure:

- OBS version >= 0.659b, and is 32 bit


Then, follow the steps:
![Plugin loaded](https://raw.githubusercontent.com/fyrestone/PythonPlugin/master/images/PythonPlugin_loaded.png)
Click "Plugins" button, make sure the PythonPlugin is loaded successful.

![Plugin add](https://raw.githubusercontent.com/fyrestone/PythonPlugin/master/images/PythonPlugin_add.png)
Right click in the blank white area below "Sources:" label, add a Python source.

![Plugin enter name](https://raw.githubusercontent.com/fyrestone/PythonPlugin/master/images/PythonPlugin_enter_name.png)
Enter a simple name for this source, then click OK.

![Plugin colorsquare](https://raw.githubusercontent.com/fyrestone/PythonPlugin/master/images/PythonPlugin_colorsquare.png)
Here is the PythonPlugin gui, which is built by tcl in Python. Click "Browse" button and select "ColorSquare.py", make sure your settings are identical to this image. Finally, before click "create" button, don't forget click "Save" button.

![Plugin colorsquare running](https://raw.githubusercontent.com/fyrestone/PythonPlugin/master/images/PythonPlugin_colorsquare_running.gif)
Click "Preview Stream" button in the OBS gui. Wow, your demo is running! Press key "W" "R" "G" "B" in the keyboard and enjoy it.
