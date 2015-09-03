.. _magnetics_simple_vs_complex:

Working with complex structures
*****************************

In previous sections we learned what the anomalous magnetic field will be over a buried dipole (xxx link) and over extended bodies of uniform susceptibility (xxx link), and how those ideas apply to geologic structures that have a uniform susceptibility. In general however, the earth is complex and the rocks have variable susceptibility. How then do we determine the anomalous magnetic fields that arise from these geologic structures". The numerical procedure by which we simulate the data that would be obseved in a survey is often referred to as "forward modelling". In this context the term "model" refers to the 3D distribution of magnetic susceptibility in the earth.  There a numerous approaches but a common one is the following. Technically it is an integral equation solution but that is not particularly relevant here. The approach has three steps: 

1. Describe the subsurface as a finite collection of prismatic cells, each with uniform susceptibility.
2. The response of a single rectangular cell with constant susceptibility in an arbitrary magnetizing field can be calculated using expressions from the literature.
3. The principle of superposition holds.  At each location where a measurement is made, the responses from the individual cells are be added up to yield the total response.

The concept is illustrated in the following eight figures selected with the buttons.

.. raw:: html
    :file: simple_vs_complex.html

Here again are the data generated from the single block, the 5 blocks and the continuous Earth models: 

.. raw:: html
    :file: simple_vs_complex2.html

The following table gives access to model, mesh and data files associated with these 3 models (uniform earth, 1 block, 5 blocks) for use with UBC-GIF modeling and inversion code MAG3D. The MeshTools3D program is used to view 3D models. The filename extensions will be understandable to those familiar with use of these codes. See MAG3D in IAG's Chapter 10, "Sftwr & manuals" . 

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










