# Gnuplot-a fast way to get a quick taste of your hard-earned data
## the gnuplot terminal type is qt

gnuplot> set xlabel 'd1'

gnuplot> set ylabel 'd2'

gnuplot> set ytics 0,1,10

gnuplot> set xtics 0,1,10

gnuplot> ``set pm3d map``


gnuplot> sp 'fes-2cv.dat' u 1:2:3 w pm3d

## add label "A red star" on the generated 2D surface:
gnuplot> set label 1 "*" at 3.5, 2.2, 0 front tc rgb "red" font ",20"

gnuplot> replot

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
