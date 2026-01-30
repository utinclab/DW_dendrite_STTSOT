# DW_dendrite_STTSOT
Multi-input DW dendrite, PMA SOT+STT driven + DMI, base current density uses STT portion of total current density with 1:3.1 STT to SOT current ratio. Current code is configured for MgO/CoFeB(1.2)/Pt(7) with bottom layer HM.

The intended use is for calculating SOT fields for custom current density mask OVFs in MuMax.

STT current densities were calculated using FEM in Wolfram Mathematica. Total current densities are calculated using equivelant parallel resistance from CoFeB/Pt and scaled down to equivelant STT current density using Kumar et al. "Large interfacial contribution to ultrafast THz emission by inverse spin Hall effect in CoFeB/Ta heterostructure" (2022), eq. (1). STT current density is then scaled up in MuMax code for equivelant SOT current density.
