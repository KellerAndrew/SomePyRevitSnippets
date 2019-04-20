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