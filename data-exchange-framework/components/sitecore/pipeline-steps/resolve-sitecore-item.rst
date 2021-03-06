Resolve Sitecore Item
=============================

This *pipeline step* is used to find a Sitecore item using the campaign identifier.

+-----------------------------------+-----------------------------------------------------------------------+
| Template name                     | **Resolve Sitecore Item Pipeline Step**                               |
+-----------------------------------+-----------------------------------------------------------------------+
| Base template                     | :doc:`base-resolve-object`                                            |
+-----------------------------------+-----------------------------------------------------------------------+

.. |value-accessor| replace:: :doc:`../data-access/value-accessors/item-field-value`

+-------------------------------------------------+---------------------------------------------------------+
| Field                                           | Description                                             |
+=================================================+=========================================================+
| | ``Parent for item to resolve``                | | This item is used as the starting point for the       |
|                                                 | | search.                                               |
+-------------------------------------------------+---------------------------------------------------------+
| | ``Value accessor for Sitecore item``          | | A search is built that looks for an item with a       |
| | ``field used to match the identifier value``  | | field whose value matches the identifier value.       |
|                                                 | | This field specifies which field on the item is       |
|                                                 | | used in the query.                                    |
|                                                 | |                                                       |
|                                                 | | The value accessor must be an item based on the       |
|                                                 | | template |value-accessor|.                            |
+-------------------------------------------------+---------------------------------------------------------+
| | ``Template for new item``                     | | If a new item is created, this is the template that   |
|                                                 | | is used.                                              |
+-------------------------------------------------+---------------------------------------------------------+
| | ``Value accessor for name for new item``      | | If a new item is created, this value accessor is used |
|                                                 | | on the identifier object. The value that is read is   |
|                                                 | | used as the name for the new item.                    |
+-------------------------------------------------+---------------------------------------------------------+
