.. _seismic_apps:

Seismic apps
************

There are four seismic related apps used in this course. They are referenced throughout the seismic course material. They are collected here for reference:

1) `Seismic NMO App`_
2) `Seismic Reflection App`_
3) `Seismic Refraction App`_
4) `Seismic Vertical Resolution App`_
5) `Seismic General App`_

Apps 2-4 are Jupyter notebooks, which can be run live on the web using the binders platform. Each notebook has self-contained instructions. 

We also link to a `seismic refraction app <https://row1.ca/seismic-layers>`__. It demonstrates seismic ray paths in a three layered earth. A snapshot of the app is shown below. It consists of two interactive plots, one showing direct, refracted, and reflected ray paths and the other showing travel-time vs receiver offest for those rays. The app allows you to explore how the different types of seismic ray paths depend on the structure (layer depth) and material properties (layer velocities) of the earth. 

.. figure:: ./images/3pt-seismic-refrac-app-snapshot.png
   	:align: center
	:scale: 60 %

Instructions for using the app are as follows: You can toggle the visibility of each ray using buttons on the left hand side of the page. Adjust the velocity of each layer using the controls on the right of the page and adjust the depth of each layer by dragging the horizontal sliders on the ray path plot. You can adjust the receiver offset by dragging the vertical slider on either plot. Finally, you can use the horizontal slider on the traveltime plot to explore how the rays progress as time advances. On the top plot, the path of each ray up to the time specified by the time slider are shown as thick solid lines. Thin dashed lines show how the rays will continue to propagate after the specified time. The traveltime vs offset plots for the refracted rays will be dashed for offsets at which the rays will arrive after the direct wave.


.. _Seismic NMO App: https://mybinder.org/v2/gh/geoscixyz/gpgLabs/main?filepath=notebooks%2Fseismic%2FSeis_NMO.ipynb
.. _Seismic Reflection App: https://mybinder.org/v2/gh/geoscixyz/gpgLabs/main?filepath=notebooks%2Fseismic%2FSeis_Reflection.ipynb
.. _Seismic Refraction App: https://mybinder.org/v2/gh/geoscixyz/gpgLabs/main?filepath=notebooks%2Fseismic%2FSeis_Refraction.ipynb
.. _Seismic Vertical Resolution App: https://mybinder.org/v2/gh/geoscixyz/gpgLabs/main?filepath=notebooks%2Fseismic%2FSeis_VerticalResolution.ipynb
.. _Seismic General App: https://mybinder.org/v2/gh/geoscixyz/gpgLabs/main?filepath=notebooks%2Fseismic%2FSeismicApplet.ipynb
