Dealing With Elements
=====================

..  toctree::
    :maxdepth: 2
    :caption: Dealing With Elements
	
	
``elementId to element``
^^^^^^^^^^^^^^^^^^^^^^^^
    .. code-block:: python
	
		##where doc = __revit__.ActiveUIDocument.Document
		element = doc.GetElement(elementId)

``Element to ElementId``
^^^^^^^^^^^^^^^^^^^^^^^^
	.. code-block:: python
	
		elementId = element.Id
		
``Get a property of an element``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
	.. code-block:: python
		
		##The orientation property of a wall returns a normalvector
		##Showing which way the wall's external side is facing.
		normalvector = wall.Orientation

``Query an element for it's mark or other parameter``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
	.. code-block:: python
		
		##Mark can be replaced by any parameter the element has.
		##http://www.revitapidocs.com/2018.1/0cf342ef-c64f-b0b7-cbec-da8f3428a7dc.htm
		##This one returns a list, even if only one element
		markString = element.GetParameter("Mark")
		##Or... Returns the first match (order may be random or change)
		markString = element.LookupParameter("Mark").AsString()
		##Or... This is mark for everything but doors. DOOR_NUMBER for doors.
		##Other built in parameters:
		##http://www.revitapidocs.com/2018.1/fb011c91-be7e-f737-28c7-3f1e1917a0e0.htm
		markString = element.getParameter(BuiltInParameter.ALL_MODEL_MARK)
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				
				