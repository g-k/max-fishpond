Notes on making Maxwell's Fishpond using the 3D printer (Makerbot) at work

Modeling techniques:

* spin around Y-axis: https://web.archive.org/web/20131010045242/http://curriculum.makerbot.com/daily_tutorial/blender/blender_01.html
* constructive solid geometry http://wiki.blender.org/index.php/Doc:2.6/Manual/Modifiers/Generate/Booleans

V1 from `spin-max-fishpond.blend`:

!(2014-09-28 22.18.07.jpg)[top view]
!(2014-09-28 22.18.29.jpg)[view from angle]
!(2014-09-28 22.18.53.jpg)[holes in side]

V1 problems and possible solutions:

* segmented sidewalls
  * subdivide mesh and refit to circular wall
* segmented pond floor
  * subdivide mesh and refit to sphere
* holes in sidewall
  * thicker sidewalls
* hard to remove from print surface (needed knife to remove)
  * print without raft
  * remove extra material on bottom (remove pattern or U-shape of material from base or make smaller)
* inside not watertight
  * use high vertical-resolution
  * treat with acetone - http://blog.reprap.org/2013/02/vapor-treating-abs-rp-parts.html
  * find Blender option Shaun mentioned to test (check for non-manifold edges with ctrl-alt/opt-shift-M and draw new triangles or quads: https://www.shapeways.com/tutorials/prepping_blender_files_for_3d_printing)

Reference:

http://www.technologyreview.com/view/428079/how-to-build-a-maxwells-fishpond/
http://arxiv.org/abs/1206.0003
http://www.qols.ph.ic.ac.uk/~kinsle/files/MFishpond/ (link broken?)
