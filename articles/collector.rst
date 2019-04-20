Collecting all the (relevant) things!
=====================================

..  toctree::
    :maxdepth: 2
    :caption: Collecting...things

	
	
``Find all elements of a type in active view``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
OfClass docs:

http://www.revitapidocs.com/2018.1/b0a5f22c-6951-c3af-cd29-1f28f574035d.htm

Autodesk.Revit.DB Namespace, for categories to be filtered:

http://www.revitapidocs.com/2018.1/87546ba7-461b-c646-cbb1-2cb8f5bff8b2.htm


    .. code-block:: python
		
		##Where doc = __revit__.ActiveUIDocument.Document
		elementList = DB.FilteredElementCollector(doc, selected_view.Id)\
		.OfClass(DB.IndependentTag)\
		.ToElements()

Another collecting walls:

	.. code-block:: python
	
		collector = FilteredElementCollector(doc)\
		.OfCategory(BuiltInCategory.OST_Walls)\
		.WhereElementIsNotElementType()\
		.ToElements()