# Ion beam simulations with IBSIMU

## Build steps

1. Clone the repository recursively to include the ibsimu git submodule.
1. Follow the INSTALL instruction file in the [extern/ibsimu](extern/ibsimu) repository.
1. Make a directory called build and run `cmake ..`, then run `make`.

## Uninstall steps
1. Navigate to extern/ibsimu and run make uninstall
1. Uninstall dependencies used (on my mac I had to install automake, libtool, gtk+3, and gsl). It is probably best to just retrace build steps and uninstall anything installed in the process.
