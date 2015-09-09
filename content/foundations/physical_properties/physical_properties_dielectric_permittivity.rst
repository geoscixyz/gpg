.. _physical_properties_dielectric_permittivity:

Dielectric permittivity
***********************

**Dielectric permittivity  \\((\\epsilon)\\)**: This physical property quantifies how easily material becomes polarized in the presence of an electric field. The permittivity of free space is \\(\\epsilon_0 = 8.8541878176 10^{-12} F/m\\), a "Farad" (F) is the unit of capacitance, named after Michael Faraday. If free space did not have finite permittivity, electromagnetic waves (light, radio, etc) could not propagate in free space.

**Relative dielectric permittivity \\((\\epsilon_R)\\)**: Relative dielectric permittivity is a ratio: since dielectric permittivity \\(\\epsilon = \\epsilon_R \\epsilon_0\\), relative dielectric permittivity \\(\\epsilon_R = \\epsilon / \\epsilon_0\\).

 
Relative dielectric permittivity is the parameter usually referred to in GPR work. It is 1 (one) for free space or air, and 80 for water. Because it is a number that compares true value to free space value, it has no units.

Dielectric permittivity is in fact a complex value, often written \\( \\epsilon_R = \\epsilon_R^{\\prime} - i\\epsilon_R^{\\prime\\prime}\\). It can be considered as a measure of the extent to which charge distribution can be distorted or polarized by an applied electric field.


The so-called "real" part, \\(\\epsilon_r^{\\prime}\\), is the *relative dielectric constant*\\( \\), often introduced in electronics or physics courses in the context of capacitors. It is a storage component measured as capacitance per unit length. (Capacitance is "the amount of charge a material can hold" for a given applied voltage.) At different frequencies, polarization occurs at different scales: at very high frequencies, only subatomic particles can be polarized. At GPR frequencies, the reorientation of dipolar molecules is the largest contribution, hence water's importance in determining the velocity of EM waves in a material. Note that \\(\\epsilon_R = 80\\) for water, whereas \\(\\epsilon_R < 10\\) for most other common materials.

 .. figure:: ../../GPR/images/dielectric_responses.jpg
	:align: center
	:scale: 100 %

	A dielectric permittivity spectrum over a wide range of frequencies, for real (top curve) and "imaginary" (bottom curve) components. Borrowed from `Wikipedia Dielectric Permittivity Article`_.

The so-called "imaginary" part, \\(\\epsilon_r^{\\prime\\prime}\\),  is a loss component that generally indicates how much energy is dissipated at the transition from one polarization mechanism to another. The behaviour of both is shown in the figure. Values are relatively constant for GPR frequencies of \\(10^6\\) through \\(10^9\\) , ensuring that wave behaviour is not dispersive; i.e. all frequency components of a broad band signal travel at the same speed.

The dielectric permittivity of most geological materials is closely dependent upon the amount of water (free or otherwise) in the material. Values of \\(\\epsilon_R\\) for geologic materials range from 1 to 80, as seen in the table above.

.. _Wikipedia Dielectric Permittivity Article: https://en.wikipedia.org/wiki/Permittivity
