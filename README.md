# AP2-DV-file
this is a small project to read and plot the data from TESS's DV file.
We will read the data validation file of TIC 100100827 (known to have at least one planet, WASP-18 b) from Sector 2 using the MAST URL location.
the file is of FITS (Flexible Image Transport System)Format .
The DVT FITS file consits of a primary HDU with metadata stored in the header, and one FITS extension HDU per TCE found in the lightcurve of the specified TIC ID. These extensions contain the detrended flux time series phased to the orbital period of the signal, stored as a binary FITS table. The last extension HDU always contains some additional statistics about the search, also stored in a binary FITS table.
we open the FITS file and extract some metadata from the headers. 
then we make a plot of detrended fluxes and model fluxes vs orbital phase
