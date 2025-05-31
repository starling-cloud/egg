# Dependencies

Grasshopper relies on two types of dependencies: 

1. **External Geometry**: References geometry declared in Rhino, and 
2. **External Components**: External plugins used within Grasshopper. 

In general, it is best practice to keep dependencies to a very minimum. Especially, when working on a project with several people and over a longer period of time.


## External Geometry

Referencing geometric objects from Rhino with a Grasshopper container is convenient at first, but it requires that the Rhino file is always opened in parallel. Also, the referenced geometry must not be deleted in Rhino; otherwise the connection is lost. The problem is that there is no hint in Rhino that an object is needed by an algorithm. To bypass the problem, at least for simple shapes, it’s possible to right-click the container in Grasshopper and select Internalise data. Now the object is saved within the Grasshopper file. If this is not an option, the referenced geometry should be on an extra layer, have another color or the filename should indicate the dependency.


## External Components

Other dependencies are components that are made available by external plugins for Grasshopper. Using one of them also requires all persons to have the same plugin installed when they’re opening the file. Also be aware that there are rare cases in which plugins are not backwards compatible.

Before using a dependency, you should question yourself, if a plugin offers a unique feature and if it justifies the extra load. If a component from a plugin is used, because it offers a shortcut to replace two or three built-in components, then it’s better to use what’s already available. Also, there are plugins that offer similar features, for example to work with meshes. Here, stick with the components from one plugin and try not to mix them.
