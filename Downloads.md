# Files #

---

  * Generate\_statistics (m file)
  * Generate\_graphs (m file)
  * boundary (mat file)
  * pt\_in\_boundary\_v2 (m file)
  * barycentric\_delaunaytri (m file)


# Description Of The Above Files #

---

  * _Generate\_statistics_
> > creates all the polygons as well as stores the results of the different point in polygon algorithms used. One can insert more algorithms if one wants. Gives a structured output called "stats".

  * _Generate\_graphs_
> > creates different comparison graphs by using the various point in polygon algorithms.

  * _boundary_
> > a structure containing different examples that can be tested with pt\_in\_boundary\_v2 (the new implementation of the point in polygon algorithm).

  * _pt\_in\_boundary\_v2_
> > contains the code to execute the point in polygon test using the concepts of epigraph and hypographs. Use the 'p' option as an argument in the function to see how the implementation works as it processes a polygon.

  * _barycentric\_delaunaytri_
> > contains the code to execute the point in polygon test using the division of the polygon into Delaunay triangles.

# Example to use _pt\_in\_noundary\_v2.m_ #

---


```
  >> load boundary.mat
  >> [IN, label, dist_to_boundary, time_elapsed] = pt_in_boundary_v2(6, 6, boundary(3), 'p');
```

# Files needed to run Generate\_statistics/graphs #

---

  * inpoly.m by Darren Engwirda: 2005­2007 for "Crossover Method" [mfile](http://www.mathworks.com/matlabcentral/fileexchange/10391-fast-points-in-polygon-test)

  * inpolygon.m by Matlab for "Winding Number Rule"


> ## note ##

  * other methods can also be inserted in the Generate\_statistics and Generate\_sraphs.

  * Matlab is needed to run the code.

  * In case of use of the point in polygon via epi-­hypographs (i.e pt\_in\_boundary\_v2.m) and the codes Generate\_statistics.m and Generate\_graphs.m for research publication/presentation/demo please cite the use the following -

# Bibliography #

---


  * Link to proceedings [pdf](http://www.uibk.ac.at/iup/buch_pdfs/icgg2014.pdf)
  * _Point In Polygon Via Epi­Hypo Graphs, Homotopy And Hopf’s Degree Theorem_; Shriprakash Sinha, Luca Nanetti, Remco J. Renken and Gert J. ter Horst; Proceedings of the 16th International Conference on Geometry and Graphics; pages ­982--­­1001; DOI: 10.13140/2.1.1220.9283; Innsbruck, Austria, 2014

```
@INPROCEEDINGS{sinha:2014,
title={Point In Polygon Revisited Via Epi­Hypo Graphs},
author={Sinha, Shriprakash and Nanetti, Luca and Renken, Remco J. and ter Horst, Gert J.},
booktitle = {Proceedings of the 16th International Conference on Geometry and Graphics},
editor = {Hans-Peter Schrocker and Manfred Husty},
publisher = {Innsbruck University Press},
pages = {982--­­1001},
year={2014}
}
```