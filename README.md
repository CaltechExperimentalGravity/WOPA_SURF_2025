# WOPA_SURF_2025
Git Repo for WOPA Summer 2025:

Waveguided Optical Parameteric Amplification (WOPA) is an experiment to generate several dB's of quantum squeezed light at a wavelength of 1064nm. The goal is to input 532nm (green) light into a Periodically Poled Lithium Niobate (PPLN) Crystal Waveguide through a single pass, generating a quantum squeezed 1064nm beam at the output of the crystal. The squeezed 1064nm beam then combines and co-propagates with a non-squeezed 1064nm beam (called a Local Oscillator (LO)), generating a combined squeezing affect of the LO. The eventual purpose is to generate > 6dBs of squeezed light meant to be used for the LIGO interferometer.

Logs of any progress made in the lab can be found in the [QIL Elog](https://nodus.ligo.caltech.edu:8081/QIL/)

## Getting Started
- Basic information on squeezed light within the LIGO detectors can be found here: [LIGO Squeezing](https://www.ligo.caltech.edu/news/ligo20231023)
- Basics of [Frequency Domain](https://en.wikipedia.org/wiki/Frequency_domain) and [Power Spectral Density](https://en.wikipedia.org/wiki/Spectral_density)
- For an introduction on what squeezing is, the paper [Squeezed States of Light](https://github.com/user-attachments/files/19538666/Basic_Squeezing.pdf) by by Teich and Saleh is a great introduction.
- For a genral overview of nonlinear optics, material properties of PPLN waveguides, periodic poling, and configurations using nonlinear optics, the [PPLN Guide Overview](https://www.hcphotonics.com/ppln-guide-overview) from HCP Photonics will be very useful.
- For more general LIGO related things, highly recommend reading [Interferometer Techniques for Gravitational-Wave Detection](https://github.com/user-attachments/files/19712074/Finesse_Physics.pdf)


## Useful Modeling Software
- Using Conda: Prior to any modeling software installation, it is useful for one to install [Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) (either Miniconda or Miniforge works). It allows users to install environments within their computer's command line, and install software packages such as FINESSE. 
- [FINESSE](https://finesse.ifosim.org/docs/latest/getting_started/index.html) is a free software package used in tandem with python (commonly installed via a command line). It is very useful to model anything lasers and optics related. It's very commonly used in LIGO. The link provides instructions on how to install and use FINESSE, as well as many examples.
- [LUMERICAL](https://www.lumerical.com/) is a commercial software useful for high-precison modeling. Could be very useful for us in modeling realistic affects of the waveguide such as thermal lensing.

## For writing reports / drafts
![Reports Compilation](https://github.com/CaltechExperimentalGravity/SURFtemplate/actions/workflows/compile.yml/badge.svg)

Template git repo for SURF projects

## Latest automatic compiled reports (change directory link to your repo):
[SURF_Proposal.pdf](https://github.com/CaltechExperimentalGravity/WOPA_SURF_2025/blob/gh-pages/SURF_Proposal.pdf)

The automatic compilation is setup using [GitHub actions](https://docs.github.com/en/actions). When you add more tex files for your interim and final reports, do following:
* Go to .github/.workflows/compile.yml
* Add your new tex files to the step "Compile LaTeX document" at root_file option. See the comments to see how to add multiple files for compilation.
* Add copy command to the step "Create published directory" to copy the generated output to ./public directory. This is the directory that is uploaded to gh-pages branch.

Handling issues:
* (Discouraged) If your file is not in reports directory, you'll need to add it to paths in on.push dictionary.
* If something does not work, check the output by going to your repo page on GitHub, then click on Actions, and follow down to your job.
* For Latex compilation issues, see [https://github.com/xu-cheng/latex-action](https://github.com/xu-cheng/latex-action).
* For gh-pages upload issues, see [https://github.com/peaceiris/actions-gh-pages](https://github.com/peaceiris/actions-gh-pages).

Healthy repo habits: (see "Sample LaTeX Document for Reports" and "GIT, git.ligo.org, GitHub" sections on SURF101 page)
* Avoid spaces in directory and file names. Use camelCase or snake_case, as per preference.
* Do not upload any files to the Github webpage. Your repo should be cloned locally on your machine, and you should pull and push local changes through git over command line. See git tutorial in SURF101 page for detailed instructions.
* Download LaTeX onto your machine for editing your tex files locally. Commit and push changes to the repo for tex files as you would for any scripts. We know Overleaf is convenient, but it becomes more complicated to interface with git for version control. LaTeX download links can be found on the SURF101 page.
