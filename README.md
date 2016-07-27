# VMOF
A general forcefield for accurate phonon properties of metal-organic frameworks

The following files contain the data used in the following publication:

"A general forcefield for accurate phonon properties of metal-organic frameworks"

Jessica K. Bristow, Jonathan M. Skelton, Katrine L. Svane, Aron Walsh and Julian D. Gale
Paper under review

The files are structured in 3 parent directories:

VMOF_library file
        -contains all parameters of the VMOF forcefield in lib.lib
        -azulene.pdf labels carbon atoms on azuelene ligands, which correspond to labels identified in the lib file


QHA-DOS-IR
        -directory contains all appropriate data for DOS,IR and QHA calculations for both density functional theory calculations (DFT) and VMOF forcefield calculations (VMOF)
        -subdirectories are formatted as follows:

                                QHA
                        DFT     DOS
                                IR
        NAME_OF_MOF

                                QHA
                        FF      DOS
                                IR

        INCAR_FILES
        -additional subdirectory that contains the INCAR files used for the DOS, IR and QHA approximation calculations using VASP (Kresse, G., and J. Furthmüller. "Software VASP, vienna (1999)." Phys. Rev. B 54.11 (1996): 169.). Note that the for the DOS and QHA this INCAR was used for each generated displacement.

STRUCTURE_FILES
        -directory contains all POSCAR converged structure files under the name of the appropriate MOF