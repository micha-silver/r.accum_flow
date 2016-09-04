# r.accum_flow
Total accumulated flow for segments in a  stream network

NAME
----
**r.accum_flow**

KEYWORDS
----------------------

DESCRIPTION
----------------------
Creates stream network (using r.stream.order) and adds flow accumulation for each stream segment, at both the start and end points of each segment. Total area of flow accumulation is in units specified by the `units` parameter (default square meters). The area contributing flow to each stream segment is added as two columns in the stream vector map: upstream_accum and downstream_accum for the start and end points of each segment, respectively.

REQUIRES
---------------------
GRASS 7.x
**r.stream.order** addon

SYNOPSIS
----------------------
**r.accum_flow**

**r.accum_flow** --help

**r.accum_flow** [**-d**] **elevation** = *name* **streams** = *name* **prefix** = *string* **thresh** = *integer*  [**units** = *string*]   [-- **overwrite**]  [-- **verbose**]  [-- **quiet**] 

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




