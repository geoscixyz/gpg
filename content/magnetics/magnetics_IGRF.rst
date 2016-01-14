.. _magnetics_IGRF:

The IGRF
********

Here are a few remarks about the IGRF or International Geomagnetic Reference Field.

The IGRF is a mathematical model that describes the field and its secular
changes as a spherical harmonic expansion. It is updated every five years, and
**later** versions may re-define the field at **earlier** times. This is
important to remember if you are comparing old maps to new ones. The IGRF is a
product of the International Association of Geomagnetism and Aeronomy (IAGA_),
and the original version was defined in 1968.

.. _IAGA: http://www.ngdc.noaa.gov/IAGA/vmod/

Every five years, the IAGA issues a contemporary main field model that
predicts the field for the next five years. These models have names that are
prefixed with "IGRF." Each new model updates the model that was used to
predict the previous five (or more) years. Updated models are called **DGRF**
for **Definitive Geomagnetic Reference Field**. Major updates since 1980 use
data from MAGSAT, consisting of measurements of vector components and total
intensity of the geomagnetic field between 350 and 560 km altitude.

To correct data sets which had older versions of reference fields removed, add
:math:`(F_0 - F_n)` to each data point, where the two parameters are total
intensity values computed from the old and new reference fields respectively.
See Peddie N.W. 1982, 1983, and 1986 for details. Charts of many types are
available on-line, as downloadable postscript files, and for sale (less than
$5.00 each) from the USGS, NOAA, GSC, and just about any other government
geoscience agency. For example, you could use either the NOAA Geomagnetism
page_, or the Canadian National Geomagnetism Program's homepage_.

.. _page: http://www.ngdc.noaa.gov/ngdc.html
.. _homepage: http://www.geomag.nrcan.gc.ca/index-eng.php

References:

* Peddie, N. W., 1986, Report on International Geomagnetic Reference Field revision 1985 by IAGA Division I Working Group 1: *Geophysics*, 51, no. 4, 1020-1023.
* Peddie, N. W., 1983, International Geomagnetic Reference Field - its evolution and the difference in total field intensity between new and old models for 1965-1980 (short note): *Geophysics*, 48, no. 12, 1691-1696.
* Peddie, N. W., 1982, Report on International Geomagnetic Reference Field 1980 by IAGA Division I Working Group 1: *Geophysics*, 47, no. 5, 841-842.
