# Test impropers using benzene and o-xylene
This directory tests whether impropers are properly (heh) implemented by looking at benzene and o-xylene.

## Manifest
- `tleap_tools.py` from `openforcefield/utilities/SMIRNOFF_vs_frosst/`, which provides functionality for parameterizing using AMBER
- test_impropers.ipynb for comparing energies of impropers; tests on several molecules including one which uses steric strain to make the improper energy for a ring system be nontrivial.
- `parm_Frosst.frcmod` from `openforcefield/utilities/SMIRNOFF_vs_frosst/parm_at_Frosst.tgz`
- `smirnoff99Frosst_modified.offxml`: `openforcefield/utilities/convert_frosst/smirnoff99Frosst.offxml` but modified to make a CA-CA-CA specific angle parameter (unimportant since it is intra-ring, but important for energy) match AMBER
- Miscellaneous molecule files - mol2 files and AMBER format coordinate/parameter files generated by the ipython notebook
