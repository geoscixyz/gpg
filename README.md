GPG: Geophysics for Practicing Geoscientists
============================================

A learning resource for applied geophysics.

Originally created by Francis H.M. Jones and Douglas W. Oldenburg.

http://gpg.geosci.xyz


For Developers:
---------------

Here are a couple resources on sphinx and reStructured Text:

- http://sphinx-doc.org/markup/
- http://docutils.sourceforge.net/docs/ref/rst/restructuredtext.html 

**Best practices for attribution:**

- https://wiki.creativecommons.org/wiki/Best_practices_for_attribution

**Tips:**

Example of how to reference a Figure.

- Insert and name your Figure
```
 .. figure:: ./ExampleImage.png
	:align: center
	:scale: 110% 
	:name: ExampleImage

	Figure Caption.
```

- Reference the Figure
```
An example image is shown in :numref:`Positive_magnetic_pole`.
```	
Output: An example image is shown in Fig. #.	
