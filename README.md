# Improved Instancing Tutorial

This demo adds on the concept of instanced rendering introduced previously.

# About

Extends the concept of Instancing where you draw the same set of coordinates from the Vertex Buffer, only changing the transformation matrix uniform. This allows you draw the same set of geometry several times using the same buffers, only changing the location via the transformation matrix. In this version, instead of calling glDrawArrays or glDrawElements multiple times, we make a single call to glDrawElementsInstanced. When this is done, an gl_instanceID variable is passed into the Vertex Shader which can be used to identify which transformation matrix in the uniform array to use.

# Setup

In order to setup, run the following in a shell, then open the project in your preferred editor. Windows setup has been configured for use with Visual Studio.

Windows:
```
cd path/to/folder
setup.cmd
```
Linux:
```
cd path/to/folder
./setup
```
