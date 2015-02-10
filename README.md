# glfw3-triangle-example
A simple glfw3 example application. Builds 32 and 64 bit binaries with dependencies included on windows. Open the Visual Studio 2013 projects and build. Building on unix is pretty straightforward. You could do the following...

```shell
# download glfw3 source code
cd <glfw-source-code>
mkdir build
cd build
cmake ../
make
make install
cd <this-repository>
g++ `pkg-config --cflags glfw3` -o main glfw-fun/main.cc `pkg-config --static --libs glfw3`
./main
```

Have Fun
