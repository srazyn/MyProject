# MyProject
This basic unreal project is setup to help troubleshoot build issues.

The standard_library.cc file which includes one function creates compile issues for building in DebugGame mode when it's present in two directories.

Source/MyProject/external/standard_library.cc

Plugins/TestPlugin/Source/TestPlugin/test/standard_library.cc


However if we remove it from the two directories and try to keep it in the plugin directory only while DebugGame compiles fine, we now have issues compiling
in DebugGameEditor mode, with undefined symbols.

We're trying to figure out how to get it to work in both modes. Be it having extra copies of the file, or not.

