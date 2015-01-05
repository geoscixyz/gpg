.. _magnetics_simple_vs_complex:

Simple and complex structures
*****************************

We learned above what the anomalous magnetic field will be over a buried dipole and over extended bodies of uniform susceptibility, and how those ideas apply to geologic structures (again, assuming uniform susceptibility). How then do we anticipate the fields due to more general geologic models of the earth? In "geophysical" terminology, the question is "how do we forward model the response to an arbitrary distribution of susceptibility?" Here is one approach that has become popular; there are 3 steps:

1. Describe the subsurface as a finite collection of cells, each with uniform susceptibility.
2. Recognize that the response to a single rectangular cell with constant susceptibility in an arbitrary magnetizing field can be calculated relatively easily using expressions from the literature.
3. At each location where a measurement is made above our model of the earth, the responses from all the individual cells must be added up. The result will be the superposition of all those little responses.

The concept is illustrated in the following eight figures selected with the buttons. (Such calculations are introduced in section 10 and details are given in section 11.)

.. raw:: html
    :file: simple_vs_complex.html

Here again are the data generated from the single block, the 5 blocks and the continuous Earth models: 

.. raw:: html
    :file: simple_vs_complex2.html

The following table gives access to model, mesh and data files associated with these 3 models (uniform earth, 1 block, 5 blocks) for use with UBC-GIF modelling and inversion code MAG3D. The MeshTools3D program is used to view 3D models. The filename extensions will be understandable to those familiar with use of these codes. See MAG3D in IAG's Chapter 10, "Sftwr & manuals" . 

+-------------------+----------------+-------------------+---------------+---------------+
|  **Model**        | **model file** | **location file** | **mesh file** | **data file** |
+===================+================+===================+===============+===============+
| Single block:     | `block_sus`_   | `block_sus_loc`_  | `block_msh`_  | `block_mag`_  |       
+-------------------+----------------+-------------------+---------------+---------------+
| Five block:       | `block_5_sus`_ |`block_5_sus_loc`_ | `block_msh`_  |`block_5_mag`_ | 
+-------------------+----------------+-------------------+---------------+---------------+
| Continuous earth: | `v_sus`_       |  --------------   | `v_msh`_      | `v_mag`_      |
+-------------------+----------------+-------------------+---------------+---------------+

.. _block_sus: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/block.sus
.. _block_sus_loc: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/block.sus_loc
.. _block_msh: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/block.msh
.. _block_mag: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/block.mag
.. _block_5_sus: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/block-5.sus
.. _block_5_sus_loc: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/block-5.sus_loc
.. _block_msh: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/block.msh
.. _block_5_mag: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/block-5.mag
.. _v_sus: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/v.mag
.. _v_msh: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/v.msh
.. _v_mag: http://www.eos.ubc.ca/courses/eosc350/content/methods/meth_3/assets/datmod-files/v.mag










