![alt text](https://github.com/DExSI/DExSI/raw/master/images/DExSI_header.png "DExSI")


# **_Data Extraction for Stable Isotope-labelled metabolites analysed by GC-MS_**


DExSI is an interactive graphical software package which can be used to rapidly quantitate isotopologues for a wide variety of metabolites detected by gas chromatography-mass spectrometry (GC/MS). DExSI performs targeted automated metabolite identification, isotopologue mass (fractional labelling) and abundance determination and natural isotope abundance correction. DExSI provides a range of output options (i.e. tables, graphs and heatmaps) and is suitable for high throughput analyses.

As DExSI is designed to detect metabolites irrespective of the extent of isotopic labelling, this software may also be used to perform targeted analysis on unlabelled data sets.  

## Citation

**By using DExSI, you agree to cite the following paper in all publications which use the software, as stated in the 'Licence.txt' file:**
```
Dagley, M. J. and McConville, M. J. (2018) 
 DExSI: A new tool for the rapid quantitation of 13C-labelled metabolites detected by GC-MS.  Bioinformatics.  
```

*DExSI is made available without charge for non-commercial use only*.  See the [Licence.txt](https://github.com/DExSI/DExSI/blob/master/Licence.txt) file for details.

## Getting Started

To begin, follow the directions below to download and install DExSI.

### Prerequisites

DExSI requires:

  * 64-bit Microsoft Windows 7 or later.
  * 8 GB or more of RAM is recommended for large data sets.
  * Administrator rights to run the installer

### Installing

Download the **latest version** of DExSI (Version 1.10) from the link below:  

  [DExSI v.1.10](https://github.com/DExSI/DExSI/releases/download/v1.10/DExSI_setup.exe)  

Run **'DExSI_setup.exe'** with Administrator rights.

Follow the prompts in the graphical installer.  DExSI will install and will be added to the Start menu.

## Using DExSI

DExSI requires four sets of data (three of which can be created in DExSI):

  1.) **GC-MS data files in CDF format**  
  Be sure to include samples containing a mixture of known metabolites of interest to serve as an authentic standards mixture. Absolute quantitation can only be perfomed if an authentic standards mixture sample (ideally, three samples of known and varied amounts) is included in the data set.
  
  Data can be acquired in either SIM or SCAN mode.
  
  2.) **A DExSI _library_ file**  
  This customised list is created in DExSI and comprises each metabolite of interest, and key parameters including retention time, isotopologue series (unlabelled to maximally labelled masses), and the chemical formula of the parental ion.
  Both the chemical formula of the ion for quantitation and the maximum number of labelled atoms in the ion must be provided to perform natural isotope abundance correction and to calculate fractional labelling.
  
  _You will require a different library for each ionization (i.e. EI, NCI, PCI) and derivitization method, reflecting differences in the most suitable ion for quantitation for each metabolite resulting from these method changes._
  
  The use of retention time locking is recommended to minimise shifts in retention time between experiments, thereby limiting the need to modify the expected retention time in your library between experiments.  
  
  3.) **A DExSI _groups_ file**  
  This defines the grouping of your samples (replicates by type and time point).
  
  4.) **A DExSI _standards_ file**  
  This defines the name and amount of known standards in your known standard mixture, and is required for the absolute quantitation on metabolites.


For a detailed step-by-step guide to using DExSI, please refer to the [DExSI Quick Start Guide](https://github.com/DExSI/DExSI//blob/master/DExSI%20Quick%20Start%20Guide.pdf).  
Detailed help is available by selecting **'DExSI Help'** from the **Help** menu.

### GC-MS data files
DExSI reads GC-MS data files in CDF format.  You may need to convert your vendor-specific files to CDF format before you can begin to use DExSI.  Usually, this can be achieved by selecting 'Export data to AIA' format or similar.  

### Sample Files

Sample CDF files, DExSI library (for EI GC-MS), standards and groups files are included in the **'Sample Files'** folder located in the DExSI install directory (i.e. 'C:\Program Files\DExSI\Sample Files'). 


If you edit these files, it is recommended that you save your modified copy in another location.  

**Please be aware that libraries must be specific to the experimental conditions used (i.e. derivitization, GC method and ionization technique).  You will likely need to create your own library rather than modify the sample library provided.** 

## Built With

* [Python](http://www.python.org/) - version 2.7.11
* [NumPy](http://www.numpy.org/) - version 1.10.4
* [Matplotlib](https://matplotlib.org/) - version 1.5.1
* [pandas](http://pandas.pydata.org/) - version 0.17.1
* [SciPy](https://scipy.org/) - version 0.17.0
* [wxPython](https://www.wxpython.org/) - version 3.0.2.0
* [nuitka](http://www.nuitka.net/) - version 0.5.28.2
* [xlwt](http://www.python-excel.org/) - version 1.0.0

## Previous Versions

The first public version of DExSI is version 1.10.

## Authors

* **Michael Dagley**

## License

**This project is licensed for non-commercial use** - see the [Licence.txt](https://github.com/DExSI/DExSI/blob/master/Licence.txt) file for details.

Commercial users must arrange a separate licence for commercial use.
