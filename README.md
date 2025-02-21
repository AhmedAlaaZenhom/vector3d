# Vector3D readme

__Vector3D__ is a lightweight package, written on python, for working with vectors and points in 3D decartian system.



## Installing
You can install vector3d from pip:
`python3 -m pip install vector3d
or by downloading a .whl file from one of releases and installing it using this command:
`python -m pip install filename.whl
or you should download  a source .tar.gz archive from one of releases, unpack it and install with following command:
`python3 setup.py build
`python3 setup.py install


## Reference

### vector3d.vector
Implements the Vector class and vector related functions.

#### vector3d.vector.Vector
A vector class.
Can be created as:
* Vector(x,y,z)
* Vector(x, y, z=0)
* Vector(x, y=0, z=0)
* or simply Vector() which is equivalent to Vector(0, 0, 0)

#### Functions in vector3d.vector
* from_points(a, b) - creates a vector from pair of points, begining and ending of vector.
* angle(a, b) - calculates angle between vectors a and b.
* horizontal_angle(a, b) - calculates angle between vectors a and b, but without Z coordinate (projections of a and b to XY plane).
* vertical_angle(a, b) - calculates angle between vectors a and b, but without X coordinate (projections of a and b to YZ plane)


### vector3d.point
Implements a Point class and point related functions.

#### vector3d.point.Point
A class for the point in 3D decartian system.
This class have only three attributes and: x, y and z coordinate of the point, and has no methods yet.
A Point can be created with following constructors:
* Point(x, y, z)
* Point(x, y, z=0)
* Point(x, y=0, z=0)
* Or even Point() which is equivalent to Point(0, 0, 0)


#### Functions in vector3d.point
* distance(a, b) - calculates distance between two points
* center(a, b) _ calculates coordinates of the center between two points (returns a Point object)

