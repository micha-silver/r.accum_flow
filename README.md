# r.accum_flow
Total accumulated flow for segments in a  stream network
=================================
GRASS GIS manual: r.accum_flow.py
=================================

.. figure:: grass_logo.png
   :align: center
   :alt: GRASS logo

NAME
----
**r.accum_flow.py** - Create stream network with flow accumulation for each stream segment

KEYWORDS
----------------------

SYNOPSIS
----------------------
**r.accum_flow.py**

**r.accum_flow.py** --help

**r.accum_flow.py** [**-d**] **elevation** = *name* **streams** = *name* **prefix** = *string* **thresh** = *integer*  [**units** = *string*]   [-- **overwrite**]  [-- **verbose**]  [-- **quiet**] 

Flags:
~~~~~~
**-d**
    Delete temporary rasters
-- **overwrite**
    Allow output files to overwrite existing files
-- **verbose**
    Verbose module output
-- **quiet**
    Quiet module output


Parameters:
~~~~~~~~~~~
**elevation** = *name* **[required]**

	Input elevation raster:


**streams** = *name* **[required]**

	Name for output streams vector map:


**prefix** = *string* **[required]**

	Prefix prepended to output map names (temp maps)


**thresh** = *integer* **[required]**

	Threshold minimum basin size (as in r.watershed)


**units** = *string*

	Units for area calculation. Values: meters, kilometers, feet, miles, hectares, acres (default: meters)

	Options: *meters, kilometers, feet, miles, hectares, acres*

	Default: *meters*





