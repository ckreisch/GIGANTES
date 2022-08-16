Organization
============

The GIGANTES data is organized in different folders:

[Details about folder]


Each void catalog has the following structure (VIDE void catalog structure):
- sample_info.txt: Small text file which lists some basic info of the sample
- zobov_slice_[sample_name].dat: Binary file with the galaxy positions, RA, Dec, redshift, and unique catalog ID. Note that this file contains all particles in the particular sample, not just void particles.
- voidDesc_[all,central]_[sample_name].out: ASCII file with void indices and basic void properties in ZOBOV-normalized units.
- voidZone_[sample_name].out: Binary file which links voids to zones.
- voidPart_[sample_name].out: Binary file which links zones to particles.
- vol_[sample_name].out: Binary file with particle local volumes

In addition, VIDE provides the following derived void information:

- centers_[all, central]_[sample_name].txt: ASCII file with void centers, volume, effective radius, void ID, density contrast, etc.
- sky_positions_[all, central]_[sample_name].txt: ASCII file with void RA, dec, effective radius, and void ID
- shapes_[all, central]_[sample_name].txt: ASCII file with best-fit eigenvalues and eigenvectors for each void, in same coordinate system as x,y,z values in centers file

In addition to the [all,central] version of each file above, there are four versions of each catalog:

- no prefix: only parent voids, density cut applied (default catalog)
- untrimmed: all voids in hierarchy, density cut not applied
- untrimmed_dencut: all voids in hierarchy, density cut applied [deprecated]
- trimmed_nodencut: only parent voids, density cut not applied [deprecated]
