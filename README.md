# VMOF

A general forcefield for accurate phonon properties of metal-organic frameworks. It is a major revision of our previous [BTW](https://github.com/WMD-group/BTW-FF) project. The following files contain the data used in: *"A general forcefield for accurate phonon properties of metal-organic frameworks"*  Jessica K. Bristow, Jonathan M. Skelton, Katrine L. Svane, Aron Walsh and Julian D. Gale (Under Review, 2016).

The files are structured in 3 parent directories:

**VMOF_library file**
* contains all parameters of the VMOF forcefield in `vmof.lib` formatted for [GULP](http://nanochemistry.curtin.edu.au/gulp/)
* `azulene.pdf` labels carbon atoms on azuelene ligands, which correspond to labels identified in the lib file


**QHA-DOS-IR**
* directory contains all appropriate data for DOS, IR and QHA calculations for both density functional theory calculations (DFT) and VMOF forcefield calculations (FF)
* subdirectories are formatted as follows:

                                QHA
                        DFT     DOS
                                IR
        NAME_OF_MOF

                                QHA
                        FF      DOS
                                IR

        INCAR_FILES
* `INCAR_FILES` contains the INCAR files used for the DOS, IR and QHA approximation calculations using [VASP](https://www.vasp.at). Note that the for the DOS and QHA this INCAR was used for each generated displacement

**STRUCTURE_FILES**
* directory contains all POSCAR converged structure files under the name of the appropriate MOF
