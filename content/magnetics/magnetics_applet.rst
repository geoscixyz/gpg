.. _magnetics_applet:

Magnetic dipole applet
----------------------

Purpose
=======

The objective is to learn about the magnetic field observed at the ground's surface, caused by a small buried dipolar magnet. In geophysics, this simulates the observed anomaly over a buried susceptible sphere that is magnetized by the Earth's magnetic field. By clicking below binder badge, you can run this app!

.. image:: https://mybinder.org/badge.svg
    :target: https://mybinder.org/v2/gh/geoscixyz/gpgLabs/master?filepath=Notebooks%2FMagneticDipoleApplet.ipynb
    :align: center

.. figure:: ./images/magnetic_dipole_applet.png
    :align: center
    :figwidth: 100%



What is shown
=============

- **The colour map** shows the strength of the chosen parameter (Bt, Bx, By, Bz, or Bg) as a function of position.

- Imagine doing a two dimensional survey over a susceptible sphere that has been magentized by the Earth's magnetic field specified by inclination and declination.  "Measurement" location is the centre of each coloured box. This is a simple (but easily programmable) alternative to generating a smooth contour map.

- The anomaly depends upon magnetic latitude, direction of the inducing (Earth's) field, the depth of the buried dipole, and the magnetic moment of the buried dipole.


Important Notes
===============

- **Inclination (I)** and **declination (D)** describe the orientation of the Earth's ambient field at the centre of the survey area. Positive inclination implies you are in the northern hemisphere, and positive declination implies that magnetic north is to the east of geographic north.

- The **"length"** adjuster changes the size of the square survey area. The default of 72 means the survey square is 72 metres on a side.

- The **"data spacing"** adjuster changes the distance between measurements. The default of 1 means measurements were acquired over the survey square on a 2-metre grid. In other words, "data spacing = 2" means each coloured box is 2 m square.

- The **"depth"** adjuster changes the depth (in metres) to the centre of the buried dipole.

- The **"magnetic moment (M)"** adjuster changes the strength of the induced field. Units are Am2.  This is related to the strength of the inducing field, the susceptibility of the buried sphere, and the volume of susceptible material.
- **Bt, Bg, Bx, By, Bz** are Total field, X-component (positive northwards), Y-component (positive eastwards), and Z-component (positive down) of the anomaly field respectively.

- Checking the **fixed scale** button fixes the colour scale so that the end points of the colour scale are minimum and maximum values for the current data set.

- You can generate a **profile** along either "East" or "North" direction

- Check **half width** to see the half width of the anomaly. Anomaly width is noted on the botton of the graph.

- Measurements are taken 1m above the surface.

- For gradient data (**Bg**), measurements are taken at 1m and 2m
