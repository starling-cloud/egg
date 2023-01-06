# Geometry Pipeline

How many times have you lost your referred geometry in Rhino to a Grasshopper? Whenever you would like to update your dwg file, you need to do a referring job manually. For example, when you update the road line in your project after some modifications, every time you have to right-click on the curve primitive component and click `Set on curve`. A thankless job, especially with many objects in Rhino. 

But I have good news! There is a built-in Grasshopper solution to help you with that. If you haven’t already heard and used the `Geometry Pipeline` component, you should start doing it right now! You can find it under param ribbon and geometry. 

Geometry Pipeline
The geometry pipeline is a link to the opened Rhino model, which lets you auto-reference any geometry. It transfers your geometry into Grasshopper, based on type (point, curve, brep and meshes). Moreover, it is possible to filter geometry based on the names of the objects and layers names. And you can do that even with hidden and locked objects.

As a default under layer and name, an asterisk is set up. It means that absolute every object’s Name and Layer will be piped through the component. In other words, you can automatically select and chose all points or curves that exist in the Rhino file.

![Geometry Pipeline](/assets/image/screenshots/geometry_pipeline.png "Geometry Pipeline")

Let’s go into a practical example…

If you would like to filter one specific layer, type the layer’s full name into the component. Note that the filter notations are case sensitive, so it is essential to write precisely characters with small or big letters. OK, but what if you need all layers that start with the ? Nothing hard. Just put an asterisk after your main name part, and the component will filter the rest for you. Furthermore, you can be more precise and use after your main text a question mark to specify any single character in this place or hashtag to grab just digits (0-9). To show you how does it work. Let’s assume that we have four layers called Roadline 1, Roadline 2, Roadline A, Roadline B. Writing in filter a command filters just layers Roadline 1 and Roadline 2.

Whole list with regular expressions how to use them in Geometry Pipeline you can find below.