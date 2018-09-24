# program1

# See CSC561_jtgill_prog1_1

Jonathan Gill
CSC 561
Program 1

Submission

My submission includes two files:
drawstuff.js
index.html

These files are packaged into the compressed folder:
CSC561_jtgill_prog1_1.zip

Code

In this program, I reused the vector class provided by Dr.Watson in exercise 3. I extended this class with a static cross product method and a static length method. However, in this submission of the program the length method was not needed nor used. It may be useful for future assignments.

I defined a helper function side(N,I,V1,V2) to help with detecting ray-triangle intersections. This function works identically to the one described in the #raycasting slides.

I also defined a function color(inputTriangle, lightPos, lightCol, I, E, N, c). This function perform the Blinn-Phong shading by altering the color object c which is passed by reference.

The main portion of my program is defined in the rayCasting(context) function. This function uses the aforementioned classes and function to render triangles using Blinn-Phong shading.

Improvements

This program could be improved by using a more efficient ray-triangle intersection algorithm.

The rayCasting function could be improved by storing the object of closest intersection, and only finding the color for that object. Instead, the current program will find the color for the first valid intersection and overwrite it for any closer valid intersection. This is something I would change if I had more time. Note: This does not alter the output, but the program could run faster by eliminating redundant calls to the color function.

The program would execute much faster if written in a compiled language(ex: C/C++) instead of an interpreted language.

The program would also run faster if hardware acceleration was used(i.e. a video card).
