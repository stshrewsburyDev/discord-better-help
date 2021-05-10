discord-better-help
===================

Release v\ |version|.

.. image:: https://pepy.tech/badge/discord-better-help
    :target: https://pepy.tech/project/discord-better-help

.. image:: https://img.shields.io/pypi/v/discord-better-help.svg
    :target: https://pypi.org/project/discord-better-help/

.. image:: https://img.shields.io/pypi/pyversions/discord-better-help.svg
    :target: https://pypi.org/project/discord-better-help/

.. image:: https://img.shields.io/pypi/l/discord-better-help.svg
    :target: https://pypi.org/project/discord-better-help/

An extension module for `discord.py <https://pypi.org/project/discord.py/>`_ to make setting up a help command easier.

Based off of `discord-pretty-help <https://pypi.org/project/discord-pretty-help/>`_ by `StroupBSlayen <https://pypi.org/user/StroupBSlayen/>`_.

-------------------

**Simple usage example**

.. code-block:: python

    from discord.ext import commands
    from better_help import Help

    bot = commands.Bot(command_prefix="!", help_command=Help())


Overview
--------
.. toctree::
   :maxdepth: 2

   reference/index.rst
   changelogs/index.rst


Installation
------------

Install with pip
^^^^^^^^^^^^^^^^
::

    $ pip install discord-better-help

Update with pip
^^^^^^^^^^^^^^^
::

    $ pip install discord-better-help --upgrade

Install from source
^^^^^^^^^^^^^^^^^^^
::

    $ python setup.py install


Support
-------
If you have any problems with ``discord-better-help`` please let me know via `the GitHub issue tracker <https://github.com/stshrewsburyDev/discord-better-help/issues>`_.


Some useful links
-----------------

- Issue Tracker: https://github.com/stshrewsburyDev/discord-better-help/issues
- Source Code: https://github.com/stshrewsburyDev/discord-better-help


License
-------

The project is licensed under the `MIT license <https://mit-license.org/>`_. (`learn more <https://en.wikipedia.org/wiki/MIT_License>`_)
