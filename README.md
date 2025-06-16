# Gnuplot-a fast way to get a quick taste of your hard-earned data
## the gnuplot terminal type is qt

gnuplot> ``set xlabel 'd1'``

gnuplot> ``set ylabel 'd2'``

gnuplot> ``set ytics 0,1,10``

gnuplot> ``set xtics 0,1,10``

gnuplot> ``set pm3d map``


gnuplot> ``sp 'fes-2cv.dat' u 1:2:3 w pm3d``

## add label "A red star" on the generated 2D surface:
gnuplot> ``set label 1 "*" at 3.5, 2.2, 0 front tc rgb "red" font ",20"``

gnuplot> ``replot``

"★" is a Unicode star.
Adjust the coordinates (x, y, z) as needed.
font ",20" sets the font size.
tc rgb "red" makes it in red color.
front ensures it shows on top.

# To Remove a Specific Label:

a. If you know the label number (e.g. label 1), run:
unset label 1
replot


![adding labels](https://github.com/HuixiaLuScienceRocks/gnuplot_tricks/blob/main/fes-2cv.png))
gnuplot> ``set pm3d map``

gnuplot> ``sp 'fes-2cv.dat' u 1:2:3 w pm3d``

gnuplot> ``set label 1 "*" at 8.97, 2.026, 0 front tc rgb "blue" font ",20"``

gnuplot> ``replot``

gnuplot> ``set label 2 "crystal structure" at 8.0, 1.726, 0 front tc rgb "blue" font ",15"``

gnuplot> ``replot``

gnuplot> ``set label 3 "*" at 4.527, 0.607, 0 front tc rgb "green" font ",20"``

gnuplot> ``replot``

gnuplot> ``set label 3 "cluster2-amber" at 3.65, 1.1, 0 front tc rgb "green" font ",15"``

gnuplot> ``replot``
