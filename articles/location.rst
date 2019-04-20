Locations, Coordinates, Levels
==============================

..  toctree::
    :maxdepth: 2
    :caption: Locations, Coordinates, Levels

	
	
``Location of point elements``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
	
	.. code-block:: python
	
		##Grabbing Min and Max points of a crop box
		maxXYZ = revit.activeview.CropBox.Max
		minXYZ = revit.activeview.CropBox.Min
		##http://www.revitapidocs.com/2018.1/c2fd995c-95c0-58fb-f5de-f3246cbc5600.htm
		##individual double for each coord
		minX = minXYZ.X
		minY = minXYZ.Y
		minZ = minXYZ.Z
	
	