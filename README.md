# SFR_GUI_Avantes
GUI for Single Fiber Reflectance Spectroscopy (SFR) measuruments with Avantes spectrometers. 

# Acquisition
Acquisition is currently focussed around two software timed (trigger mode = 0) Avantes spectrometer, one for VIS, one for NIR. By default, upon connection, it uses the full spectral range, but for both spectrometers the start and stop pixels can be adjusted to only reflect the relevant part of the spectrum. It is necessarry that the calibration spectra are acquired with exactly the same spectral range. Both VIS and NIR spectrometers can be operated and controlled indiviudally. 

# Saving
Each file gets a pre-fix (VIS/NIR), which is also used as an identifier in the scripts. The sample measurement is only saved to disk, upon clicking the save button, where as the calibration files are saved immedieatly. Your sample measurement can be given a name, whereas the REF and DARK are saved with the current timestamp. 

All data is stored as a csv file with colums: wavelength,counts and also a text file with all the spectrometer data is generated. 

# Analysis
When, for the VIS and NIR spectro indidivually, REF and DARK files are present, the reflectance spectrum gets visualized. When also an absolute calibration file is present, it gets converted to absolute reflectance instead of relative to REF. In the analysis tab (upcoming feature), the absolute reflectance spectra can be converted to tissue optical properties. 
