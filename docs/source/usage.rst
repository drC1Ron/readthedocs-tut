Usage
=====

.. _installation:

Installation
------------

To use drC1Ron, first install it using pip:

.. code-block:: console

   (.venv) $ pip install drC1Ron

Creating agents
----------------

To retrieve a list of random agents,
you can use the ``obj.get_random_agents()`` function:

.. autofunction:: obj.get_random_agents

The ``kind`` parameter should be either ``"good"``, ``"bad"``,
or ``"god"``. Otherwise, :py:func:`obj.get_random_agent`
will raise an exception.

.. autoexception:: agent.InvalidKindError

For example:

>>> import drc1ron as obj
>>> obj.get_random_agent()
['good', 'bad', 'god']

