.. _foundations_model_types:


Mathematical representations of the Earth
*****************************************

Earth materials and buried structures are complicated. Yet we need to be able
to represent these mathematically so that responses from geophysical surveys
can be numerically simulated. Ultimately, our goal is to find a mathematical
representation of the earth, such that when simulated responses are generated,
then the simulated responses are in agreement with the observations. The
process of carrying this out is referred to as "inversion".

There are many ways to parameterize the earth mathematically. We can have
discrete objects with boundaries or we can divide the earth into "cells", each
of which has constant value of a physical property. The earth is 3-dimensional
and to accommodate this the cells can be: layers, 2D cylinders, 3D prisms.

We generically refer to the parameterized earth as a "model". In the inverse
problem we attempt to find values for each element in the model. In the
application step, these values are interpreted to help solve the problem of
interest. This means we need to know the relationship between values of a
physical property and rock type, alteration, buried object etc.

Below we provide some examples of commonly used earth parameterizations.

.. sidebar:: Uniform halfspace

    .. figure:: ./images/modelytpes_0d.gif
    	:align: center

1. **A "uniform halfspace"** means the earth beneath the surface has the same
   physical property value. No topography is permitted and the region above the
   surface is assumed to be air (sometimes called "free space"). In a "uniform
   wholespace" the entire volume has the same physical property value. This is
   useful in borehole studies.

**Typical geoscience tasks:** Mapping shallow apparent conductivity for site
characterization, contaminated ground, or other shallow investigation
projects

.. sidebar:: Buried objects

    .. figure:: ./images/modelytpes_0obj.gif
    	:align: center

2. When **buried objects** are the focus, the earth is usually considered to
   be uniform all around the object. The object itself may be represented with a
   more or less complicated set of parameters.

**Typical geoscience tasks:** Finding or characterizing buried utilities, tanks,
UXOs, or other objects.

.. sidebar:: 1D (layered) models

    .. figure:: ./images/1d-interp.gif
    	:align: center

3. In a **1D model**, the physical property is assumed to vary only in one
   direction (usually depth). The earth is commonly divided into layers (cells),
   each of which has a constant value of physical property. Surveys that are
   designed to yield 1D results are often called soundings. Results are often
   displayed in a way that resembles a drill core.

**Typical geoscience tasks:** Layered Earth problems, such as hydrology,
overburden thickness, clay layer detection, etc.

.. sidebar:: 2D models

    .. figure:: ./images/2d-interp.gif
    	:align: center
	
4. In a **2D model**, the physical property is assumed to vary in two
   directions, usually depth and the direction parallel to a survey line. Surveys
   that yield 2D results are interpreted as cross sections. The assumption is
   that the structures extend without change either side of the survey line.

**Typical geoscience tasks:** Detailed geologic structure characterization such
as defining ore bodies or other geologic features

.. sidebar:: 3D models

    .. figure:: ./images/modelytpes_3d.gif
    	:align: center

5. In a **3D model**, the subsurface is divided into prismatic cells. Each
   cell is assumed to have a constant physical property. This is the most general
   parameterization and 3D inversion is computatinally intensive.

**Typical geoscience tasks:** Detailed geologic structure characterization such
as defining ore bodies or other geologic features

For 2D and 3D models, structures within the earth may be considered as simple
geometric shapes, or as continuously varying distributions of a physical
property. Simple shapes (spheres, blocks, cylinders, etc.) are easy to
describe - they require few parameters. For example a cylinder is fully
described by a fixed radius, depth to top, length and density. For
continuously varying physical property distributions, the Earth's structure
must be described as a *function* with the physical property dependent upon
position. Representing this mathematically requires that the earth be
represented with many cells. In the next section, we expand upon the
distinctions between discrete simple geometric shapes and continuously varying
models.
