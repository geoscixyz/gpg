.. _magnetics_buried_dipole:

Response over a buried magnetic dipole
**************************************

Fields due to buried magnetic dipoles 
=====================================

.. no_field.gif
.. inducing_field.gif
.. magnetic_anomaly.gif
.. measurements.gif

To learn about magnetic field data that will be recorded at Earth's surface over buried susceptible material, start by considering a small susceptible object that is magnetized by the Earth's field. "Small" means that all of the object's dimensions are several times smaller than the depth to its center. If the object is small, its induced field can be approximated as if the object were a "magnetic dipole" -- that is, a little bar magnet with strength and direction caused by the inducing field. Understanding this simple situation is crucial because all real scenarios can be thought of as a combination (superposition) of many dipoles (see the "Buried structures" section). The sign convention will be that horizontal fields are positive if they point in the \\(\\hat{x}\\) direction and vertical fields are positive if they point down.

The figures below illustrate the problem. The pattern recorded at the surface arises by measuring the field strength everywhere on the surface, removing the Earth's field, and then plotting the results as a contour map of anomalous field strength. In the third figure, regions of blue anomalous field are "negative" because at those surface locations, the **anomalous** field crossing that surface points in the opposite direction for Earth's field.

.. raw:: html

    <tbody>
        <tr>
            <td>
                <p align="center">
                    <font size="-1">
                        <img width="200" height="188" name="burieddipole" src="../../_images/no_field.gif"></img>
                    </font>
                </p>
                <form action="" method="post" name="form2">
                    <input type="radio" onclick="MM_swapImage('burieddipole','','../../_images/no_field.gif',1)" checked="checked" value="radiobutton" name="radiobutton"></input>
                    <b>

                        1.

                    </b>

                     No incident magnetic field. 

                    <br></br>
                    <input type="radio" onclick="MM_swapImage('burieddipole','','../../_images/inducing_field.gif',1)" value="radiobutton" name="radiobutton"></input>
                    <b>

                        2.

                    </b>

                    Earth's field causes material to become magnetized. What total field pattern (anomaly) will be measured at all points on the surface above the buried feature?

                    <br></br>
                    <input type="radio" onclick="MM_swapImage('burieddipole','','../../_images/magnetic_anomaly.gif',1)" value="radiobutton" name="radiobutton"></input>
                    <b>

                        3.

                    </b>

                     The answer is found by determining the amount of the anomalous field that is in line with the incident field's direction. Plotting these measurements produces a map of this magnetic anomaly.

                    <br></br>
                    <input type="radio" value="radiobutton" onclick="MM_swapImage('burieddipole','','../../_images/measurements.gif',1)" name="radiobutton"></input>
                    <strong>

                        4.

                    </strong>

                      Often measurements are made along lines and the anomaly is plotted as a graph. 

                </form>
            </td>
        </tr>
    </tbody>

    <p>
    </p>



Magnetic dipoles: a Java applet
-------------------------------


As noted above, a real buried feature will look like a magnetic dipole if its physical dimensions are much smaller than the depth to the feature's centre.

The response that will be measured at points on a surface overlying a buried magnetic dipole can be explored using the UBC-GIF magnetic dipole Java applet; click here_ to start it in a separate browser window. Be sure to read the description and instructions below the applet before using it. This tool shows you a surface map of the total field anomaly, \\(B_t\\), after you specify the inclination, declination, and strength of the inducing field, the depth of the buried dipole, and the strength of the buried dipole's magnetic moment, **m** (which is proportional to its magnetic susceptibility and the inducing field strength). Recall from the introduction that the strength of induced magnetization in a material is related to its susceptibility via \\( \\textbf{m} =\\kappa \\textbf{H} \\). 

.. _here: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/magdipole/dipoleapp.html

Note that the applet also allows you to define a line across the surface map in order to see the corresponding line profile anomaly. Also, there are options for displaying the surface map of the X, Y, or Z-component, or the vertical gradient, \\(B_g\\), as if the total field had been measured using two sensors 1 m apart.

The next figure shows three versions of the field induced in a buried object under a survey line, which is oriented towards magnetic north. The UBC-GIF dipole applet is also used to show the measured (i.e. anomalous) fields that would be recorded over the surface.


On the cross section, red arrows show Earth's field's direction, blue arrows show induced field vectors, and the sign of measurements can be determined by comparing the directions of these two fields at each location on the Earth's surface. On the map and profile image (which shows the dipole applet screen), pay particular attention to the amplitudes. Also note that the profile is approximately anti-symmetric, *not* at 45° latitude but at around 30° latitude.
