# Parameters

Design Variables and Parameters


Different types of parameters
Design Variables, or sometimes referred to as User Defined Variables, are those parameters that are crucial to the concept definition of the design. Often those parameters contain numerical inputs that are allowed to change during the design (and/or optimization). A parameter is a symbolic name often associated with a numerical value and which may be changed. Not all parameters are Design Variables but all Design Variables are parameters. Parameters could be constant. If this is the case, do not use sliders to define their values, but Set Numbers instead. Clearly label Design Variables.



Extract Parameters


Extract a parameter
Do not plug Design Variables directly into components, but use paramater containers to clearly identify them. To extract a parameter, right-click the parameter and select Extract Parameter. A new parameter container appears. Depending on the type of parameter you are extracting, this usually is either an integer, or number but can also be text, a boolean, domains, matrices, etc. These parameter containers can be found in Params » Primitive » Integer/Number/...


| Type              | Group             | Syntax            |
| ----------------- | ----------------- | ----------------- |
| Boolean           | Primitive         | (bool)            |
| Box               | Geometry          | (box)             |
| Brep              | Geometry          | (brep)            |
| Circle            | Geometry          | (cir)             |
| Colour            | Primitive         | (col)             |
| Curve             | Geometry          | (crv)             |
| Data              | Primitive         | (dat)             |
| Domain            | Primitive         | (dom)             |
| Geometry          | Geometry          | (geo)             |
| Group             | Geometry          | (grp)             |
| Integer           | Primitive         | (int)             |
| Line              | Geometry          | (ln)              |
| Mesh              | Geometry          | (mesh)            |
| Number            | Primitive         | (num)             |
| Plane             | Geometry          | (pln)             |
| Point             | Geometry          | (pt)              |
| Rectangle         | Geometry          | (rect)            |
| Subdivision       | Geometry          | (subd)            |
| Surface           | Geometry          | (srf)             |
| Time              | Primitive         | (time)            |
| Text              | Primitive         | (txt)             |
| Vector            | Geometry          | (vec)             |

