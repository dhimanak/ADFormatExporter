# ADFormatExporter
3D format converter utility. This program takes in most of the renowned  3D formats(.obj, .dae,  .3ds, .max, .fbx)  and convert it to Threejs(ready for web)

Prerequisites:
Latest version of Python must be installed with setting to environment variable path option selected.  

Step-by-step guide for ADFormatExporter utility
Utility can only be used on windows command line. It has following options:
Option	Required/Optional	Summary
-i	Required	Used for input path for file or folder
-p	Optional	Path to python executable, if python is not added to environment variables
-o	Optional	Output path for converted threejs files or folder


Usages examples
There are different ways to use the utility which are as explained below:

ADFormatExporter.exe -i "D:\3DModels\zeb"
Converts all 3d files in the folder D:\3DModels\zeb to threejs files and puts them into default Output folder.

ADFormatExporter.exe -i "D:\3DModels\zeb\test.obj" –o "D:\3DModels\zeb\test.js"
One to one file conversion

ADFormatExporter.exe -i "D:\3DModels\zeb"  -o "D:\3DModels\zeb1"
Converts all 3d files in the folder D:\3DModels\zeb to threejs files and puts them into specified output folder i.e.  D:\3DModels\zeb1.

ADFormatExporter.exe -p "C:\Users\Anil\AppData\Local\Programs\Python\Python36-32\python.exe"   -i "D:\3DModels\zeb"  -o "D:\3DModels\zeb1"
Python executable path can also be supplied but its optional


This utility uses Autodesk FBXConverter and convert_to_threejs.py script as a bases for conversion.
