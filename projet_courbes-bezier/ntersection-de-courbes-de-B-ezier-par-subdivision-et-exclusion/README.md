# ntersection-de-courbes-de-B-ezier-par-subdivision-et-exclusion
Let’s consider the problem of the intersection of two B´ezier 2D-curves of degree n and m
respectively.
1. Each curve is included in the convex hull of its control polygon. Thus, if these two convex hulls
do not intersect, we conclude by the exclusion principle that the two curves do not intersect.

3. This approach is particularly interesting when combined with the principle of subdividing B´ezier
curves. Specifically, in the case where the two convex hulls intersect, the subdivision of each
B´ezier curve (for example, according to parameter α = 1/2) leads to testing the intersection of
of ever-smaller convex hulls (which are also ever closer to the curve).

5. The intersection of two convex polygons (convex hulls) is complex. It is much simpler to
determine the smallest rectangle parallel to the axes that contains each convex hull, then apply
the exclusion principle again and intersect these rectangles.



# we also give a figure that explain the process:
1. The first step involves in the mouse acquiring two BÉzier curves of different degrees.
   
3. after that with a right clique  to make the curve
   
5. the algorithm must :
a) either conclude that the two curves do not intersect,
b) or in case of intersection, for each intersection point :
• display an approximation of the intersection point in the 2D plane as a green point,
• determine an approximation of the intersection parameters ui and vi such that P (ui) ≈
Q(vi) (plot these 2 points as blue and red points),
• improve the accuracy of this intersection thanks to the Newton-Raphson method (plot
these 2 new points as blue and red crosses)

# Result:
in the case of this figure , the result is :

--> INTERSECTIONS IN PARAMETRIC DOMAIN :

Intersection 1: u=0.838600, v=0.008982, point=(2.172449, 1.087073)

Intersection 2: u=0.009998, v=0.493649, point=(-2.763441, 1.970375)
