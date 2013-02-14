OpenSURF
========

C. Evans, Research Into Robust Visual Features,
MSc University of Bristol, 2008.


Requirements
============

Requres CMake:<br>
http://www.cmake.org/

All code in this package requires the OpenCV library:<br>
http://sourceforge.net/projects/opencvlibrary/

Building
========

<b>Compile & Run Surf:</b>
<pre>
mkdir build
cd build
cmake ..
make
../bin/surffeat
</pre>

This should produce a few executables in bin/, a static library 
lib/libsurf.a, and some HTML documentation in docs/.  You can use the -h 
argument to get help with any of the executables.  libsift.a can be 
compiled into your own code using the standard method:

  gcc -I/path/to/surf/include/ -L/path/to/surf/lib/ yourcode.c -o yourexecutable -lsurf

The documentation in docs/ describes all of the functions available in 
libsurf.a as well as #defines, etc.  Use the documentation to determine 
what header files from include/ to include in your code.

License
=======

This library is distributed under the GNU GPL.
Please use the contact form at http://www.chrisevansdev.com for more information.

Other Info
==========

There are a several examples of code in main.cpp which can be configured
to run by change the value of PROCEDURE which is defined at the top.

If you have any questions contact me via the form on http://www.chrisevansdev.com.

If you want to stay up to date with the library follow @chrisevansdev on twitter.

Please also support the library by visiting our sponsors on http://www.chrisevansdev.com.
