Alimentation 
============

Le site enob contient trois niveaux de contenus.

#. La description des "entités intellectuelles" (item) auxquelles sont rattachées les numérisations du fonds de l'INHA (media) 
   #. La description pages des entités intellectuelles
#. Les références bibliographiques mobilisées par JB   


.. _num:

Ajout de nouvelles numérisations
--------------------------------

To use Lumache, first install it using pip:

.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

