# Gift Wrapping Algorithm
Computational Geometry Project
-Aravindh Shanmuganathan
ID: 467481

Gift Wrapping Algorithm:

The gift wrapping algorithm can be used to find the convex hull of a set of points in a plane. This has a wide range of applications in the field of computational geometry such as collision detection, triangulation , etc. The gift wrapping algorithm has a run time of O〖(n〗^2).
But if we know the number of output points on the convex hull then this is a output sensitive algorithm with a runtime of O(n*h) where h is the number of points on the convex hull.

The Visualization shows the formation of the convex hull in which each step  shows the formation of a single side of the convex edge. The red lines indicate the line between the set of 3 points (p,q,r) for which the orient is calculated.

 Pseudocode:
	Given a set S of n points in a plane:
	Initialize set Convex_Hull.
	Find the leftmost point (left_point) in the set 
	ConvexHull.add(left_point)
	Do while the first point is not revisited:
	For each point loop through every other point:
	Find a point for which Orient(p,q,r) is always negative, i.e. counter clockwise.
	p = q




## Instructions

Project Link : https://aravindh96.github.io/comp_geo/index.html

1) Click to select points inside box, then click Gift wrap button. 

2) Press on 'Step' button to step through the algorithm along each of the convex hull sides.

3) Select 'Reset' button to restart the algorithm.,

## Implementation
I used the d3.js library for drawing shapes. I modified the implementation of Kirkpatricks algorithm to gift wrapping from this repository: https://github.com/rkaneriya/point-location
  
