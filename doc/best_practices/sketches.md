# Sketches

Making sketches on your script can be a useful visual solution. In a huge script, it will be easier to refer to particular parts in your construction. 

The first step is to create a sketch object. The second step is to import the whole .dwg file to Rhino and export it to a Grasshopper script. It can be for example the whole bridge or just a small cross-section where you can refer to your script. With extra arrows, you can show which part of the structure refers to which part of the script so that it’s easier for your colleagues to work in your script.



Sketch in Grasshopper
Draw function in Grasshopper is not the best one I have ever seen. My created lines are always ugly, and it is impossible to make a straight line.

However, making sketches on your script can be a helpful visual solution thanks to the function called – load from Rhino. Just right click on the sketched line and choose Load from Rhino. If your Rhino geometry is placed near zero points, then imported geometry in Grasshopper will be placed in the top left corner on the canvas. You can import frames, lines or even huge text visible for everyone in a big script.

More than that, you can import whole dwg drawings. In a colossal script, it will be easier to refer to particular parts in your construction. For example, it can be the entire bridge or just a tiny cross-section where you can refer to your script with extra arrows.

You can show which part of the structure refers to which part of the script so that it’s easier for your colleagues to work on your script.







When it is needed to establish an order to some elements depending of its geometrical position, a good practice will be doing a sketch in the Grasshopper workspace. For instance, if we want to get individually the vertices of an hexagon and we want to help an external person to identify them, we could do what follows:


> Draw the geometry in Rhino, taking in consideration that the dimensions of the grid used in Grasshopper are 15×5 units, and the upper left point of the workspace corresponds to the 0,0,0 in Rhino.

> Draw a scribble with “Sketch Object” in Grasshopper.


> Right-click on the scribble and select “Load from Rhino”.


> Modify its colour and thickness if necessary and it is ready to continue working.


https://www.modelical.com/en/best-practices-in-grasshopper/