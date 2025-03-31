# WOPA_SURF_2025
Git Repo for WOPA Summer 2025:

Waveguided Optical Parameteric Amplification (WOPA) is an experiment to generate several dB's of quantum squeezed light at a wavelength of 1064nm. The goal is to input 532nm (green) light into a Periodically Poled Lithium Niobate (PPLN) Crystal Waveguide through a single pass, generating a quantum squeezed 1064nm beam at the output of the crystal. The squeezed 1064nm beam then combines and co-propagates with a non-squeezed 1064nm beam (called a Local Oscillator (LO)), generating a combined squeezing affect of the LO. The eventual purpose is to generate > 6dBs of squeezed light meant to be used for the LIGO interferometer.

Logs of any progress made in the lab can be found in the [QIL Elog](https://nodus.ligo.caltech.edu:8081/QIL/)

## Getting Started
- Basic information on squeezed light within the LIGO detectors can be found here: [LIGO Squeezing](https://www.ligo.caltech.edu/news/ligo20231023)
- For an introduction on what squeezing is, the paper [Squeezed States of Light](https://github.com/user-attachments/files/19538666/Basic_Squeezing.pdf) by by Teich and Saleh is a great introduction.
- For a genral overview of nonlinear optics, material properties of PPLN waveguides, periodic poling, and configurations using nonlinear optics, the [PPLN Guide Overview](https://www.hcphotonics.com/ppln-guide-overview) from HCP Photonics will be very useful.

## Useful Modeling Software
- Using Conda: Prior to any modeling software installation, it is useful for one to install [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) (either Miniconda or Miniforge works). It allows users to install environments within their computer's command line, and install software packages such as FINESSE. 
- [FINESSE](https://finesse.ifosim.org/docs/latest/getting_started/index.html) is a free software package used in tandem with python (commonly installed via a command line). It is very useful to model anything lasers and optics related. It's very commonly used in LIGO. The link provides instructions on how to install and use FINESSE, as well as many examples.
- [LUMERICAL](https://www.lumerical.com/) is a commercial software useful for high-precison modeling. Could be very useful for us in modeling realistic affects of the waveguide such as thermal lensing.
