# welcome gnupl-frec
appendix gnuplot radios frequency to guides platform about the shark to analysis about base of position about limit of elements about utilization of mechanism latter to contribution of logic to apo output to side of platform about yields.
```gnuplot
#!/usr/bin/gnuplot -persist
#
#    
#    	G N U P L O T
#    	Version 5.4 patchlevel 2    last modified 2021-06-01 
#    
#    	Copyright (C) 1986-1993, 1998, 2004, 2007-2021
#    	Thomas Williams, Colin Kelley and many others
#    
#    	gnuplot home:     http://www.gnuplot.info
#    	faq, bugs, etc:   type "help FAQ"
#    	immediate help:   type "help"  (plot window: hit 'h')
# set terminal pngcairo  background "#ffffff" enhanced font "Verdana,10" fontscale 1.0 size 350, 262 
# set output 'animation/water050.png'
unset clip points
set clip one
unset clip two
unset clip radial
set errorbars front 1.000000 
unset border
set zdata 
set ydata 
set xdata 
set y2data 
set x2data 
set boxwidth
set boxdepth 0
set style fill  empty border
set style rectangle back fc  bgnd fillstyle   solid 1.00 border lt -1
set style circle radius graph 0.02 
set style ellipse size graph 0.05, 0.03 angle 0 units xy
set dummy u, v
set format x "% h" 
set format y "% h" 
set format x2 "% h" 
set format y2 "% h" 
set format z "% h" 
set format cb "% h" 
set format r "% h" 
set ttics format "% h"
set timefmt "%d/%m/%y,%H:%M"
set angles radians
set tics back
unset grid
unset raxis
set theta counterclockwise right
set style parallel front  lt black linewidth 2.000 dashtype solid
set key notitle
set key fixed right top vertical Right noreverse enhanced autotitle nobox
set key noinvert samplen 4 spacing 1 width 0 height 0 
set key maxcolumns 0 maxrows 0
set key noopaque
unset key
unset label
unset arrow
unset style line
unset style arrow
set style histogram clustered gap 2 title textcolor lt -1
unset object
unset walls
set style textbox  transparent margins  1.0,  1.0 border  lt -1 linewidth  1.0
set offsets 0, 0, 0, 0
set pointsize 1
set pointintervalbox 1
set encoding default
unset polar
set parametric
unset spiderplot
unset decimalsign
unset micro
unset minussign
set view 40, 200, 1, 1
set view azimuth 0
set rgbmax 255
set samples 100, 100
set isosamples 200, 100
set surface 
unset contour
set cntrlabel  format '%8.3g' font '' start 5 interval 20
set mapping cartesian
set datafile separator whitespace
set datafile nocolumnheaders
unset hidden3d
set cntrparam order 4
set cntrparam linear
set cntrparam levels 5
set cntrparam levels auto
set cntrparam firstlinetype 0 unsorted
set cntrparam points 5
set size ratio 0 1,1
set origin 0,0
set style data points
set style function lines
unset xzeroaxis
unset yzeroaxis
unset zzeroaxis
unset x2zeroaxis
unset y2zeroaxis
set xyplane relative 0.5
set tics scale  1, 0.5, 1, 1, 1
set mxtics default
set mytics default
set mztics default
set mx2tics default
set my2tics default
set mcbtics default
set mrtics default
set nomttics
unset xtics
unset ytics
unset ztics
unset x2tics
unset y2tics
unset cbtics
unset rtics
unset ttics
set title "" 
set title  font "" textcolor lt -1 norotate
set timestamp bottom 
set timestamp "" 
set timestamp  font "" textcolor lt -1 norotate
set trange [ * : * ] noreverse nowriteback
set urange [ 0.00000 : 18.0711 ] noreverse nowriteback
set vrange [ 0.00000 : 4.71239 ] noreverse nowriteback
set xlabel "" 
set xlabel  font "" textcolor lt -1 norotate
set x2label "" 
set x2label  font "" textcolor lt -1 norotate
set xrange [ * : * ] noreverse writeback
set x2range [ * : * ] noreverse writeback
set ylabel "" 
set ylabel  font "" textcolor lt -1 rotate
set y2label "" 
set y2label  font "" textcolor lt -1 rotate
set yrange [ * : * ] noreverse writeback
set y2range [ * : * ] noreverse writeback
set zlabel "" 
set zlabel  font "" textcolor lt -1 norotate
set zrange [ -1.00000 : 1.00000 ] noreverse nowriteback
set cblabel "" 
set cblabel  font "" textcolor lt -1 rotate
set cbrange [ -1.00000 : 1.00000 ] noreverse nowriteback
set rlabel "" 
set rlabel  font "" textcolor lt -1 norotate
set rrange [ * : * ] noreverse writeback
unset logscale
unset jitter
set zero 1e-08
set lmargin at screen 0.03
set bmargin at screen 0
set rmargin at screen 0.97
set tmargin at screen 1
set locale "pt_BR.UTF-8"
set pm3d explicit at s
set pm3d depthorder 
set pm3d interpolate 1,1 flush begin noftriangles noborder corners2color mean
set pm3d clip z 
set pm3d nolighting
set palette positive nops_allcF maxcolors 0 gamma 1.5 color model RGB 
set palette rgbformulae 3, 9, 9
set colorbox vertical origin screen 0.9, 0.2 size screen 0.05, 0.6 front  noinvert bdefault
unset colorbox
set style boxplot candles range  1.50 outliers pt 7 separation 1 labels auto unsorted
set loadpath 
set fontpath
set psdir
set fit brief errorvariables nocovariancevariables errorscaling prescale nowrap v5
bessel(x,t) = besj0(x) * cos(2*pi*t)
GNUTERM = "wxt"
I = {0.0, 1.0}
VoxelDistance = 0.0
n = 6
k = 18.0641577581413
u_0 = 18.0710775381829
t = 1.0
end_time = 1
outfile = "animation/water050.png"

splot u*sin(v),u*cos(v),bessel(u,t) w pm3d ls 1
#    EOF
```
