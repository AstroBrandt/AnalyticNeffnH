# Estimating attenuating column density from number density
This repository contains an example Jupyter notebook to demonstrate a few different types of calculations using the analytic method presented in Gaches 2025 (A&A accepted). The method requires a number of parameter inputs, many of which can be derived from macroscopic investigations of a molecular cloud, such as the linewidth-size relation, virial parameter, and temperature (or sound speed).

## Example notebook
The example notebook uses astropy for units (which is useful for good sanity checks!), along with matplotlib, numpy and scipy. It currently also uses cmasher for a colormap for the parameter space plot. If you do not have cmasher, you should get it anyways since it's a wonderful colormap package for python! If you still don't want to, you can just change the colormap in that plot to anything you like (matplotlib's viridis is closest).

The notebook creates the following plots:
- A plot of the relevant length scales for the turbulent column density component. The plot demonstrates the usefulness of the chosen filter function for requiring that the turbulent length scale is confined to the cloud size.
- A plot of the attenuating column vs number density for the fiducial model (Figure 2 of the paper)
- The parameter space investigation for the attenuating column (Figure 3)
- The slopes of the parameter space plots (Figure B.1)
- A new plot showing the attenuating column for the fiducial parameters, except the sound speed/temperature is a free parameter. The figure is a 2D plot of the attenuating column for solar neighborhood-like clouds as a function of density and temperature.
