.. _magnetics_buried_dipole:

Fields due to a magnetic dipole
********************************


The general principles of magnetic surveying are encapsulated into the following steps:

(a) An object with magnetic susceptibility \\(\\kappa\\) is buried in the earth. 
(b) At the location of burial, the earth's field magnetic field is \\(\\vec{H}\\) and the magnetization in the object is \\(\\vec{M} = \\kappa \\vec{H}\\).
(c) If the object is "small", that is all of the object's dimensions are several times smaller than the depth to its center, then  the object acts as a "magnetic dipole" -- that is, a little bar magnet with strength and direction caused by the inducing field. The  dipole moment of the magnet is \\(\\vec{m} = \\text{Volume} * \\vec{M}\\)
(d) The magnetic field of the object is referred to as the "secondary" field or sometimes the "anomalous" field \\(\\vec{B_a}\\). This is what we seek to measure. 
(e) \\(\\vec{B_a}\\) is a vector field and hence requires three components to specify it. In the accompanying applet observations of individual components \\((B_x,B_y,B_z)\\) can be displayed. The projection of \\(\\vec{B_a}\\) onto the direction of Earth's field \\(\\hat{B_0}\\) is displayed as \\(B_t\\). See xxx linkgpg xxx.  In addition the vertical gradient of the field, obtained if measurements were acquired with a gradiometer, are listed as \\(B_g\\).  Sign conventions must be adopted when data are plotted. For magnetic surveying the coordinate system used is: {\\(x\\) is northing, \\(y\\) is easting, and \\(z\\) is downward}.  The sign convention will be that horizontal fields are positive if they point in the \\(\\hat{x}\\) direction for \\(B_x\\), in the \\(\\hat{y}\\) direction for \\(B_y\\) and vertical fields are positive if they point downward. For \\(B_t\\) the anomaly is positive if it points in the same direction as the earth's field and negative if it is the opposite direction. 

Understanding the magnetic fields of a buried dipole, and the resultant observations, is crucial because all real scenarios can be thought of as a combination (superposition) of dipoles (see the "Buried structures" section). More advanced applets will be used to look at some of the responses of some of these bodies.


The figures below illustrate the problem. The pattern recorded at the surface arises by measuring the field strength everywhere on the surface, removing the Earth's field, and then plotting the results as a contour map of anomalous field strength. In the third figure, regions of blue anomalous field are "negative" because at those surface locations, the **anomalous** field crossing that surface points in the opposite direction for Earth's field.

.. raw:: html
    :file: buried_dipole.html

Magnetic dipoles: a Java applet
-------------------------------

As noted above, a real buried feature will look like a magnetic dipole if its physical dimensions are much smaller than the depth to the feature's center.

The response that will be measured at points on a surface overlying a buried magnetic dipole can be explored using the UBC-GIF magnetic dipole Java applet; click here_ to start it in a separate browser window. Be sure to read the description and instructions below the applet before using it. This tool shows you a surface map of the total field anomaly, \\(B_t\\), after you specify the inclination, declination, and strength of the inducing field, the depth of the buried dipole, and the strength of the buried dipole's magnetic moment, **m** (which is proportional to its magnetic susceptibility and the inducing field strength). Recall from the introduction that the  induced magnetization in a material is related to its susceptibility via \\( \\vec{M} =\\kappa \\vec{H} \\) and the magnetic moment is a volume integral of the magnetic susceptibility. 

.. _here: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/magdipole/dipoleapp.html

Note that the applet also allows you to define a line across the surface map and observe a line profile of the anomaly. Also, there are options for displaying the surface map of the X, Y, or Z-component, or the vertical gradient, \\(B_g\\), as if the total field had been measured using two sensors 1 m apart.

The next figure shows three versions of the field induced in a buried object under a survey line, which is oriented towards magnetic north. The UBC-GIF dipole applet is also used to show the measured (i.e. anomalous) fields that would be recorded over the surface.


On the cross section, red arrows show Earth's field's direction, blue arrows show induced field vectors, and the sign of measurements can be determined by comparing the directions of these two fields at each location on the Earth's surface. On the map and profile image (which shows the dipole applet screen), pay particular attention to the amplitudes. Also note that the profile is approximately anti-symmetric, *not* at 45° latitude but at around 30° latitude.

.. raw:: html
    :file: buried_dipole2.html

The map and profile anomaly at the surface calculated by the UBC-GIF dipole applet is plotted to the right.
   