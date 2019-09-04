# NSIDC Polar Stereographic Projection

Legacy Fortran and IDL utilities for converting polar stereographic coordinates.

To access the Python repository, see [polar_stereo_passivemicrowave](https://github.com/nsidc/polar_stereo.git).

NSIDC's polar stereographic projection specifies a projection plane or grid tangent to the Earth's surface at 70° northern and southern latitude. While this increases the distortion at the poles by six percent and decreases the distortion at the grid boundaries by the same amount, the latitude of 70° was selected so that little or no distortion would occur in the marginal ice zone.

This repo contains conversion routines between longitude/latitude and generic x, y (km) coordinates. There are also conversion routines between longitude/latitude and i, j grid coordinates for specific datasets for AMSR-E and SSM/I.

See also [Polar Stereo Overview](https://nsidc.org/data/polar-stereo).

## Level of Support

* This repository is not actively supported by NSIDC but we welcome issue submissions and pull requests in order to foster community contribution.

See the [LICENSE](LICENSE.md) for details on permissions and warranties.  Please contact nsidc@nsidc.org for more information.

## Requirements

* Fortran 77 or 90
* IDL 6.0 or higher

## Installation

No special installation is needed

## Usage

See the individual files for details.  

### FORTRAN Code

**mapll.for** (_obsolete_): Convert from latitude and longitude to Polar Stereographic x, y (km).

**mapxy.for** (_obsolete_): Convert from Polar Stereographic x, y (km) to latitude and longitude.

**locate.for** (_obsolete_): Transform I,J coordinates of an SSM/I grid cell to latitude and longitude and vice versa.

### IDL Code

**extract_ice.pro** (_obsolete_): Extract sea ice concentrations from Polar Stereographic grid files.

**disp_ssmi_ice_xa.pro** (_obsolete_): Create animations of sea ice concentrations from SSM/I Polar Grids.

## License

See [LICENSE](LICENSE.md)

## Code of Conduct

See [Code of Conduct](CODE_OF_CONDUCT.md).

## Credit

This software was developed by the National Snow and Ice Data Center with funding from multiple sources.
