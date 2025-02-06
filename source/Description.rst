Description
===========

Void catalogs: Gigantes includes 15,000 VIDE fiducial cosmology void catalogs, as well as over 9,000 catalogs in non-fiducial cosmologies, spanning various values of the following cosmological parameters :math:`\Omega_{\rm m}`, :math:`\Omega_{\rm b}`, :math:`h`, :math:`n_s`, :math:`\sigma_8`, :math:`M_\nu`, and fully leveraging the Quijote simulation suite, which covers redshifts z = 0.0, 0.5, 1.0, and 2.0 in real and redshift space.

Void finder: The void finding relies on the popular public void finder VIDE (`Sutter et al. 2015b <https://arxiv.org/abs/1406.1191>`__), arguably the most used void finder, as testified by its use in a plethora of papers performing both simulation-based theoretical modelling and data analysis from modern surveys (`Papers using VIDE <http://bitbucket.org/cosmicvoids/vide_public/wiki/Papers%20Using%20VIDE>`__).

Information about VIDE, used to build Gigantes can be found here : `VIDE Wiki <https://bitbucket.org/cosmicvoids/vide_public/wiki/Home>`__ .

Provided statistics:
Void center position (x,y,z---this is the volume-weighted barycenter, a.k.a. macrocenter), Void effective radius (Mpc/h), Void ID, void volume, redshift, ellipticity, density contrast, number of children (sub-voids), central density ...

The video below shows an example of a Gigantes void together with the positions of the galaxies used to identify it. Credit: Wang et al. 2022, see `ArXiv <https://arxiv.org/abs/2212.06860>`__ and `ApJ <https://iopscience.iop.org/article/10.3847/1538-4357/aceaf6>`__ ; (for videos of more voids see : `here <https://www.youtube.com/embed/nJyXYPPJaok>`__).

.. image:: Wang.gif
   :width: 69 %

**Note**: The Gigantes catalogs are created with the VIDE repository. In the VIDE repository, on the 2024-03-27, a minor bug has been fixed for the ellipticity file, where eigenvectors were printed in transposed order (see : `here <https://bitbucket.org/cosmicvoids/vide_public/commits/16301287def7959ee9ba6fb10e99035adf5568f9>`__). Therefore for catalogs created before 2024-03-27 (this includes the Gigantes catalogs) the eigenvectors are printed in transposed order. This does *not* impact the computed ellipticities, so it would only affect analyses directly using the eigenvectors values. 
