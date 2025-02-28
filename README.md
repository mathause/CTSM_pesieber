# CTSM for CCLM2 (branch release-clm5.0) 

Clone the branch:  
git clone -b release-clm5.0 https://github.com/pesieber/CTSM.git clm5.0  
cd clm5.0  
./manage_externals/checkout_externals  

Note: you may need a fresh clone if you have ran checkout_externals on the main branch before
(e.g. if you get errors about non-existing xml variable names, this is why...)

Install oasis (required for coupling):   
spack install oasis@master%gcc@9.3.0 fflags="-ffree-line-length-512"

Copy CCLM2_inputdata to your $SCRATCH (2 alternatives, depending on access)  
cp -r /project/sm61/shared/CCLM2_inputdata $SCRATCH/.  
cp -r /scratch/snx3000/psieber/CCLM2_inputdata $SCRATCH/.  

## CTSM

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3739617.svg)](https://doi.org/10.5281/zenodo.3739617)

## Overview and resources

The Community Terrestrial Systems Model.

This includes the Community Land Model (CLM5.0 and CLM4.5) of the Community Earth System Model.

For documentation, quick start, diagnostics, model output and
references, see

http://www.cesm.ucar.edu/models/cesm2.0/land/

and

https://escomp.github.io/ctsm-docs/

For help with how to work with CTSM in git, see

https://github.com/ESCOMP/CTSM/wiki/Quick-start-to-CTSM-development-with-git

and

https://github.com/ESCOMP/ctsm/wiki/Recommended-git-setup

For support with model use, troubleshooting, etc., please use the CTSM forum (or other
appropriate forum) here:

https://xenforo.cgd.ucar.edu/cesm/

To get updates on CTSM tags and important notes on CTSM developments
join our low traffic email list:

https://groups.google.com/a/ucar.edu/forum/#!forum/ctsm-dev

(Send email to ctsm-software@ucar.edu if you have problems with any of this)

## CTSM code management team

CTSM code management is provided primarily by:

Software engineering team:
- [Erik Kluzek](https://github.com/ekluzek)
- [Bill Sacks](https://github.com/billsacks)
- [Mariana Vertenstein](https://github.com/mvertens)
- [Negin Sobhani](https://github.com/negin513)
- [Sam Levis](https://github.com/slevisconsulting)

Science team:
- [Dave Lawrence](https://github.com/dlawrenncar)
- [Will Wieder](https://github.com/wwieder)
- [Danica Lombardozzi](https://github.com/danicalombardozzi)
- [Keith Oleson](https://github.com/olyson)
- [Sean Swenson](https://github.com/swensosc)
- [Mike Barlage](https://github.com/barlage)
- [Rosie Fisher](https://github.com/rosiealice)
- [Peter Lawrence](https://github.com/lawrencepj1)
