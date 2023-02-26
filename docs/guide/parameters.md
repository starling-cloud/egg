# Parameters


When naming design parameters in your Rhino Grasshopper scripts, it is important to use clear and descriptive names that accurately reflect the purpose of the parameter. 
Using the following best practices, you can create more readable, understandable, and maintainable definitions in Rhino Grasshopper:

#### 1. Meaningful Mames
Always use descriptive and meaningful names: Use names that describe the purpose or function of the parameter. Avoid using vague or generic names that do not provide enough information about the parameter's role in the definition.

2. Use consistent naming conventions: Use consistent naming conventions throughout your definition. This makes it easier to understand the relationships between different parameters and components.

3. Use camelCase or snake_case: Use either camelCase or snake_case when naming parameters. CamelCase capitalizes the first letter of each word except the first, while snake_case uses underscores to separate words. For example, "numberOfPoints" or "number_of_points".

4. Use abbreviations judiciously: Use abbreviations only when they are commonly understood and widely used. Avoid using obscure or idiosyncratic abbreviations that may be confusing or difficult to understand.

5. Use singular nouns: Use singular nouns when naming parameters, as they are easier to understand and less ambiguous than plural nouns.

6. Use clear units: If the parameter is a measurement, include the units in the parameter name. For example, "length_in_meters" or "radius_in_inches".

7. Be concise: Use short but descriptive names for parameters. Avoid using overly long names that may be cumbersome to type or read.



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

