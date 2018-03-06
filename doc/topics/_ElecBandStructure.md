---
authors: XG
description: ElecBandStructure Abinit topic
---
<!--
This file is automatically generated by mksite.py. All changes will be lost.
Change the input yaml files or the python code
-->

This page gives hints on how to generate the electronic band structure related topics with the ABINIT package.

## Introduction

The eigenenergies along a set of segments can be computed (non-self-consistent
calculations [[iscf]]=-2) using a negative value of [[kptopt]], with
[[kptbounds]] defining the end points of the segments, and [[ndivsm]] (or
[[ndivk]]) defining the sampling.

A band structure can even be represented using weights proportional to the
orbital content (so-called "Fat Bands"), in case of PAW calculation, see
[[pawfatbnd]], and related variables.

Different interpolation schemes for the band energies can be defined thanks to
[[einterp]]. The Wannier interpolation is also available through the use of
the [[lesson:wannier90]] post-processor.

The band structure from a supercell calculation can be unfolded to the (large)
Brillouin zone of the (small) primitive cell thanks to the [[help:fold2bloch]]
post-processor. See the related [[topic:Unfolding]].

Different plotting postprocessors exist to produce graphical representations
of electronic band structures from ABINIT. The most powerful is based on
[[topic:Abipy]]. Simpler tools also exist, and can be found in
~abinit/scripts/post_processing, e.g. AbinitBandStructureMaker.py,
plot_bandstructure.py or abinit_eignc_to_bandstructure.py.



## Related Input Variables

{{ related_variables }}

## Selected Input Files

{{ selected_input_files }}
