.. _foundations_seeing_underground_example:

Mineral exploration example
***************************

Large quantities of magnetic field measurements are routinely gathered over mineral and petroleum exploration prospects using airborne techniques. Resulting magnetic anomaly maps can provide information about geological trends because rocks containing higher proportions of the mineral magnetite have a higher magnetic susceptibility, and will affect the local behavior of the earth's magnetic field. Data can also be inverted to reveal three dimensional features of the earth. 

Regional and local magnetic surveys
===================================

Figure 3 (supplied courtesy of Placer Dome Exploration) provides an example of regional information from an area surrounding the Mt Milligan copper porphyry deposit, located in central British Columbia. Geological trends can be discerned using this type of data, however, exploration for a specific deposit requires more detailed information about local subsurface distributions of rock types. Figure 3b shows anomalous strengths of the earth's magnetic field for a small region of one ore body. Evidently there is a range of different rock types below the surface, but details of location, depth and magnetic susceptibility are difficult to determine directly using conventional methods. 

 .. raw:: html
    :file: ../figure3.html

Inversion to obtain 3D details 
==============================

The goal of inverting this data set was to produce detailed 3D models of magnetic susceptibility to help geologists develop a more complete understanding of the rocks associated with the ore deposit. The first step was to reduce the dense data set from the small region (Figure 3a) to a more manageable 1,029 evenly spaced data points and to divide the model region into 169,000 cells. Then a desirable model type was chosen. In this instance, the process was set up with two criteria; namely to find a model that was (i) as close as possible to a uniform earth with zero susceptibility, and (ii) included structure that was smooth in all three spatial dimensions. 

In addition, the numerical procedure for finding plausible subsurface models of susceptibility was constrained so that data predicted from the model would match observed field measurements to a degree specified by assuming a noise level (on measurements) of 5%. The resulting model was a 3D volume represented by the 169,000 cells, each with a magnetic susceptibility recovered by the inversion. 

Visualizing results
===================

There are several ways to usefully present volumetric information of this kind. Contour plots of horizontal or vertical slices through the volume, as shown in Figure 4, provide quantitative details at any required location. Alternatively, for a more general impression of the model, a 3D isosurfacee image can be created. This is shown in Figure 5, which suggests there is a well-defined volume of magnetically susceptible rocks associated with this deposit. This model correlates well with one of the known principal local rock units (MBX monsonite stock) and with locations of mineralization. 

.. figure:: ../images/fig2-s.jpg
	:align: right
	:scale: 90 %

	Figure 4: The model of magnetic susceptibiility recovered by the inversion of ground-based magnetic data is illustrated by plotting slices from the volume under the survey area. The left panel is a horizontal slice at 80m depth; the right panels are three vertical slices taken along lines at 9600, 9500, and 9400 metres north. Gray lines indicate the slice locations.

Corroboration with independent geophysical results
==================================================

Few geophysical surveys are used alone with no other independent information. At Mt Milligan many types geophysical surveys were performed on the ground, from airborne platforms, and from within boreholes. For example, a similar inversion procedure was used to interpret DC electrical measurements gathered over the same area. The 3D isosurfacee image of Figure 6 shows a model of the distribution of chargeability (the capacity for material to hold an electrical charge), a physical property related essentially to metal or clay content and grain size. The apparent anti-correlation between magnetic susceptibility and chargeability at Mt Milligan is evident only after careful inversion of two unrelated geophysical data sets. This example illustrates that conducting inversions on multiple types of data can provide an enhanced understanding of the surveyed region; in this case it provides insight about subsequent alteration of the rocks that occurred after the initial formation of the mineral deposit.

 .. raw:: html
    :file: ../animated_fig1.html


**Figure 5:** The same magnetic susceptibility distribution model shown in the previous figure is plotted here as a 3D isosurface of constant susceptibility. Any surface between zero and the maximum susceptibility recovered could be chosen for the plot. The best choice for illustrating geologically relevant features depends upon estimating the true susceptibility of rocks, perhaps from borehole or outcropping samples. 

 .. raw:: html
    :file: ../animated_fig2.html

 **Figure 6:** An isosurface plot of chargeability, which is usually related to the presence of sulphide ores, graphite, or clay minerals. The chargeability model was obtained by carrying out a 3D inversion of induced polarization data collected along parallel survey lines over the deposit region. Comparison with the 3D model of magnetic susceptibility shows that low chargeability is correlated with high susceptibility. Detailed correlation of the two inversion results provided information that contributed to an enhanced understanding of how the ore body was deposited. 

